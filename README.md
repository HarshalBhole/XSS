# XSS

Objective was to find the password of given user in different work environment with different security level and affect the multiple user profiles on elgg site

We Performed XSS attack on elgg website using JavaScript to affect multiple user profiles. Learned the impact of XSS like user accounts can be hijacked, credentials could be stolen, sensitive data could be exfiltrated, and lastly, access to your client computers can be obtained.
![image](https://user-images.githubusercontent.com/81542403/180305967-d2911eab-e054-4b5f-aeed-b246a5349a31.png)
So we Created the script in java to perform brute force attack on password files on Windows and Linux. Gained password of user which can give access to root admin and backdoor to system after further exploitation.



Overview
Cross-site scripting (XSS) is a type of vulnerability commonly found in web applications. This vulnerability
makes it possible for attackers to inject malicious code (e.g. JavaScript programs) into victim’s web browser.
Using this malicious code, attackers can steal a victim’s credentials, such as session cookies. The access
control policies (i.e., the same origin policy) employed by browsers to protect those credentials can be
bypassed by exploiting XSS vulnerabilities. Vulnerabilities of this kind can potentially lead to large-scale
attacks.
To demonstrate what attackers can do by exploiting XSS vulnerabilities, we have set up a web application named Elgg in our pre-built Ubuntu VM image. Elgg is a very popular open-source web application
for social network, and it has implemented a number of countermeasures to remedy the XSS threat. To
demonstrate how XSS attacks work, we have commented out these countermeasures in Elgg in our installation, intentionally making Elgg vulnerable to XSS attacks. Without the countermeasures, users can post any
arbitrary message, including JavaScript programs, to the user profiles. In this lab, students need to exploit
this vulnerability to launch an XSS attack on the modified Elgg, in a way that is similar to what Samy
Kamkar did to MySpace in 2005 through the notorious Samy worm. The ultimate goal of this attack is to
spread an XSS worm among the users, such that whoever views an infected user profile will be infected,
and whoever is infected will add you (i.e., the attacker) to his/her friend list. This lab covers the following
topics:
• Cross-Site Scripting attack
• XSS worm and self-propagation
• Session cookies
• HTTP GET and POST requests
• JavaScript and Ajax
