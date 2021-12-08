# Quick Security Reference: Cross-Site Scripting (XSS) 

> [time=Sun, Dec 5, 2021 2:26 PM]
> Microsoft Security Development Lifecycle
> For the latest information: http://www.microsoft.com/sdl.


# Overview
- Cross-site scripting attacks (XSS) 
    - occure whenever an application 
        1. takes **data that originated from a user** 
        2. and **sends it to a WEB browser** 
        3. without properly **validating** or **encoding**
- WEB application security issue
    - XSS allows **script in the victim's browser**
        - hijack user sessions
        - devace Web sites
        - port scan internal networks
        - conduct phishing attacks
        - take over the user's browser using scripting malware
- 

# Understanding XSS for the Buisiness Decision Maker

- In charge of deliverint the development project from start to finish, on time, within budget
- Aware of the fact that security is a customer-perception and cost-management issue
- Needs to understand security issue at a high level to make overall project planning decisions includeing: 
    - budget and justification of time
    - resource investments toward security development

## Risk 

![](https://i.imgur.com/GNnCGyv.png)

- fixing cost
    - takes around 40 man-hour/indicent
    - combined with 
        - hiring or training  an engineer (~$100/hour)
    - 7 XSS vulnarabilityes/WEB site 
        - total estimated cost to $28,000 to fix each problem


## Business Impact
- XSS vulnarabilityes include: 
    - Google Desktop allowe attackers to gain full access to the user's system
    - Over one million MySpace accounts were infected/defaced in the first day of the attack that allows DoS attack.
    - In 2008, as a resulst of XSS, Barack Obama's Web site to redirect visitors to Hillary Clinton's site.

## Fixing the Code
- design phase
    - coding vulnerabilities during the implementation phase
    - fixing the code same person or familier person
- In Verification/QA/Test, check XSS vulnerabilities
    - QA/Test team shoulc be the most effective team at uncoering XSS vulnerabilities


## Resources and Traning for Business Decision Makers
- [19 Deadly Sins of Software Security: Programming Flaws and How to Fix Them](https://www.amazon.com/Deadly-Sins-Software-Security-Programming/dp/0072260858/ref=sr_1_1?ie=UTF8&amp&s=books&amp&qid=1256159028&amp&sr=8-1)


# Understanding XSS for the Architect
- In charge of the technical design of the development project
- cares about security from an overall integrity standpoint
- Understands security concepts in enough detailto aboid crating a bulueprint that whould result in security issues
- Respoinsible for creating the core principles that developers use to implement the functional goals of the project, managing awareness of security ussies as they relate to the specific solution, and tracking and verifying fixes to potentially costly security mistakes in code leading up to release


## Identifying the Problem
- Reflected XSS (Type-1 XSS)
    - exploit a page reflects attacker-supplied data directly back to the victim
- Stored XSS (Type-2 XSS)
    - web application accepts hostile data, stores it in a file , database, or other backend-system, and then at a later stage displays the unfilterd date to the victim
- Local XSS (Type-0 XSS/Document Object Model-based XSS)
    - attacks client side JavaScript code and variables

Alternatively, attacks can be a blend or gybrid of all three types


|

## Designing a Fix
### Input Validation Rules
### Output Encoding Rules
## Future Design Considerations
## Tools for Desining Software That Prevents XSS
## REsources and Traning for Arhitects/PMs

# Understanding XSS for the Developer
## Identifying XSS Exploits
### Identifying Untrusted Input
### Identifying Untrusted output
### Stealing Cookies and User Information
## Witing SEcure Code
### VAlidating Untrusted Input
### An Alternative Approach: Sanitize Untrusted INput
### Validating Trusted Output
### Protecting Cooki9es and User Information from XSS
### Use Validate Request
### Tools and libraries
## REsources and Traning for Developers

# Understanding XSS for the Tester/QA
## Identifying INsecure Code
### Map Out the Site and Its Functionality
### Identify and List Out Every Point of User-Suppolied Input
### Start Testing and Pay Attenstion to the Output
## VEryfying Security Agtainst XSS Attacks
## Modifying Your Test Process for XSS
## Tools You Can Use
## Resourc es and Traning for Testers

# The Microsoft SDL and Preventing XSS
## Long-Term Solutions

# Conclusion


