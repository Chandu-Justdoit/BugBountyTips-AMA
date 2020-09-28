---
layout: post
title:  "Infosec Bugbounty  AMA with Debangshu kundu"
categories: infosec-bugbounty-ama
image:
  path: /images/DK.jpg
---

# AMA with [Debangshu_kundu](https://twitter.com/debangshu_kundu)

<br>

- Glad to be a part of this awesome series!
   
  - ***Thanks for accepting the invite !***

<br>

- What originally got you into hacking?
 
 - ***I was fascinated by tech from an early age just like you guys, once I saw a social engg. video on YouTube, it got me intrigued. I searched more and more,then found out what defacing is, maybe did a couple lol. Day by day i grew more attracted to it! This is what initiated it.***

<br>

- Why do you find it so fun?
  
   - ***It gives me an adrenaline rush! My dopamine levels get super high! Slowly slowly you get addicted to this feeling, like Oh noo this shouldn't be accessible, yes P1! And you can't get enough of it :)***

<br>

- What is your approach while looking for bugs in main web application?
  
  - ***First of all fingerprinting the application! Detecting which technologies or CMS is running. If its aem, I'll search for querybuilder, get servlet, POST servlet, groovy console, etc. If its wordpress, I'll search known exploits, same for all the other CMSes.*** 

<br>

- Generally which functions you target to find bugs?Thanks in advance :)
  
  - ***Functions?
1) Impersonation can i pose as another user? Can I send custom emails?
2) upload functionality!
3) download functionality! Specially pdfs and invoices!
4) Testing lesser known input fields
5) Testing CSRF on less tested functions like deleting bookmarks
6) Homograph attacks
7) Lack of X-FRAME-Options on critical endpoints
8) Testing IDOR cross-platform/cross tenant***

<br>

- Homograph attack in which feature? Any examples
  
  - ***Could be used to reset the admin password of http://target.com if you can fetch it in http://tàrget.com or similar
https://hackerone.com/reports/861940
Here's one example. The redirect_uri param didn't check input correctly***

<br>

- What is the first bug you found?
   
   - ***First bug : Information disclosure***

<br>

- What was the best or most memorable bug you found?
   
   - ***Most memorable: LFI that I and @ArmanSameer95 found :)***

<br>

- What was the insane bug you found and thought how stupid is this developer?
  
   - ***Stupid: Found a pastebin data dump was probably a scan leaking tenant creds lol***

<br>

- How I important you found reading about cve in bugbounty?
   
  - ***Subscribing to @CVEnew is the best thing yoh can do for yourself lol***

<br>

- Advice for beginners like me?
   
  - ***Lastly, strengthen your basics while actively exploring new vulnerabilities***

<br>

- finding subdomains and finding  livedomains(https or http)what is your next step..?
   
  - ***next i use aquatone to get screenshots and fingerprint headers***

<br>

- which wordlist you use and tips for LFI &INFORMATION DISCLOSURE
   
  - ***Raftlists and commonspeak wordlists. For fetching local files, use upload and download functionality, any functionality that tries to fetch a absolute/relative path/resource could be an entry point for LFI***

<br>

- Tips for Beginner's..?
   
  - ***Google stuff you don't know! Whether its an endpoint or technology, google has it all :)***

<br>

- Do you use notes while bughunting, and if so how do you take notes while hunting?
  
   - ***yeah definitely! I use sublime for quick notes, sometime whatsapp web too, and using swiftnessX for detailed notes or approach mindmaps***

- Do you follow a set procedure or methodology, or do you just smash at everything on sight?
   
  - ***Well I started by smashing everything at sight but gradually I'm getting into more of a methodology, but its tough to stick to one!***

<br>

- Tips to start BugBounty?
  
  - ***A brain and google[dot]com is enough ;)***

<br>

- How  did you get started in bug hunting
   
   - ***I was into hacking for quite some time already, so I was familiar with certain stuff, then blogs, whitepapers, labs, etc made the way!***

<br>

- And any advice for beginers 
  
   - ***For beginners, strengthen your base while focusing on newer vulns/exploits/research, it'll help you understand better***

<br>

- You do bug hunting as full time or part time (including time for how long you hunt a day)
  
   - ***I hunt when i feel like, mostly from evening to late night. In morning i focus on reading stuff and taking notes***

<br>

- How long have you been bug hunting
  
  - ***Its been 8 months!***

<br>

- what else you do other then bug hunting.
   
    - ***Other than bughunting, I eat, sleep, roam about and play COD***

<br>

- At what age you started bug hunting and in how many days you found your first bug...?
   
   - ***)I started hunting at 16. It took me around 2.5 months to get my first, it was 50 bucks. ***

<br>

- What was your Suggestions for beginners
   
  - ***strengthen your basics while focusing on newer things. E.g. Maybe learn a bit of PHP to understand that DEFCON talk better or learn a bit of JS to get the impact of that XSS higher!***

<br>

- Any tips in finding Idors
   
  - ***My man @swaysThinking has created an awesome compilation on IDOR! https://notion.so/IDOR-Attack-vectors-exploitation-bypasses-and-chains-0b73eb18e9b640ce8c337af83f397a6b
Check it out! Kudos to him!***

<br>

- how to tackle with duplicates as i am getting only duplicates!! Is there a good scope in app testing also?
  
 - ***Leave the class of bugs that you maybe looking into and focus on something new probably. Something other people won't bother looking. Checkout @jon_bottarini's disclose reports. Lots to learn from him.There's lesser competition in mobile apps, might as well go for that.***

<br>

- Any alternative for burp collabarater for those who don't have buro suite pro
   
  - ***http://canarytokens.com is a great alternative. The only drawback is that it doesn't provide custom subdomains. But provides features for specific functions and even emails it to you!***

<br>

- I wanted to ask this during your talk, due to time delay couldn't do it. You said you look for cve frequently, but most of the time cve comes with no explanation discription or poc, how do you find the exploitation?
   
  - ***I just wait until the exploit is public :P also, the sources you get exploit from matters, maybe there's some abc website/person who's already uploaded a poc and the ones where you normally look haven't already

<br>

- Any tips for ssrf and PII bugs.I'm using only burpsuite and Google Chrome as tools. Can I succeed with these tools?
   
  - ***Tools don't matter, your brain does.For SSRF, observe every function minutely and take a note of the functions that probe an URL, path or any other protocol. 
Check waybackurls, alienvault and google dorks to find lesser known paths that may reveal any PII

<br>

- How a beginner should chosen programs to hunt? Should he go for new programs or old programs?
   
  - ***There are quite a few public programs on h1 and bugcrowd both, that are unnoticed by the majority of the crowd. 
Check when the last report was resolved or try out RDPs. Turn on notifications for @disclosedh1 for fresh programs!***

<br>

- What is your process for moving from a dump of recon data to few dozen endpoints which look interesting ?Am i suppossed to know (or i can learn) how to  see through list of  [functions|Parameters|Url] &pick prob vuln ones Or is this just an experience thing that i can't learn
  
  - ***Yeah, there is experience involved too but you'll be good to go if you can simply google! Use httpscreenshot for mass-screenshotting of endpoints.Well my focus will be on 200 OK endpoints with unique content-length. Google is the most powerful tool out there, you can simply Google the endpoint you found to know about it. If you have problem in that, fingerprint the technologies and search docs! Might prove useful.***

<br>

- Bro what's your perspective while you search for Info Disclosures? &  which will force u like ..  "Hey !! here's something suspicious I've to spend time on looking this"
:)
  
  - ***Weird behaviour like forced redirect is alarming! Any 200 OK response on critical endpoints with different content-length gets me excited!***

<br>

- Can you put some more light into force redirect? Do u mean 302 on sensitive endpoints? Do u try bypasses on it? Or something else
   
   - ***I'll share a recent example.
Found a spring boot endpoint, rewarded, fixed. Was originally on http://sandboxsub.com/endpoint . After fix it redirected me to http://domain.com/endpoint and returned 404
So i used http://sandboxsub.com/..;/endpoint and it didn't redirect me! Instead displayed basic auth

<br>

- Burp suite extensions that you use
   
   - ***I use Taborator, Param miner that's it :)***

<br>

- Any specific lab,source that you are aware of to learn sqli from basic to advanced level?(Including the blind sqli!)
   
  - ***No single resource, will help you in that. Watch, learn, adapt. Portswigger labs will help you get started. Then understand how SQL queries are formed (development phase) then start looking and experimenting for bypasses :)***

<br>

- Do you think focusing on specific class of bugs and hunting for them  helps rather than looking and  hunting for every type
   
  - ***Yeah kind of, like, I have a favorite zone like Information Disclosure and PII Leakage but a lot of times you have to adapt and come out of that comfort zone to score some bugs :) But if you're a beginner, feel free to stick to a particular one untill you master it :)***

<br>

- What makes a program interesting for you to hack on? Or, how do you decide you want to hack on a specific program?
   
  - ***The larger the scope, the more interested I am!Most probably *.foo.com will get me going! Also, payment times! No one wants to wait months to get paid up! :)***

<br>

- I got 3 private programs where should i begin web or app?
   
  - ***Totally depends on what you are comfortable with!Android targets are likely to be less crowded,But if you're more comfortable with webapp, start with that!***

<br>

- What is your methodology to approach information disclosure and LFI Thank you:)
   
  - ***Test upload/download functionality. Check for storage buckets. Grep for absolute and relative paths that seem to be fetching some internal resource :)
Use dorks well...***

<br>

- Which is the best fuzzing tool? ffuf, wfuzz, gobuster, dirbuster or any other?
   
   - ***Each has their own merits/demerits.I personally use dirsearch :)***

<br>

- any tips to find sensitive information?
    
    - ***Recon is king! From github to gitlab, trello, pastebin, and all other content-pasting sites that are indexed easily are worth a shot. Scan JS files nicely and keep an eye on chrome's network tab :)***

<br>

- What do you do toh keep yourself motivated in the burnout phase??
    
   - ***I just disconnect from bughunting and focus more on reading/implementing new stuff, maybe improve my existing approach and chill out, go riding with my cycle

<br>

- do you follow any kind of roadmap for bug hunting??
   
   - ***Not any exact roadmap, just functions which seem interesting, i target them.***

<br>

- Do you make your own wordlists or use existing ones? What wordlists do u use ( if it's an existing one)
   
  - ***It depends. Normally a combination of different RAFTlists and commonspeak wordlists. Only if the target is something specific like AEM, I'll use my own.***

<br>

- What is the story how you get interest in hacking?
   
  - ***Random YouTube videos, seeing defaced websites and curiousity to experiment with applications drove me to this.***

<br>

- Your fav bugs?
   
 - ***Information disclosure, anything involving PII, RCE***

<br>

- How you manage your time between hacking and study?
   
 - ***It's tough to balance, opted for a non-attending school for the same.***

<br>

- How you make use of shodan while bug hunting
   
 - ***Some dorks like Org:Target ssl:target fetch you list of IPs and instances belonging to the target that you wouldn't normally find ;)***

<br>

- List of RFCs you can think of to learn from related to web, that create a stackoverflow in my brain
  
 -  ***Http itself
Websockets
Email RFC
DNS
Ftp
Icmp
Ipv4/v6
Ldap
Kerberos
Utf-8!***

<br>

- Any tips for new bug hunters?
   
   ***Build a balance between exploring new stuff and at the same time strengthening your basics!***

<br>

- Write an essay on not less than 300 words on how to find sensitive endpoint and start fuzzing. Where to stop. What's the unique thing in your fuzzing. 
   
  - ***Best guy for fuzzing! @pwntester
     Just stop when your brains feels, its too much, grab a drink, chill out and get back again.
     I met @ArmanSameer95 in intigriti's comment section on instagram lol***

<br>

- Any tips for new bug hunters?
    
   - ***Build a balance between exploring new stuff and at the same time strengthening your basics!***

<br>

- Bro, how dp you fingerprint internal applications running on a webserver ? What methodology yoiu will recommend else running FavFreak.
   
  - ***Checking the HTTP responses on multiple endpoints, possibly upload/download or critical functions might help. Try adding new headers, might help. Also, check exifdata of an uploaded document, might reveal something. Once I checked for exif and found they were using imagemagick Wasn't able to get that rce, since program closed but it helped in fingerprinting :)***

<br>

- How to bypass waf for xss. Generic examples or resources
   
 - ***Here You go
     https://github.com/R0X4R/D4rkXSS
     https://github.com/s0md3v/AwesomeXSS
  https://owasp.org/www-community/xss-filter-evasion-cheatsheet***

<br>

- Any tips for begginers in Android Bug Hunting ?
   
  - ***Sorry mate, I'm not into android hunting. But @B3nac has awesome content on android hacking! Specially the Injured Android is great stuff to start with :)***

<br>

- which one should i do first hack_the box or portswigger ?for web hacking
   
  - ***Portswigger In my opinion!***

<br>

- Your favourite tool?
   
 - ***@Burp_Suite:)***

<br>

- Give some tips for beginners who wants to come in cyber security field
   
 - ***Build your basics (all about HTTP)
A bit on networking, Learn a bit about diff web technologies, web languages.
A scripting language like py, rust or go will be beneficial. learn linux. Google terms of basic web hacking, understand them. Read a lot of blogs, experiment with stuff
Whenever you come across an unfamiliar term, Don't ask anyone, simply google it***



