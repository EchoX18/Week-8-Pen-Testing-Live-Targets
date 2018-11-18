
Week 8 Pen-Testing on Live Targets(Websites) 
# Project 8 - Pentesting Live Targets

Time spent: **6** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1:SQLI (BLIND SQLI)
![Alt Text](https://github.com/EchoX18/Week-8-Pen-Testing-Live-Targets/blob/master/SQLI%20BLIND.gif)

The SQLI input makes the database sleep for 5 seconds once the systems generates the user is different.

Vulnerability #2: Session Hijacking
![Alt Text](https://github.com/EchoX18/Week-8-Pen-Testing-Live-Targets/blob/master/Session%20Hijacking.gif)

On one browser a user must login and then retrieve session ID. On another browser a non logined in user will change its session ID to match that of a logged in user. This allows for attacker to be able to use logged in users account/sessionID. Tool used to change session ID was given by CTF Codepath in 5.10

## Green

Vulnerability #1: CROSS SITE SCRIPTING XXS

GIF WALKTHROUGH- ![Alt Text](https://github.com/EchoX18/Week-8-Pen-Testing-Live-Targets/blob/master/XXS.gif)

Vulnerability #2: User Enumeration

GIF WALKTHROUGH-![Alt Text](https://github.com/EchoX18/Week-8-Pen-Testing-Live-Targets/blob/master/User%20Enumeration.gif)

Bounus XXS
GIF WALKTHROUGH-![Alt Text](https://github.com/EchoX18/Week-8-Pen-Testing-Live-Targets/blob/master/extra.gif)
Used this XXS to redirect the site to Youtube.com.

## Red

Vulnerability #1: Insecure Direct Object Reference
(The User ID is vulnerable if ID is to be changed the object in this case the salesman search is changed.ID 10 should not be avalible to the public.)
 GIF WALKTHROUGH- ![Alt Text](https://github.com/EchoX18/Week-8-Pen-Testing-Live-Targets/blob/master/IDOR.gif)
 ![Alt Text](https://github.com/EchoX18/Week-8-Pen-Testing-Live-Targets/blob/master/IDOR%202.gif)

Vulnerability #2:CSRF
 ![Alt Text](https://github.com/EchoX18/Week-8-Pen-Testing-Live-Targets/blob/master/CSRF%202.gif)
 Used html to secertly change out the form when user with admin privilleges loads the page.


## Notes

Only challenge I had was that the site would not refresh fast enough so XXS on green site at times would prevent me from doing more.
