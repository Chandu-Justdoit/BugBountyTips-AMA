---
layout: post
title:  "Spend more time doing recon, you’ll find more BUGS"
categories: write-ups

author:
  name: Vedant Tekale
  twitter: Vegeta
  picture: images/Vedant Tekale.jpg
  links:
    - title: Twitter
      url: https://twitter.com/_justYnot
      icon: fab fa-twitter-square
  
  
--- 


# Spend more time doing recon, you’ll find more BUGS

Hello again great #bugbounty community! My name is Vedant(Also known as Vegeta on Twitter😁) and I’m a cybersecurity enthusiast and an aspiring Bug hunter :) I’m learning and doing bug hunting for about 6 months now and I really love what I do. So from August I spent more time learning different methodologies of doing “Recon” and recon is the most important phase of bug hunting. Today I’ll share a story about my recent findings and a way of recon that I tried for first time. So lets begin.

<br> ![](https://cdn-images-1.medium.com/max/2000/1*Yg5pQfjaK1LM8gwk3CSzyA.png)


<img src="/images/batman.gif" width="663" height="340" />

So whenever I pick a program and start recon I always try collect all of its subdomains and then start fingerprinting, fuzzing and all other things. But this time I used a different approach. I recently watched a video of [Jason](https://twitter.com/jhaddix?lang=en) Haddix about the bug hunting methodology and I learned about the ASNs and CIDR. So I was hunting on a private program which had all of its assets owned in scope and I already found some great bugs like information disclosure, SSRF and XSS on some of its subdomains but some of them got duped. So one day I decided to take a different approach and I visited [https://whois.arin.net/ui/](https://whois.arin.net/ui/) and searched for the target name and got some results. There I got the CIDR of my target which is nothing but the range of IPs the target company owns. Then I used a tool known as [masscan ](https://github.com/robertdavidgraham/masscan)to scan the range of IPs and I used the following command :-

      bin/massscan — range CIDR_here -p 80, 443, 8080, 8443 -oG results.txt — rate 10000

![Masscan](https://cdn-images-1.medium.com/max/2516/1*NINOBBsYG1jVXvpGtlyNCA.png)

*Masscan*

After the scan completed there were about 140 IPs in the output file so I used aquatone to screenshot all the IPs and for that I used the following command:-

      cat results.txt | aquatone -out ~aquatone/target

Then I was checking all the screenshots one by one and after some time I saw that some IPs had JIRA dashboard running on them. I checked the version and it was 7.3.3 , I quickly googled for Jira 7.3.3 vulnerabilities and got the [results ](https://www.cvedetails.com/vulnerability-list/vendor_id-3578/product_id-8170/version_id-236326/Atlassian-Jira-7.3.3.html)and I was like,

<img src="/images/tenor2.gif" width="663" height="318" />

I read some of the CVEs and after going through each of them one by one I got the CVE-2018ΓÇô20824 which is a reflected XSS vulnerability. I quickly googled about its exploits and got one. I copied the exploit path and appended it to one IP which had JIRA dashboard and YEAHH!! XSS triggered successfully. After that I tried for the same on all other IPs which had JIRA dashboard running and all of them were vulnerable :)

So instead of manually checking for all other CVEs I used the tool known as [Nuclei ](https://github.com/projectdiscovery/nuclei). I used the following command :-

     nuclei -t /path/to/nuclei-templates/cves/ -l results.txt -o nuclei_cve.txt -c 200


![Nuclei output](https://cdn-images-1.medium.com/max/2000/1*_mCDAs2vrJ6iQKNH_OwKfw.png) 
 
 *Nuclei output*


And after some time I got some IPs which were vulnerable to the CVEs such as CVE-2019ΓÇô8449 and CVE-2020ΓÇô14179 which lead to information disclosure. This was the first time I got so many bugs in very short time and I was very happy with this.

<img src="/images/tenor3.gif" width="663" height="406" />

I made some good reports and sent it to the target company. Some of them got duped and few of them got accepted 😂😂😂 but I learned a lot from this and I always say to myself that “I never lose, I either win or I learn”.

I hope you learned something new from this writeup and if you have any doubts or questions about it you can get in touch with me [HERE](https://twitter.com/_justYnot). I daily learn a lot of new things from this awesome community so I'm trying to give something back to the commnity by sharing such writeups and #bugbountytips on Twitter.

Thank you so much for reading and happy breaking!
