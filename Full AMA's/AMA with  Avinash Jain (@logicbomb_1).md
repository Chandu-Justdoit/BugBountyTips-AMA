---
layout: post
title:  "Infosec/Bugbounty  AMA with Avinash Jain"
categories: infosec-bugbounty-ama
---


# AMA with [Avinash Jain](https://twitter.com/logicbomb_1)

# About Avinash Jain 😎 and His success 💪

<br>

- What's ur methodology of  selecting the targets for bug hunting ? 
  
  - ***To start with, go for new programs. To practice harder, go for medium scaled programs. Once I develop enough confidence and learning, I go about bigger companies.***

<br>

- What is your methodology in findings  a bugs..?
  
    - ***I always start with creating a layout of the application, breaking it down in subparts, writing the technologies involved in it***

<br>

- When will u decide to change to another target if u didn't find anything in the target ?

    - ***When I fell short of all the ideas, thinking to understand how app is behaving.***
    
<br>
    
- what bug you find most and how and tools you used..?
  
    - ***Mostly my focus is on logical bugs, breaking the logic behind the code. Though it doesn't require any tool, I always have my burp suite open.***

<br>

- How do you map the application and when do you feel that "Yeah! I need to start from here"?
  
    - ***I break the application into subparts and start it when I feel I understood the working of the application clearly***

<br>

- What was your best bug?
  
    - ***My first Bug [Medium](https://medium.com/@logicbomb_1/the-journey-of-web-cache-firewall-bypass-to-ssrf-to-aws-credentials-compromise-b250fb40af82)***

<br>

- what type of bug do you hunt for?
    
    - ***Mostly logical bugs***

<br>

- What the most function/part you focus on when testing web application ?

    - ***Section which seems to interact with critical services and features.***

<br>

- And how's your prespetcive while you're searching for Bussiness logic bugs ??

    - ***Understanding the web app to the depth, technologies, and framework being involved and then I go about thinking what particular logic is behind the particular functionality.***

<br>

- how many days it took for u to find your 1st bug
   
   - ***It took me a week or so to find a good bug.*** 

<br>
   
 # Tips for Beginners 🔰
 
- How worthy is it to learn bug bounties nowadays? As you know there are tons of experienced researchers whom are actively testing all programs. If it is still worthy then what should be the strategy to become a successful bug bounty hunter?
  
    - ***See nowadays there is "healthy" competition in bug bounty hunting and at every moment you have to think out of the box having your basics clear at the very first step.
   Start with clearing your basic, learn the fundamentals, understand how an application is built, code it by yourself, develop confidence within you, and then go after it.***

<br>

- What is your methodology in findings  a bugs..?
  
    - ***I always start with creating a layout of the application, breaking it down in subparts, writing the technologies involved in it.***

<br>

- Who can be a good bug bounty hunter? What kind of experience do I need?
 
    - ***1) The one who knows how an application works, the one who doesn't go for "what" but go for "why".2) Practice and practice harder is the only experience initially.***

<br>

 - How do you map the application and when do you feel that "Yeah! I need to start from here"?
  
     - ***I break the application into subparts and start it when I feel I understood the working of the application clearly***

<br>

- What advice you would give to your younger self who is starting  bug bounty?
  
   - ***Code more, develop the application from scratch, go for learning not for HOF, and bounty. They will come sooner rather than later***

<br>

- What is that thing you would like to tell your younger self who was learning the basics of Web app security
 
     - ***Code everything. There is no better learning you can get by actually getting your hands dirty into developing something and that's when you would be able to think like a developer, what actual mistake they make.***

<br>

 - And how's your prespetcive while you're searching for Bussiness logic bugs ??

      - ***Understanding the web app to the depth, technologies, and framework being involved and then I go about thinking what particular logic is behind the particular functionality.***

<br>

 - (in your opinion) Is ctf's and labs are important to practice before trying live web applications

      - ***Yes, ctfs and labs help a lot.***

<br>

 - On which type of bugs beginners should concentrate (if any)
   
      - ***Concentrate less on the type of buys but more on the cause of it.***

<br>

 - Do you suggest me learning JavaScript for static analysis. or the better question is, Is it worth learning static analysis of JavaScript for DOM based vulns and for better understanding of webapps? or there are tools that can find all vulns in JS and my time will go to waste?
  
      - ***Yes, there is a clear benefit of learning JS especially when it comes to hacking. Still, most of the controls are at the client end, you need specific skills to understand and bypass them and that's when your Javascript expertise comes into the picture. Tools -Retirejs,NodeJsScan***

<br>

# Tips for INFORMATION DISCLOSURE ℹ

- Any specific mindset for finding SSRF and Information disclosure ?
 
   - ***1) Understand how the input parameter is getting processed at the backend or how they could be. 
        2) Look out for APIs which seems to provide some sensitive data, check for misconfigs, idors, etc.***
<br>

# Tips For IDOR'S 🆔

- What is the Best way &tool to find to IDOR?
 
   - ***IDORs are manual bugs. They occur due to a lack of authorization checks. You have to manually find them.***

<br>

# Tips For Business logics 👨‍💼

- Any specific mindset for finding business logics ?
 
    - ***Think from the developer’s mind, break it using a hackers mindset. Understanding the web app to the depth, technologies, and framework being involved. Breaking logic is mostly when you have the practical knowledge of the implementation.***

<br>

- And how's your prespetcive while you're searching for Bussiness logic bugs ??
 
    - ***Understanding the web app to the depth, technologies, and framework being involved and then I go about thinking what particular logic is behind the particular functionality.***

<br>

# Tips For LFI 📁

- Any tips for finding SSRF and LFI..?
  
  - ***See you will find a dozen of tips on ssrf, lfi, rce, etc but what approach you should follow is to understand how your input is being processed in the backend? Is it interacting with any file system, cloud service, etc ?***

<br>

# Tips For SSRF 🛡️


- How to chain idor to SSRF.
  
  - ***Not anything I can think on this line. These are 2 separate lines***

<br>

- Any tips for finding SSRF and LFI..?
  
  - ***See you will find a dozen of tips on ssrf, lfi, rce, etc but what approach you should follow is to understand how your input is being processed in the backend? Is it interacting with any file system, cloud service, etc ?***

<br>

- Any specific mindset for finding SSRF and Information disclosure ?
   
   - ***1) Understand how the input parameter is getting processed at the backend or how they could be. 
       2) Look out for APIs which seems to provide some sensitive data, check for misconfigs, idors, etc.***

<br>

- Any Tips for SSRF RCE &SQLi
   
   - ***Understand how the input parameter is getting processed at the backend or how they could be.***
   
<br>
   
# Advice's 👍

- bug bounty as a career in 2020?

   - ***Bug Bounty is every rising and so the competition. More and more people turning towards this even as their permanent source of income. More and more companies are shifting towards crowd source pentesting. Bug bounty career looks brightful than ever.***
   
<br>

- How worthy is it to learn bug bounties nowadays? As you know there are tons of experienced researchers whom are actively testing all programs. If it is still worthy then what should be the strategy to become a successful bug bounty hunter?
  
   - ***See nowadays there is "healthy" competition in bug bounty hunting and at every moment you have to think out of the box having your basics clear at the very first step.
   Start with clearing your basic, learn the fundamentals, understand how an application is built, code it by yourself, develop confidence within you, and then go after it.***

<br>

- Who can be a good bug bounty hunter? What kind of experience do I need?
 
    - ***1) The one who knows how an application works, the one who doesn't go for "what" but go for "why".
         2) Practice and practice harder is the only experience initially.***
         
<br>

 - why writing on medium it is better to create your own site right ?

     - ***Because medium is a single stop for all the articles and once you have good amount of followers, you can switch to your own site.***

<br>

- any tips how we can get job using our bugbounty hof achivement ,bugbounty platform rank ..because many company asked for certification,exp

    - ***Highlight all such achievements in your resume clearly. Call out them in your introduction during interviews.***

<br>

- How can a fresher get an infosec job in india?Like is it necessary that you should have a certification like ceh or oscp?

   - ***Most companies require certification and some not. In the end, what really matters is how logical you are during interviews, what sort of interesting work/projects you have done in your curriculum.***

<br>

# Note Taking 📒

- How do you keep your notes and progress when hunting, do you trust online services to keep your private notes?
For example, do you trust Dropbox when to save sensitive progress when you hack Dropbox?
  
  - ***I use sublime to keep my notes. There is a limit to which you can avoid online services. Most of the big companies also get hacked that doesn't mean they are not secure but when it comes to my private data, I always try not to use online services.***

<br>

# Burnouts 🔥

- How do you deal with burnouts ?
 
   - ***Follow a healthy work life balance. I have been following it for more than 2 years now and never felt burnout. Keep multiple targets in scope in case you think you are not able to find bug in any of them.***

<br>
