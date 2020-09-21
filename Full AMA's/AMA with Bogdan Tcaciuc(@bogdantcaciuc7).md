# AMA with Bogdan Tcaciuc(@bogdantcaciuc7)

<br>

# About Bogdan Tcaciuc 😎

- What was your first bug and what was your first purchase with the bounty ?
  
  - ***My first bug was a Reflected XSS and the first purchase was a laptop.***

<br>

- How u climbed that mountain 
  And what is its location
 
    - ***location - Romania, Transylvania***

<br>

- What's your fav vulnerability?

   - ***SSRF***

<br>

- Do you collaborate with others ? Any hunters u look up to ? role models ?  People  you wanna give shout out to ? Any good #FF s for beginners to watch ?
  
   - ***I don’t have role models and didn’t collab with anyone.
 There is a lot of guys in this community which provide awesome research and tips. Can’t just shout out few of them.***

<br>

- It seems that you are doing full time bug bounty. What are your take on bugbounty as single source of income? And what advice you will give to the people who want to do full time bugbounty?
 
    - ***I'm gonna say that the most important thing is to figure out if this is the only thing you want to do.
 I'm very passionate about this and learn new things every day. If someones wanna go full time should know that it's not easy if you don't plan to spend a lot of time on it.***

<br>

- How long you have been hacking for?
 Any tips/recommendations for keep improving yourself on daily basis
 
   - ***I started learning web app vulnerabilities at 12 years old, like 8 years ago.
But nothing serious since 2016 when I started bug bounty.***  

<br>

# Tips for Beginners 🔰

- Any suggestion for newbies how to start bug bounty and how to be strong to face Failure and demotivation in the beginning?

   - ***"Read Web Hacking 101 for introduction then practice every vulnerability you learned on VDP programs. Don't go in this field for the money, the most important thing for newbies is to stay focused and keep learning without expecting "huge bounties".***

<br>
  
- What is the present method of studying do you recommend to the beginners ( like sites, people, topics,etc)

  - ***The present method is practice.Practice every little thing you learned on VDP programs.
       Didn't do CTF's but I saw a lot of people who learned that way.***

<br>

- Do you think Bug Bounty will be extinct in a few years?
 
  - ***No way.
  It will be bigger.***

<br>

- There are many factors which you can't deny about my fear. Such as
*Implementation of modern technologies like AI, ML, NL on appsec
*Overcrowd of experienced researchers
*Crowdsourced and AI-powered security platforms like 
@detectify
 will reduce the attack surface a lot

   - ***We can’t talk too much about the future but I believe that it will be vulnerabilities for everyone.There's a risk of being flop if someone is starting now. And the reasons are mentioned above. Even you couldn’t refute my logics. Also you are unable to predict a positive future of it. You guys have already achieved a lot so tension for you, only beginners like us will suffer
  If you think like that you shouldn't do this.
 I put a lot of effort and take a risk doing this and it turned out very good.
 There are a lot of examples of new successful people coming in.
 If you think too much and don't do something you will achieve nothing.
 Good luck!***

<br>

- Your burp suite version , extension and some tricks and tips.  ( Thanks for AMA)
 
   - ***Burp pro. I don’t use extensions. Try to understand the application/site you testing and use it as a normal user.***

<br>

- H1 - RDP - BC
Which one you prefer for beginners 
Thanks 
   
   - ***I only tried hackerone so.. yea***

<br>

# Tips to Approach a Target  🎯

- Things you take into consideration and how you proceed further when you are approaching a completely new target?
 
     - ***I definitely take into consideration the response time.
When I approach a new target I look for easy vulnerabilities, report some and see how the team interacts and if I'm okay with that I go deeper in that application ( javascript files, docs, github, etc)***

<br>

# Tips for SSRF 🛡️


- Some tips for getting my first SSRF?

  - ***Try to find every endpoint on that application that takes an URL or fetch your resource.
        Look everywhere for those endpoints: javascript files, application features, webhooks, etc..
        Also, I had a lot of success with SSRF via PDF 
         Nice resource about this:
         https://docs.google.com/presentation/d/1JdIjHHPsFSgLbaJcHmMkE904jmwPM4xdhEuwhy2ebvo/htmlpresent***
 
 <br> 
 
# Tips for Recon 🔍
 
- If you dont do much recon kindly let us know your methodology ? how do you approach a target ? Any checklists you follow ?

   - ***I'm always checking for logical bugs, going through the application, and thinking of what shouldn't happen and go further testing. I'm not doing a checklist at first, I make a goal.. let's say I want to find Blind XSS. I'm going to find every endpoint which goes on an admin panel***

<br>

- Can you elaborate your recon methodology/tools ?
 
    - ***I don't really do too much recon nowadays.There are too many resources on recon and everybody does this now.The most important thing is to know the application and read the docs. Also collecting interesting endpoints and fuzzing them resulted in some nice idors.***

<br>

# Tools 🛠

- Which are some of the awesome tools you use ?

  - ***I use the well known ones, aquatone & amass & combination between ffuf and dirsearch.***

<br>

- Can you elaborate your recon methodology/tools ?
 
  - ***I don't really do too much recon nowadays.
      There are too many resources on recon and everybody does this now.
 The most important thing is to know the application and read the docs. Also collecting interesting endpoints and fuzzing them resulted in some nice idors.***

