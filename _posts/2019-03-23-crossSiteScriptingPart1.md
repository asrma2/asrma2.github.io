---
title: Cross-Site Scripting - Part 1
tags: [XSS, Javascript, Cyber Attacks]
style: fill
color: primary
description: Everything is vulnerable, even your website. If you use JavaScript as your language for the development, you know it is a client-side scripting language. Now, what does...
---

## Introduction

Everything is vulnerable, even your website. If you use JavaScript as your language for the development, you know it is a client-side scripting language. Now, what does client-side scripting? As the term suggests, all the scripts are run on the client side i.e. via the browser. The script is transferred from web server to the client side and then the client uses a browser to run those scripts directly. Now, this is the power of JavaScript. However, an attacker who wants to do some malicious tasks can easily use this feature. \\
One such attack is Cross-Site Scripting (commonly known as XSS). Uff another technical term. Now, what is this? In this attack, an attacker injects malicious scripts into web applications. It does not attack the website as a whole but its users. The user thinks that he is accessing the website that he wants but actually, he doesn’t know about the scripts that are running at the back. Those scripts can easily extract user’s cookies that can contain some personal information. There are two main types of XSS attacks, Reflected XSS and Stored XSS.

## Reflected XSS

Also known as non-persistent attacks, Reflected XSS is done by loading some malicious scripts off a web application onto the client side. Now suppose a web application is receiving some data through the parameters and then it is displaying them or using them in some other way without any check. Now an attacker can prepare a link that contains his script as a parameter and can send it to the user via mail or some other platform. Now unknowingly, the user will click on that link and while loading the web application, the browser will also load the script that can execute any task, even fetch his cookies and other private data.

## Stored XSS

Also known as, persistent attacks, Stored XSS is done by storing some malicious scripts in a source from where user retrieves the data (mainly database). Now when the user fetches the data from the database, the malicious script is also fetched and it can execute any task, even fetch his cookies and other private data. For example, there is an input field that let you comment in some post. Now if there is no validation in that field, the attacker can input any data such as a malicious script and it will be stored in the database. Now when a user will open that post, all the comments will also be loaded along with the script. Now the attacker will have access to the data that he desires. \\
Apart from the above two main types, Document Object Model (DOM) based XSS attacks also exist. These scripts are used to manipulate and modify DOM in the user’s browser.

