---
id: edit-3
title: Top 3 Threats of 2024 and How To Protect Against Them
description: Cyber security threats never stop. A technology gets created, a vulnerability is discovered within it, the vuln gets patched, only for a new vuln to be found – rinse, repeat.
author: Ross Moore
date: 2024-03-15T11:13:24.000Z
---

# Top 3 Threats of 2024 and How To Protect Against Them

Written by Ross Moore
Mar 15, 2024 • 16 min read

---

![This AI-generated image was created on Midjourney](../content/images/2024/03/cafeperc_3-headed_cybersecurity_monster_in_a_forest_mountains_562c7e07-2205-4f8d-bc1d-4f7636249ccc_2.png)

*This AI-generated image was created on Midjourney*

Cyber security threats never stop. A technology gets created, a vulnerability is discovered within it, the vuln gets patched, only for a new vuln to be found – rinse, repeat.

Based on numerous reports of the top threats in recent years and expected in 2024 (*see “Resources” at the end of this article*), I've decided to go with these 3 top threats:

1. Ransomware
2. Social Engineering
3. Misconfigurations

An important note: when these are successfully exploited, it doesn't automatically follow that the company or person that fell victim is the one to blame. So, we don't want to automatically blame victims for laziness, lack of aptitude and vigilance - media being what it is, we readers of the news only get a small part of the story. Often, the media won't actually be able to pass along more valid information until many days after the initial notice. It's too common for news followers to jump to conclusions based on headlines and limited information that only serve to spread fear fearful and anxiety. Many people want to be the expert on the newest cybercrime when in fact there is limited information available to the public. 

 Keep in mind how your industry could be attacked - every industry, every company has its own risks and threats (beyond just the security category). Many companies, while not necessarily targeted, will get caught up in threat campaigns, much like collateral damage. 

Overviews like this always come with, not so much the need for taking it with a grain of salt, but with the need for discernment. These are definitely threats to every organization - even every household, person, and device - but the degree to which one really needs to be on high alert to each threat is up to each person in charge of keeping things secure (this counts even for those in their home who are responsible for keeping their family safe).

For each topic, I've provided the following points:

- What it is
- Examples
- How it's perpetrated
- How to test
- How to fix

“How to test” is perhaps the toughest and trickiest to write about and as such is probably our of scope of this article. 

When I read things that say, "here's all the gory detail of how it's done" and they end with "turn on 2fa and good luck!" - it just seems to fall short of actionable steps. Don't get me wrong - it's good advice, and 2FA is a wonderful addition to login credentials but for orgs looking to up their security posture X%, I hope the steos outlined below will help. Proceed at your own risk, get permission as needed.

# Ransomware

## What it is

Ransomware is a type of malware designed to block access to a computer system or files until a sum of money is paid, making those systems and files inaccessible by encrypting them. Once the files are encrypted or locked, the ransomware displays a message demanding payment, often in cryptocurrency in exchange for a decryption key or other means to regain access.

## Examples

Lately, Lockbit and Blackcat/ALPHV have been snatching the headlines so we’ll start with them as our first examples. 

Lockbit is considered by some to be among the top 3 big ransomware groups, the othera being Cl0p and Blackcat. Cl0p was disrupted in 2021 (<a href="">https://www.darkreading.com/cyberattacks-data-breaches/ukraine-police-disrupt-cl0p-ransomware-operation</a>), Blackcat was disrupted in 2023, leaving Lockbit to rise to the top (even though they’ve been around for a long time in different variations, making them one of the most pernicious ransomware-as-a-service (RaaS) groups).

Lockbit’s infrastructure was taken down a few weeks ago by an international law enforcement collaboration but came back online soon after. It’s anyone’s guess what they’ll end up doing. An odd lesson from Lockbit: update your PHP versions, because outdated PHP was the vulnerability used by law enforcement to gain a foothold within Lockbit’s infrastructure. <a href="https://therecord.media/lockbit-relaunch-attempt-follwing-takedown?ref=secjuice.com">https://therecord.media/lockbit-relaunch-attempt-follwing-takedown</a>

Blackcat/ALPHV (you’ll see these 2 as an aka or even used interchangeably) successfully attacked Change Healthcare with a hefty ransom demand to the tune of $22 million. It’s possible that the payment was made by Change, but in a recent and not-so-ironic turn of events, a classic case of no honor among thieves, the criminal affiliate who had the decryption key (remember: RaaS is a business model with affiliates, clients, customers, salespeople, incentives, etc) never received their part of the ransom payment, leaving Blackcat with no access to the data. Therefore Change still has data encrypted, Blackcat doesn’t have the key, and the affiliate doesn’t have their money.

More news here: <a href="https://krebsonsecurity.com/2024/03/blackcat-ransomware-group-implodes-after-apparent-22m-ransom-payment-by-change-healthcare/?ref=secjuice.com">https://krebsonsecurity.com/2024/03/blackcat-ransomware-group-implodes-after-apparent-22m-ransom-payment-by-change-healthcare/</a>

## How It’s perpetrated

Very often, someone clicked on something they shouldn't have.

But that's not the only case. A famous instance is SamSam ransomware and other perimeter attacks: <a href="https://cybersecurity.att.com/blogs/security-essentials/ransomware-attacks-on-the-perimeter?ref=secjuice.com">https://cybersecurity.att.com/blogs/security-essentials/ransomware-attacks-on-the-perimeter</a>

Because of the myriad ways that ransomware can be used, the MITR ATT&amp;CK framework is a great way to map out the relevant attack vectors and get an overview of how ransomware can be leveraged against your organization. <a href="https://www.cyberark.com/resources/blog/how-to-use-the-mitre-att-ck-framework-to-fight-ransomware-attacks?ref=secjuice.com">https://www.cyberark.com/resources/blog/how-to-use-the-mitre-att-ck-framework-to-fight-ransomware-attacks</a>

## How to test

One never wants to test using real ransomware, but there are ways to simulate or emulate an attack that don’t destroy data or drain the budget.

One option is KnowBe4’s free ransomware simulator "RanSim,” which they describe on their site: “RanSim will simulate 24 ransomware infection scenarios and 1 cryptomining infection scenario and show you if a workstation is vulnerable.” <a href="https://www.knowbe4.com/ransomware-simulator?ref=secjuice.com">https://www.knowbe4.com/ransomware-simulator</a>

Another option is Infection Monkey, buy Akamai Guardicore, and is found here: <a href="https://github.com/guardicore/monkey?ref=secjuice.com">https://github.com/guardicore/monkey</a> with documentation here: <a href="https://techdocs.akamai.com/infection-monkey/docs/welcome-infection-monkey?ref=secjuice.com">https://techdocs.akamai.com/infection-monkey/docs/welcome-infection-monkey</a>

Per their site, “The Infection Monkey is an open-source breach and attack simulation tool for testing a data center's resiliency to perimeter breaches and internal server infection. Infection Monkey will help you validate existing security solutions and will provide a view of the internal network from an attacker's perspective.”

A third option is AttackIQ Flex, here: <a href="https://www.attackiq.com/products/flex/?ref=secjuice.com">https://www.attackiq.com/products/flex/</a> “Safe, real-world attack scenarios are at the click of a button. Designed for anyone to run with actionable guidance to keep you protected.”

The account is free, and there are a few modules you can run on machines to get a report. 

Need your own environment to test, emulate, and simulate? The MAD GitHub repo and CITD repo have great sources for creating a mini VM environment for threat emulation·       

<a href="https://github.com/maddev-engenuity/AdversaryEmulation?ref=secjuice.com">https://github.com/maddev-engenuity/AdversaryEmulation</a>

<a href="https://github.com/center-for-threat-informed-defense/adversary_emulation_library/tree/master?ref=secjuice.com">https://github.com/center-for-threat-informed-defense/adversary_emulation_library/tree/master</a>

Two more options to take are ATOMIC Red Team and MITRE Caldera at <a href="https://github.com/redcanaryco/atomic-red-team?ref=secjuice.com">https://github.com/redcanaryco/atomic-red-team</a> and <a href="https://github.com/mitre/caldera?ref=secjuice.com">https://github.com/mitre/caldera</a> respectively.

## How to fix it

To protect your org from ransomware, here are 10 recommended practices based on expert advice:

1. Backup Your Data: Regularly back up your data to an external hard drive or cloud server following the 3-2-1 rule - keep 3 separate copies of data on 2 different storage types with 1 copy offline.

2. Keep All Systems and Software Updated: Ensure your OS, browsers, antimalware, and other software are always updated to the latest versions to prevent vulnerabilities that ransomware can exploit.

3. Install Antimalware &amp; Firewalls: Use comprehensive antivirus and anti-malware software along with firewalls to defend against ransomware attacks.

4. Security Awareness Training: Provide security awareness training to employees on safe web surfing, strong password creation, recognition of suspicious emails, and maintaining updated systems and software.

5. Set Up Strong Spam Filters: Implement strong spam filters in email and messaging services to reduce the risk of phishing attacks that can introduce malware into your system.

6. Understand Ancillary Threats: Be aware that ransomware is often linked to other cyberattacks, so use centrally managed antivirus solutions and provide training on various threats like phishing and malware.

7. Set Up Application Whitelisting: Utilize application whitelisting to only allow trusted files, applications, and processes to run, preventing unauthorized software from executing.

8. Use a Zero Trust Approach: Implement a zero-trust framework that assumes no device or user is authorized by default, requiring proof of authorization like multifactor authentication for access control.

9. Implement Multifactor Authentication (MFA): Enforce MFA for critical systems to make it harder for cybercriminals to gain unauthorized access, reducing the risk of ransomware attacks.

10. Regularly Back Up Data Off-Site: Back up data regularly off-site and test the recovery process to ensure quick restoration in case of a ransomware attack.

There’s no single source of truth for “best practices,” so ensure you consider all the relevant attack vectors for your org.

# Social Engineering

Bruce Schneier said, “Amateurs hack systems, professionals hack people.” Social engineering is used to manipulate individuals into divulging confidential information, performing actions, or providing access to systems or resources that they would not normally provide.

According to Carnegie Mellon University, “social engineering is the tactic of manipulating, influencing, or deceiving a victim in order to gain control over a computer system, or to steal personal and financial information. It uses psychological manipulation to trick users into making security mistakes or giving away sensitive information.”

## Examples

A recent famous example was the MGM hotels compromise, described here: “Scattered Spider used social engineering to trick MGM help desk employees into resetting the passwords and multi-factor authentication (MFA) codes of high-value MGM employees.” (<a href="https://thrivedx.com/resources/article/investigating-the-mgm-cyberattack-how-social-engineering-and-a-help-desk-put-the-whole-strip-at-risk?ref=secjuice.com">https://thrivedx.com/resources/article/investigating-the-mgm-cyberattack-how-social-engineering-and-a-help-desk-put-the-whole-strip-at-risk</a>)

In 2023, imposter scams were quite popular (<a href="https://www.cnbc.com/2024/02/15/imposter-scams-are-top-fraud-of-2023-ftc-says-how-to-protect-yourself.html?ref=secjuice.com">https://www.cnbc.com/2024/02/15/imposter-scams-are-top-fraud-of-2023-ftc-says-how-to-protect-yourself.html</a>). Obviously a powerful variation that can cover many of the categories above, in an imposter scam, “Criminals pretend to be someone you trust to persuade you to send them money, or to get information that can later be leveraged for money.”

<a>$100 Million Google and Facebook Spear Phishing Scam:</a> Perpetrated by a Lithuanian national, Evaldas Rimasauskas, who set up a fake company and sent phishing emails to specific Google and Facebook employees, cheating the two tech giants out of over $100 million. <a href="https://www.justice.gov/usao-sdny/pr/lithuanian-man-pleads-guilty-wire-fraud-theft-over-100-million-fraudulent-business?ref=secjuice.com">https://www.justice.gov/usao-sdny/pr/lithuanian-man-pleads-guilty-wire-fraud-theft-over-100-million-fraudulent-business</a>

## How It’s perpetrated

Phishing is perhaps the most prevalent method of social engineering (SE), but there are plenty of other ways. A few broad categories of SE are hi-tech, lo-tech, and influence based. Several examples of these types are as follows:

- Hi-tech
  - Phishing
  - Spear Phishing
  - Vishing
  - Baiting
  - Rogue Wi-Fi AP
- Lo-tech
  - Intrusion
  - Impersonation/Identity Theft
    - Two examples are badge copying and AI voice.

*  A recent example of AI video and voice was the $25 million deepfake of a CFO. More details here: <a href="https://www.cnn.com/2024/02/04/asia/deepfake-cfo-scam-hong-kong-intl-hnk/index.html?ref=secjuice.com">https://www.cnn.com/2024/02/04/asia/deepfake-cfo-scam-hong-kong-intl-hnk/index.html</a>

  - Tailgating/Piggybacking
  - Shoulder Surfing
  - Dumpster Diving
- Influence
  - Scarcity
  - Authority
  - Liking
  - Consistency
  - Social Proof
  - Reciprocation

## How to test it

A famous toolset is SET – Social Engineering Toolset, found here: <a href="https://trustedsec.com/resources/tools/the-social-engineer-toolkit-set?ref=secjuice.com">https://trustedsec.com/resources/tools/the-social-engineer-toolkit-set</a>

The Social Engineering Toolkit (SET) is an open-source Python-based tool designed for penetration testing and ethical hacking purposes. Developed by Dave Kennedy (also known as "ReL1K"), SET automates various social engineering attacks, enabling security professionals to simulate real-world attacks and assess the security posture of their systems.

Key features of the Social Engineering Toolkit include:

- Multiple Attack Vectors: SET offers a wide range of attack vectors, including spear phishing, credential harvesting, website cloning, and more.
- Customization: Users can customize various aspects of the attacks generated by SET, such as email templates, phishing web pages, and payloads. This allows testers to tailor the attacks to specific targets or scenarios.
- Payload Generation: SET includes tools for generating malicious payloads, such as Metasploit payloads, that can be used to exploit vulnerabilities in target systems. These payloads can facilitate remote access, data exfiltration, and other malicious activities.
- Reporting: SET provides functionality for generating detailed reports on the results of social engineering campaigns. These reports can be used to document findings, track progress, and communicate with stakeholders.
- Integration with Metasploit: SET integrates with the Metasploit Framework, a popular penetration testing tool, allowing users to launch coordinated attacks that combine social engineering techniques with traditional exploitation methods.

It's important to use this – and every tool - responsibly and ethically. Using SET for unauthorized or malicious purposes can have serious legal and ethical consequences.

 More guidance on SET is here: <a href="https://www.stationx.net/social-engineer-toolkit/?ref=secjuice.com">https://www.stationx.net/social-engineer-toolkit/</a>

 Some phishing simulators are noted here: <a href="https://resources.infosecinstitute.com/topics/phishing/top-9-free-phishing-simulators/?ref=secjuice.com"><u>https://resources.infosecinstitute.com/topics/phishing/top-9-free-phishing-simulators/</u></a>

## How to fix it

Education, training, i – whatever you want to call it (“training” can seem too clinical, or education can seem too informal, so find what term works for your organization’s culture).

 social engineering can take many forms, often depending on the size of the intended targets– e.g., large orgs can be easy targets for C-Suite fakes because many don’t know the C-Suite; high-stress companies that focus on output and quick turnaround are targets for urgency; companies were there are lots of deliveries are targets for tailgating.

What’s important is that personnel are trained about what to do in XYZ instance – make sure they know what they can or can’t do. Can they deny access? Should they follow a person they suspect? To whom should they report it? Can they take photos of strangers? Are they allowed to interact with suspicious visitors? These are just some of the questions that need to be answered.

# Misconfigurations

A security misconfiguration occurs when system or application configuration settings are missing or implemented improperly, allowing unauthorized access to resources.

<a href="https://csrc.nist.gov/glossary/term/misconfiguration?ref=secjuice.com">NIST defines</a> it as “An incorrect or suboptimal configuration of an information system or system component that may lead to vulnerabilities.”

OWASP very helpfully describes instead of defines it:

“The application might be vulnerable if the application is:

- Missing appropriate security hardening across any part of the application stack or improperly configured permissions on cloud services.
- Unnecessary features are enabled or installed (e.g., unnecessary ports, services, pages, accounts, or privileges).
- Default accounts and their passwords are still enabled and unchanged.
- Error handling reveals stack traces or other overly informative error messages to users.
- For upgraded systems, the latest security features are disabled or not configured securely.
- The security settings in the application servers, application frameworks (e.g., Struts, Spring, ASP.NET), libraries, databases, etc., are not set to secure values.
- The server does not send security headers or directives, or they are not set to secure values.
- The software is out of date or vulnerable (see A06:2021-Vulnerable and Outdated Components).”

## Examples

<u>NASA</u>

In 2019, the personal information of NASA personnel, including their names and email addresses, as well as information about current projects within the space agency, were made public via a misconfigured app, specifically excessive permissions on a web-based tool used to track internal issues and processes.

More information here: <a href="https://www.itpro.com/security/32732/nasa-employee-data-exposed-for-at-least-three-weeks-due-to-misconfigured-web-app?ref=secjuice.com">https://www.itpro.com/security/32732/nasa-employee-data-exposed-for-at-least-three-weeks-due-to-misconfigured-web-app</a>

Lockbit

There’s not a lot of information, but misconfigurations can be leveraged against threat actors. In February 2024, the US FBI and UK NCA were able to compromise Lockbit’s server by using a known PHP vulnerability that hadn’t been patched. More info here: <a href="https://krebsonsecurity.com/2024/02/feds-seize-lockbit-ransomware-websites-offer-decryption-tools-troll-affiliates/?ref=secjuice.com">https://krebsonsecurity.com/2024/02/feds-seize-lockbit-ransomware-websites-offer-decryption-tools-troll-affiliates/</a> and here: <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-3824?ref=secjuice.com">https://nvd.nist.gov/vuln/detail/CVE-2023-3824</a>

## How It’s perpetrated

Criminals often take advantage of misconfigurations in various ways to steal data. Misconfigurations can occur at different levels of an organization's infrastructure, including network, server, application, and cloud services. Here are some common scenarios:

1. Unsecured Databases: Misconfigured database servers may have default or weak credentials, lack encryption, or improperly configured access controls. Attackers can exploit these misconfigurations to gain unauthorized access to sensitive data stored in databases, such as customer information, financial records, or intellectual property.

2. Exposed Services: Misconfigured network devices or servers may have unnecessary services or ports open to the internet, providing attackers with potential entry points into the network. Attackers can scan for such exposed services and exploit vulnerabilities to gain access to systems and steal data.

3. Weak Authentication: Misconfigured authentication mechanisms, such as weak passwords, lack of multi-factor authentication, or improper user permissions, can make it easier for attackers to compromise user accounts and access sensitive data or resources.

4. Insecure APIs: Misconfigured APIs (Application Programming Interfaces) may lack proper authentication, authorization, or encryption mechanisms, making them susceptible to exploitation. Attackers can abuse insecure APIs to access or manipulate data stored in cloud services, web applications, or other online platforms.

5. Cloud Misconfigurations: Misconfigured cloud services, such as storage buckets or server instances, may have overly permissive access controls or inadequate security configurations. Attackers can exploit these misconfigurations to access sensitive data stored in the cloud environment, such as customer records, proprietary information, or credentials.

6. Unpatched Systems: Failure to apply security patches or updates to software and operating systems can leave systems vulnerable to known exploits. Attackers can exploit these vulnerabilities to gain unauthorized access to systems and exfiltrate data.

Criminals exploit misconfigurations to steal data by taking advantage of vulnerabilities in security settings that are not correctly defined or deployed with insecure default settings. These misconfigurations can lead to major data breaches, financial losses, and exposure of sensitive information. For instance, a former Amazon engineer exploited Capital One's misconfigured firewall to steal over 100 million customer records by gaining unauthorized access to backend resources due to configuration errors.

## How to test it

Because there are so many ways to misconfigure something, and because that “something” could be physical, hardware, software, or who knows what, there’s no ABC123 generic list to present. But principled guidance is possible.

bWapp (<a href="http://itsecgames.com/?ref=secjuice.com">http://itsecgames.com/</a>) and WebGoat (<a href="https://owasp.org/www-project-webgoat/?ref=secjuice.com">https://owasp.org/www-project-webgoat/</a>) are traditional downloadable vulnerable apps to learn about testing for misconfigs.

Portswigger’s Web Academy has great and free training for learning about and testing numerous misconfigurations: <a href="https://portswigger.net/web-security?ref=secjuice.com">https://portswigger.net/web-security</a>

APISecUniversity has a great list of vulnerable APIs for testing the ever-increasing API world: <a href="https://www.apisecuniversity.com/api-tools-and-resources?ref=secjuice.com">https://www.apisecuniversity.com/api-tools-and-resources</a>  

And OWASP’s Top Ten lists have example attacks that can provide some direction in your testing: <a href="https://owasp.org/Top10/?ref=secjuice.com">https://owasp.org/Top10/</a>

## How to fix it

Fixing or avoiding security misconfigurations requires a combination of proactive measures and reactive responses.

1. The OWASP Top 10 is a great place to start for AppSec issues.

2. For many other misconfigurations, the CIS Controls (<a href="https://www.cisecurity.org/controls?ref=secjuice.com">https://www.cisecurity.org/controls</a>) are a great reference.

a. A CAUTION for OWASP and CIS (and any other controls): “It looks good on paper” applies here. Fixing a misconfiguration could easily cause immediate and/or cascading troubles. Proceed with caution! Determine what the repercussions could be, and see if your org either needs to accept the risk as-is, is ready to deal with trouble, can implement compensating controls, or just needs to work toward sunsetting the product while creating the new one.

3. Appropriate authentication and authorization policies

a. This includes following the least privilege model.

4. Stay Informed: Keep yourself updated with the latest security best practices, vulnerabilities, and patches related to the technologies and platforms you use.

5. Implement Security Policies: Enforce relevant  and reasonable security policies within your organization. These policies should cover aspects such as access control, password management, data encryption, network security.

6. Regular Audits and Assessments: Conduct regular security audits (e.g., vulnerability scanning, penetration testing, code review) and assessments to identify and address misconfigurations.

7. Follow the Principle of Least Privilege: Limit user and system privileges to only what is necessary for their roles or functions.

8. Secure Configuration Management: Ensure that all software, applications, devices, and systems are configured securely according to industry best practices. This includes disabling unnecessary services, changing default passwords, and applying security patches and updates promptly.

9. Automate Configuration: Use automation tools and scripts to configure systems consistently and securely. Automation helps reduce human error and ensures that configurations are applied uniformly across your infrastructure.

10. Implement Secure Development Practices: Follow secure coding practices when developing or customizing software. This includes input validation, output encoding, secure error handling, and other techniques to prevent common vulnerabilities such as injection attacks, XSS, CSRF, etc.

11. Monitor and Log: As much as possible, monitor all the things for signs of suspicious behavior.

12. Security Awareness and Best Practices Training: Educate employees or users about security best practices, common threats, and the importance of adhering to security policies. Role-appropriate education helps reduce the likelihood of human error leading to misconfigurations.

13. Third-Party Risk Management: Assess and monitor the security posture of third-party vendors, service providers, and contractors who have access to your systems or data. Ensure they adhere to the same security standards as your organization.

# Staying ahead of the threats

It’s not easy - staying ahead of the game, keeping aware of emerging threats, maintaining infrastructure, educating the org about relevant threats and mitigations, managing all the things. When one stops to think about it, one probably wants to quit. But with a roadmap, project management, and taking the next step  - these work together to keep things sane and moving in the right direction.

Best wishes!

# Resources and Sources for further reading and information

## General

### Reports

2023 DBIR - https://www.verizon.com/business/resources/reports/dbir/
Sophos report - <a href="https://www.sophos.com/en-us/content/security-threat-report?ref=secjuice.com">https://www.sophos.com/en-us/content/security-threat-report</a>

ZeroFox report<u> - </u><a href="https://www.zerofox.com/2024-predictions/?ref=secjuice.com">https://www.zerofox.com/2024-predictions/</a>

IBM XForce - <a href="https://www.ibm.com/reports/threat-intelligence?ref=secjuice.com">https://www.ibm.com/reports/threat-intelligence</a>

Crowdstrike – <a href="https://www.crowdstrike.com/global-threat-report/?ref=secjuice.com">https://www.crowdstrike.com/global-threat-report/</a>

Spycloud Ransomware Report<u> </u><a href="https://engage.spycloud.com/rs/713-WIP-737/images/spycloud-report-2023-ransomware-defense-report.pdf?ref=secjuice.com">https://engage.spycloud.com/rs/713-WIP-737/images/spycloud-report-2023-ransomware-defense-report.pdf</a>

Mimecast 2023 State of Email Security Report: <a href="https://www.mimecast.com/state-of-email-security/?ref=secjuice.com">https://www.mimecast.com/state-of-email-security/</a>

<a href="https://healthcyber.mitre.org/?ref=secjuice.com"></a>

<a href="https://www.forbes.com/advisor/personal-finance/cybersecurity-threats-for-2023/?ref=secjuice.com">https://www.forbes.com/advisor/personal-finance/cybersecurity-threats-for-2023/</a>

<a href="https://blog.qualys.com/vulnerabilities-threat-research/2023/12/19/2023-threat-landscape-year-in-review-part-one?ref=secjuice.com">https://blog.qualys.com/vulnerabilities-threat-research/2023/12/19/2023-threat-landscape-year-in-review-part-one</a>

h<a href="https://www.gartner.com/en/newsroom/press-releases/04-12-2023-gartner-identifies-the-top-cybersecurity-trends-for-2023?ref=secjuice.com">ttps://www.gartner.com/en/newsroom/press-releases/04-12-2023-gartner-identifies-the-top-cybersecurity-trends-for-2023</a>

<a href="https://www.cobalt.io/blog/cybersecurity-statistics-2024?ref=secjuice.com">https://www.cobalt.io/blog/cybersecurity-statistics-2024</a>

## Ransomware

<a href="https://delinea.com/hubfs/Delinea/whitepapers/delinea-whitepaper-state-of-ransomware-2024-report.pdf?ref=secjuice.com">https://delinea.com/hubfs/Delinea/whitepapers/delinea-whitepaper-state-of-ransomware-2024-report.pdf</a>

<a href="https://www.securityweek.com/the-ransomware-threat-in-2024-is-growing-report/?ref=secjuice.com">https://www.securityweek.com/the-ransomware-threat-in-2024-is-growing-report/</a>

<a href="https://www.crowdstrike.com/cybersecurity-101/ransomware/history-of-ransomware/?ref=secjuice.com">https://www.crowdstrike.com/cybersecurity-101/ransomware/history-of-ransomware/</a>

<a href="https://www.darkreading.com/cybersecurity-operations/global-law-enforcement-disrupts-lockbit-ransomware-gang?ref=secjuice.com">https://www.darkreading.com/cybersecurity-operations/global-law-enforcement-disrupts-lockbit-ransomware-gang</a>

<a href="https://www.cisa.gov/stopransomware/services?ref=secjuice.com">https://www.cisa.gov/stopransomware/services</a>

<a href="https://www.helpnetsecurity.com/2023/10/02/free-ransomware-guides-checklists?ref=secjuice.com">https://www.helpnetsecurity.com/2023/10/02/free-ransomware-guides-checklists</a>

<a href="https://gate15.global/the-white-house-memo-to-industry-on-ransomware-take-action-now/?ref=secjuice.com">https://gate15.global/the-white-house-memo-to-industry-on-ransomware-take-action-now/</a>

<a href="https://www.ncsc.gov.uk/whitepaper/ransomware-extortion-and-the-cyber-crime-ecosystem?ref=secjuice.com">https://www.ncsc.gov.uk/whitepaper/ransomware-extortion-and-the-cyber-crime-ecosystem</a>

America's Data Held Hostage: <a href="https://www.hsgac.senate.gov/wp-content/uploads/imo/media/doc/Americas%20Data%20Held%20Hostage.pdf?ref=secjuice.com">https://www.hsgac.senate.gov/wp-content/uploads/imo/media/doc/Americas%20Data%20Held%20Hostage.pdf</a>

<a href="https://www.mitre.org/news-insights/publication/ransomware-getting-started-guide-and-deep-dive-revil?ref=secjuice.com">https://www.mitre.org/news-insights/publication/ransomware-getting-started-guide-and-deep-dive-revil</a>

CSET: <a href="https://www.cisa.gov/news-events/alerts/2021/06/30/cisas-cset-tool-sets-sights-ransomware-threat?ref=secjuice.com">https://www.cisa.gov/news-events/alerts/2021/06/30/cisas-cset-tool-sets-sights-ransomware-threat</a>

CSET GitHub repo: <a href="https://github.com/cisagov/cset/releases/tag/v10.3.0.0?ref=secjuice.com">https://github.com/cisagov/cset/releases/tag/v10.3.0.0</a>

<a href="https://www.crowdstrike.com/cybersecurity-101/ransomware/how-to-prevent-ransomware/?ref=secjuice.com">https://www.crowdstrike.com/cybersecurity-101/ransomware/how-to-prevent-ransomware/</a>

<a href="https://www.crowdstrike.com/cybersecurity-101/ransomware/?ref=secjuice.com">https://www.crowdstrike.com/cybersecurity-101/ransomware/</a>

## Social Engineering

<a href="https://www.securitymetrics.com/blog/social-engineering-training-what-your-employees-should-know?ref=secjuice.com">https://www.securitymetrics.com/blog/social-engineering-training-what-your-employees-should-know</a>

<a href="https://www.tessian.com/blog/examples-of-social-engineering-attacks/?ref=secjuice.com">https://www.tessian.com/blog/examples-of-social-engineering-attacks/</a>

Jenny Radcliffe <a href="https://humanfactorsecurity.co.uk/?ref=secjuice.com" rel="noreferrer">https://humanfactorsecurity.co.uk/</a>

<a href="https://www.copado.com/resources/blog/12-types-of-social-engineering-attacks-to-look-out-for?ref=secjuice.com">https://www.copado.com/resources/blog/12-types-of-social-engineering-attacks-to-look-out-for</a>

<a href="https://www.knowbe4.com/what-is-social-engineering/?ref=secjuice.com">https://www.knowbe4.com/what-is-social-engineering/</a>

## Misconfigurations

<a href="https://www.balbix.com/insights/security-misconfiguration-impact-examples-and-prevention/?ref=secjuice.com">https://www.balbix.com/insights/security-misconfiguration-impact-examples-and-prevention/</a>

<a href="https://brightsec.com/blog/security-misconfiguration/?ref=secjuice.com">https://brightsec.com/blog/security-misconfiguration/</a>

<a href="https://www.cisa.gov/stopransomware/misconfigurations-and-weaknesses-known-be-used-ransomware-campaigns?ref=secjuice.com">https://www.cisa.gov/stopransomware/misconfigurations-and-weaknesses-known-be-used-ransomware-campaigns</a>

<a href="https://owasp.org/Top10/A05_2021-Security_Misconfiguration/?ref=secjuice.com">https://owasp.org/Top10/A05_2021-Security_Misconfiguration/</a>

<a href="https://healthcyber.mitre.org/?ref=secjuice.com">https://healthcyber.mitre.org/</a>

<a href="https://healthcyber.mitre.org/blog/resources/attack-navigator/?ref=secjuice.com">https://healthcyber.mitre.org/blog/resources/attack-navigator/</a>

<a href="https://www.attackiq.com/2023/12/29/response-to-cisa-advisory-aa23-353a/?ref=secjuice.com">https://www.attackiq.com/2023/12/29/response-to-cisa-advisory-aa23-353a/</a>

<a href="https://www.flowmatters.com/blog/the-impact-of-security-misconfiguration-and-how-to-avoid-it/?ref=secjuice.com">https://www.flowmatters.com/blog/the-impact-of-security-misconfiguration-and-how-to-avoid-it/</a>

<a href="https://usa.kaspersky.com/resource-center/threats/data-theft?ref=secjuice.com">https://usa.kaspersky.com/resource-center/threats/data-theft</a>

<a href="https://www.aquasec.com/cloud-native-academy/supply-chain-security/security-misconfigurations/?ref=secjuice.com">https://www.aquasec.com/cloud-native-academy/supply-chain-security/security-misconfigurations/</a>

<a href="https://hbr.org/2024/02/why-data-breaches-spiked-in-2023?ref=secjuice.com">https://hbr.org/2024/02/why-data-breaches-spiked-in-2023</a>

<a href="https://www.darkreading.com/cloud-security/you-re-one-misconfiguration-away-from-a-cloud-based-data-breach?ref=secjuice.com">https://www.darkreading.com/cloud-security/you-re-one-misconfiguration-away-from-a-cloud-based-data-breach</a> <a href="https://owasp.org/Top10/A05_2021-Security_Misconfiguration/?ref=secjuice.com"><u>https://owasp.org/Top10/A05_2021-Security_Misconfiguration/</u></a>

<a href="https://brightsec.com/blog/security-misconfiguration/?ref=secjuice.com">https://brightsec.com/blog/security-misconfiguration/</a>

<a href="https://brightsec.com/blog/misconfiguration-attacks/?ref=secjuice.com">https://brightsec.com/blog/misconfiguration-attacks/</a>

<a href="https://reciprocity.com/blog/security-misconfigurations-how-to-avoid-them/?ref=secjuice.com">https://reciprocity.com/blog/security-misconfigurations-how-to-avoid-them/</a>

## Help Support Our Non-Profit Mission

If you enjoyed this article or found it helpful please consider making a **U.S. tax-deductible** donation, Secjuice is a non-profit and volunteer-based publication powered by donations. We will use your donation to help cover our hosting costs and **keep Secjuice an advertisement and sponsor free zone**.

[Make a tax-deductible donation](https://opencollective.com/secjuice)
