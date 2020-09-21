# AMA with Aditya Shende(@ADITYASHENDE17)

<br>

# About Aditya Shende 😎 and His Success 💪


- Bhai when did you started bug hunting, what were you doing before bug hunting,how did you got started in bug hunting and what was your highest bounty ever.
Thank You
 
  - ***In middle of 11th I started this stuff with very skid skills. I used participate into boxing , taekwondo and kick boxing. I started bb coz my friend suggestion and I made 10k$ (my highest)***

<br>

- Will you do bug bounties for full time after graduating also

    - ***No , I'll take bb as part time. Willing to do MS in cyber security***

<br>

- What your plan after graduating this year? Like full time bug bounty or joining security team in some organization.

   - ***Gonna do MS and then dream to join in Google***

<br>

- Which is Worst N/A you found ever? and Which is the Best bug u found Ever?
 
   - ***My cve based rce got NA .  Best bug I found:  Desk access to rce***

<br>

- was that CVE released within a month when you reported
 
   - ***2019-11581***

<br>

- What is your favorite note-taking app?
 
   - ***Pen and paper***

<br>


-  what are your goals for next 5 years? Or where do you see yourself in next 5 years? And and and, Thanks for all the contributions you have done for the community! Respect
  
    - ***Buy a house and a special area for my all bikes. I want to work with google***

<br>

# Tips for Beginners 🔰
 
- What will you suggest for begginers
 
   - ***Rdp at 1st phase***

<br>

- books which you have read and found valueable 
And what resources do you use to keep yourself up-to-date
 
   - ***All reading about blackhat conf. PDF and slides are available***

<br>

- What would be the things you will tell your younger self, when he is starting his bugbounty journey?

   - ***Me to younger me: Buddy don’t go for money, you’ll get that but don’t be fast and take care of health***

<br>

- When going through targets subdomain list how would we know a particular domain may have bug or show we go through each and every domain(my target has a lot of subdomains)

    - ***I always check each and every sub , There is no special power to assume this one is buggy or not***

<br>

- How your approach for bug hunting differs for a target which have all assets in scope versus only main application in scope?
Thanks in advance

  - ***Scan for each and single target. 1st step to get all urls and check for valid urls. Side by side fuzzing . I do check main application 1st because everyone thinks it’s secure***

<br>

- What bugs to focus as a beginner I wanna learn about all the critical bugs but not possible to find it on programs.
Any tips for critical vulns finding?

   - ***Always try to find high paid bugs . Rce, ssrf, information disclosure etc. for that you can read slide of blackhat and Hackerone reports***

<br>

- When I see a target as "*.site.com " that means that I'm able to hack on that domain and any sub-domain under that domain ? Please help me I'm too confused and also just started my journey.
 
    - ***Yes . You can test all domains + subs. And also check oos domains because some subs are in oos***

<br>

- We used to follow your achievements steps as easy 1, 2, 3.
  Can you post your recon as that 1, 2, 3?
 
  - ***Sub domains enum and sorting into live***
  - ***Wayback , dirsearch, ffuf for brute forcing meanwhile github recon, checking js files. And api ep too***
  - ***Using known vulns to chain with another bug, Few templates created for nuclei, Function check + exploit.***
  - ***Burp: Playing with req***

<br>

- Finding all parameter seems to be a very good idea for manual testing phase. I just wonder for what else purpose they can be utilized.
 
   - ***Xss, ssrf, debug errors, user circumvented vulns(idors), redirections, sometimes rce, oauth bugs etc***

<br>

- Also, one question more, I have been ignoring this question for a while, but now I guess I should ask, what does 0days or something like that mean? What's 0 in that? Sorry, This might be the silliest question, but yeah.
   
    - ***Zero-day is a bug in software, application, hardware or firmware that is unknown to the party or those who are responsible for it which hits all service who are using the vendor application or software.***

<br>

# Tips to Approach A target 🎯

- When approaching a Target, what are first things that come into your Mind that you should hunt for? 
Also, How to not get distracted from other things? (This might be a relative term, but still What points you might consider in General? ) 
Much love

  - ***Recon is common but view is different. Analysis of js files for information, fuzzing, default urls, understand function etc. If you are very passionate about your target then there is no thing to distract***

<br>

- How do you approach a target and any tips for business logic errors
 
  - ***Mostly using tools of project discovery for subdomain enumeration,  parsing, sorting into valid one . Subfinder, httpx, shuffledns and nuclei. For finding all urls or path I use wayback. Mostly that helps me to find information disclosure and sometimes unauthorised access.***

<br>

-  How do you approach multiple JavaScript endpoints? (Tools, Flow, methods)?
 
    - `https://web.archive.org/cdx/search/cdx?url=*.target.com/*&output=text&fl=original&collapse=urlkey`
     
      
   - ***Multiple tools you can use , In my study OTX, GAU, wayback and gron for sorting helped me alot. Another part I am really weak at xss***

<br> 

- 1.How to develop intuition about the type of vulnerability and vulnerable site.
  2. What are the checklist you follow while checking for vulnerability.3. Sir I have found a vulnerability (open redirect) bt.  unable to explain the triage team that how I found it. What to do???
 
    - ***There is no specific checklist which I follow. I hunt application as per feature. Instead developing scenario read about techniques and implement while testing. From my point of view I was testing bugs on local sites obviously its not legit but I was curious about learning.***

<br> 

- How your approach for bug hunting differs for a target which have all assets in scope versus only main application in scope?
Thanks in advance

   - ***Scan for each and single target. 1st step to get all urls and check for valid urls. Side by side fuzzing . I do check main application 1st because everyone thinks it’s secure***

<br>

- I get annoyed after a while hunting the target.
   1.Can you tell how long and how should I approach a target, so that I can find bugs like you?,
   2. How to approach a target where there is no auth?
 
    - ***If I found target don’t have much more function except register and login, I’ll leave that target. Or else I start to fuzz the same target. Simple rule : no functions no bugs.
 Js files check, source code view for sensitive keywords, dirsearch, ffuf, git recon if target is high***

<br>
 
 # Tools for Sensitive Information ℹ

- In Terms of Content Discovery, 
What Tools Should We Use To Enumerate Paths, Parameters, Endpoints etc.

  - ***Dirsearch, ffuf, wfuzz, paramspider, gf patterns***

<br>

# Tips for Business logic errors ⚠️

- How do you approach a target and any tips for business logic errors
 
  - ***Mostly using tools of project discovery for subdomain enumeration,  parsing, sorting into valid one . Subfinder, httpx, shuffledns and nuclei. For finding all urls or path I use wayback. Mostly that helps me to find information disclosure and sometimes unauthorised access.***

<br>

# Tips for RCE 🏇

- Any new techniques for RateLimit_Bypass?
 
   - ***Add multiple headers in request, put null chars in end of endpoint, Sometimes protection is on time so slow down requests***

<br>

# Tips For API-Hunting 💻

- What will be your step by step methodology while testing for bugs in APIs?
  
  - ***Discovery testing, documentation functional api, calling another function, fuzzing api ep with api list of random robbie. Inducing application to make call on different methods. Main part Parameter Combination, Parameter Selection, and Call Sequencing.***

<br>

# Tips for Injection 💉

- Any suggestion for SQL injection? How I approach for this vulnerability
Thank you 

  - ***I am not into common findings but this one will help you https://blackhat.com/presentations/bh-usa-04/bh-us-04-hotchkies/bh-us-04-hotchkies.pdf
 There are many resources but I prefer http://securityidiots.com/Web-Pentest/SQL-Injection***

<br>

- in main application you actively look for ways to abuse particular functionality right?
 
   - ***Yes . Mostly feedback form for blind os injection***

<br>

- How you look for Information disclosure on OTX or or how you can test OS injection on feedback form or somewhere else.
  
   - ***Instead of otx u can use wayback, I use multiple for more results and there is lab on os    injection in port swigger , cmdi pdf of blackhat also available***

<br>

# Tips for Recon 🔍

- We used to follow your achievements steps as easy 1, 2, 3.
  Can you post your recon as that 1, 2, 3?
 
  - ***1. Sub domains enum and sorting into live,2. Wayback , dirsearch, ffuf for brute forcing meanwhile github recon, checking js files. And api ep too,3. Using known vulns to chain with another bug, Few templates created for nuclei, Function check + exploit.,4. Burp: Playing with req***

<br>

- How do you approach multiple JavaScript endpoints? (Tools, Flow, methods)?
 
   - `https://web.archive.org/cdx/search/cdx?url=*.target.com/*&output=text&fl=original&collapse=urlkey`
          
    - ***Multiple tools you can use,In my study OTX, GAU, wayback and gron for sorting helped me alot. Another part I am really weak at xss***

<br>

- When approaching a Target, what are first things that come into your Mind that you should hunt for? 
Also, How to not get distracted from other things? (This might be a relative term, but still What points you might consider in General? ) 
Much love
 
   - ***Recon is common but view is different. Analysis of js files for information, fuzzing, default urls, understand function etc. If you are very passionate about your target then there is no thing to distract***

<br>

- I am on my way to build a fully automated scanner for recon. Common things like finding subdomains, extracting JavaScript, searching for secrets, cvescan, directory  bruteforce, etc already done. What else I can add for better results.
 
  - ***Add grabbing all possible parameters , screenshots, redirection payloads, sub domain alert, valid sorting of subs***

<br>

- What about android bug bounty setup & how you approach . 
What you think about 
@mobexler system or you use other type of setup.
Any word list you use for manually  search ( or tool for automation) in source code for juice stuff.
  
   - ***I just started android bb so not good into that . For wordlist I will say all.txt of jason and here https://github.com/random-robbie/bruteforce-lists 
 I am using all open source stuff***

<br>

# Tips for SSRF 🛡️

- Bro ssrf is possible via Email address ?? like email@burp.collaborator.net if yes provide me detials plz
 
   - ***No. You’ll receive smtp conversation which is no useful. I’ll suggest learn about whitelist-based input filter ssrf
  If you are going via boxes then you need to craft payload for ssrf in that.
  [portswigger](https://portswigger.net/web-security/ssrf/lab-ssrf-with-whitelist-filter)***

<br>

# Admire person 🦸‍♂️

- Whom did you admire when you were at the learning stage? How long did it take to be where you are now? And mention one of your favourite books if you have ever read! Thanks!

    - ***My teacher who introduced me to new stuff of computing. Its been basic 5 years where I am. There is nothing like favourite book but all slides of blackhat***

<br>

# Note Taking 📒

- What is your favorite note-taking app?
 
  - ***Pen and paper*** 


