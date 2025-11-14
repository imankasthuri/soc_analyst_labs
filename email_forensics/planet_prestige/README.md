# Planet Prestige

- This is my first cybersecurity lab, where I learned how to analyze a suspicious email. I opened a raw email file, checked the headers, and found signs of spoofing. This lab helped me understand the basics of phishing analysis and how a SOC analyst investigates suspicious messages.

## What I did

- First I opened the raw email file with notepad ++ and quickly identified the spoofed sender information and the other suspicious content.

**Received: from localhost (emkei.cz. [93.99.104.210])**

- I found out that localhost means this is not a real, legitimate email server; attackers often use localhost when sending fake emails.
- And attacker used emkei.cz. fake email generator to generate the email.

 **spf=fail** 

 - This means sending server not authorized to send emails for the domain it claimed by using, so the sender identity is fake.

##Content-Transfer-Encoding: base64##

- Another sighn of suspicious behaviour is the presense of base64 encoded content.
  


