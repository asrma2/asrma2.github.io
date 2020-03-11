---
title: Cross-Site Scripting - Part 2
tags: [XSS, Javascript, Cyber Attacks]
style: fill
color: primary
description: This is second part of the article on Cross-Site Scripting. You can check out the first at...
---

## Introduction

This is second part of the article on Cross-Site Scripting. You can check out the first at [Cross-Site Scripting - Part 1](cross-site-scripting-part1.html)


## Impacts of XSS Vulnerabilities

As already discussed, XSS attacker does not attack the website as a whole but its users. The attacker can act like a victim user, can do all the things that a user can do even access the data that the user has access to. It can also steal private information of the user such as its login credentials etc. It can also inject malicious things into the website. It all depends on the type of website and its functionality.

## Finding XSS Vulnerabilities

It usually takes very much time to find the vulnerabilities if you are doing it manually. You need to analyze all the input fields and check their validations. You need to check every input field that is returned in HTTP responses and trust me it takes a lot of time. So what else can we do? Fortunately, we have software that can find vulnerabilities in our website quickly and reliably like Burp Scanner, etc.

## Preventing XSS Vulnerabilities

Now we know what XSS is, what its types are and how to find them. However, we need to know how to prevent these vulnerabilities. There are few measures that we can take into account to prevent XSS: \\
•	We need to validate the input as strictly as possible. \\
•	There are places where user data is output in HTTP responses. We need to encode this output data so that no one can read it if it is intercepted in between. \\
•	At last, we can use the Content Security Policy (CSP) as the last line of defense to reduce the effect of these vulnerabilities. \\
This wraps up the article about Cross-Site Scripting (XSS). One thing is clear that XSS attacker does not attack the website as a whole but its users. SO many of us would think why to bother when it does not affect our website. However, if your website is not safe for your users, why would they use it. We concern ourselves about how our website is looking and all but, we should give equal attention to the security side of our website.
    

