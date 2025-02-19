---
id: osint-data-breach-research
title: Using Newly Surfaced Data Breaches for OSINT Research
description: Data Breach Search Engines (DBSEs) collect and organize leaked information from data breaches, enabling OSINT investigators to access it.
author: Tom Caliendo
date: 2024-11-25T03:05:38.000Z
---

# Using Newly Surfaced Data Breaches for OSINT Research

Written by Tom Caliendo
Nov 24, 2024 • 5 min read

---

![Using Newly Surfaced Data Breaches for OSINT Research](../content/images/2024/11/turkeys-doing-cirque-du-soleil.png)

*Turkeys performing at a modern circus show. Microsoft Copilot created this image.*

Data breaches are an unfortunate reality for many websites, leading to leaked information often posted on dark web forums or discovered by security researchers. Before this data disappears or is removed, Data Breach Search Engines (DBSEs) gather, verify, and categorize it, making it accessible to people seeking to understand what information may have been compromised. DBSEs like _Have I Been Pwned_ allow OSINT (open-source intelligence) investigators to enter an email address and see if it was used on a breached site, often revealing critical information about the target’s online footprint. These DBSEs serve as an important privacy service, allowing users to know if their information has been exposed and, in some cases, request its removal from these databases.

## **What are Data Breach Search Engines?**

DBSEs provide a way to find out where an email address, phone number, username, or other identifier has been used, giving researchers a clearer sense of a person’s digital presence. If a DBSE search shows that an email was compromised in a LinkedIn breach, for example, an investigator knows the person likely had a LinkedIn account. This information is invaluable for OSINT researchers, as it offers hints about a target’s professional network, social media presence, and even connections to colleagues or alternate emails. Some of the most popular DBSEs include _Have I Been Pwned_ (searchable by email or phone), _IntelX.io_ (email), and _dehashed.com_ (email, username, domain, password, IP). There are also more specific breach-focused tools, such as _haveibeenzucked.com_ for Facebook data and _checkashleymadison.com_ for the Ashley Madison breach. These tools maintain deep web databases, and the information within them can often be accessed only through the website itself. For OSINT investigators, understanding DBSE resources is critical, as each can reveal unique details about where an email address, phone number, or other identifier was registered and whether it has been compromised.

## **Data Breaches Now Available on Data Breach Information Sites**

This month, four major data breaches have appeared on platforms like _Have I Been Pwned_, each offering unique insights into different user communities. Although some breaches occurred years ago, the data is newly available on DBSEs, presenting OSINT researchers with new avenues to explore.

1\. Internet Archive (October 2024)

In October 2024, the Internet Archive, famous for its digital preservation efforts and the Wayback Machine, experienced a breach affecting 31 million user accounts. Data exposed includes email addresses, screen names, and bcrypt-hashed passwords. The Internet Archive responded to the breach quickly and transparently, immediately implementing security measures, disabling compromised libraries, and restoring service in read-only mode while the organization strengthened its defenses. This breach is notable for OSINT researchers interested in online archives and historical data access, as it suggests users engaged in digital research or preservation activities.

2\. VimeWorld (October 2018)

VimeWorld, a Russian Minecraft service, experienced a data breach in 2018 that exposed data on 3.1 million users. The compromised information includes usernames, email addresses, IP addresses, and hashed passwords (MD5 or bcrypt). This breach’s recent availability in DBSEs presents new opportunities for researchers interested in gaming communities, particularly among Russian-speaking audiences.

3\. StreamCraft (July 2020)

The StreamCraft breach in July 2020 affected 1.8 million records, exposing usernames, email addresses, IP addresses, and hashed passwords (MD5 or bcrypt). StreamCraft data, newly accessible for OSINT purposes, provides a look into the online behavior of gaming communities, especially among users who favor multiplayer gaming.

4\. AlpineReplay (2019)

The 2019 breach of AlpineReplay, a fitness-tracking app later integrated into Trace, exposed 900,000 records, including email addresses, usernames, dates of birth, gender, weight, and passwords hashed with MD5 or bcrypt. Recently appearing in DBSEs, this data gives insights into the interests of fitness enthusiasts, particularly those who use digital tools to track performance in sports like skiing and snowboarding.

## **Why These Data Breaches Matter to Researchers**

When an OSINT researcher finds an email address in one of these breaches, it can reveal valuable information about the target’s digital activities. Each platform represents a specific online community or interest, giving clues about an individual’s preferences, affiliations, or lifestyle.

• Internet Archive: If someone’s data is in the Internet Archive breach, it might indicate an interest in digital preservation, academic research, or access to open-source content. This can suggest a background in academia or a strong interest in historical records.

• VimeWorld and StreamCraft: The presence of someone’s account in these gaming-related breaches points to involvement in online gaming, possibly within Russian-speaking or international communities. This can help an investigator understand the target’s recreational interests and engagement in gaming culture.

• AlpineReplay: An account in the AlpineReplay breach implies an interest in fitness, specifically in winter sports like skiing and snowboarding. The individual is likely health-conscious and inclined toward tracking their performance, providing insights into their lifestyle and personal values.

Simply knowing that a target’s email address is associated with one of these platforms can reveal a lot about them. However, OSINT researchers should approach this data cautiously. While these accounts provide contextual information, they don’t give a complete picture of a person’s behavior or habits, so researchers should use this information as a starting point rather than a conclusive profile.

## **Detailed Look at the Internet Archive Data Breach**

The October 2024 Internet Archive breach involved the exposure of data from around 31 million user accounts. This breach, linked to a compromised GitLab token, allowed attackers to access development servers, revealing email addresses, screen names, and bcrypt-hashed passwords. The first breach occurred on October 9, with attackers exploiting a GitLab configuration file on the Internet Archive’s servers that contained an exposed authentication token. This gave them access to the source code, credentials, and, ultimately, the database management system, where they downloaded user data and modified site elements. Reports suggest this token had been accessible since December 2022, giving attackers a prolonged opportunity to exploit it. On October 20, a second breach occurred, this time exploiting unrotated Zendesk API tokens to access user support tickets. During this period, hackers defaced the Internet Archive’s website using JavaScript alerts and launched DDoS attacks attributed to the hacker group SN\_BlackMeta. In response, the Internet Archive implemented security measures, scrubbed compromised systems, and temporarily operated in a read-only mode before restoring full access. This quick and transparent response from the Internet Archive emphasized the organization’s commitment to user security.

An additional OSINT trick is available for researchers using the Internet Archive. By using the search function on the top right corner of the Internet Archive’s website, investigators can enter an email address associated with a target’s account to see if an account exists. Although the email address itself isn’t publicly identified in the profile, the search function will still locate the account, providing access to profile information and showing data and websites archived by the user. This technique can be particularly useful for tracing interests, historical engagements, and online behavior through the Internet Archive.

Founder Brewster Kahle reported that the organization is reinforcing its defenses and emphasized the Internet Archive’s commitment to secure its platform. For OSINT researchers, this breach provides a unique opportunity to explore user demographics and interests in digital archives, though it demands careful handling to avoid further privacy violations.

## **Citations**

1\. Internet Archive (Archive.org) Hacked for Second Time in a Month

URL: https://hackread.com/internet-archive-archive-org-hacked-for-second-time/

2\. Internet Archive hacked, data breach impacts 31 million users

URL: https://www.bleepingcomputer.com/news/security/internet-archive-hacked-data-breach-impacts-31-million-users/

3\. Hackers Claim ‘Catastrophic’ Internet Archive Attack - Newsweek

URL: https://www.newsweek.com/catastrophic-internet-archive-hack-hits-31-million-people-1966866

4\. Internet Archive Breach Exposes 31 Million Users - WIRED

URL: https://www.wired.com/story/internet-archive-hacked/

5\. The Internet Archive is finally mostly back online after a series of cyberattacks

URL: https://www.zdnet.com/article/the-internet-archive-is-finally-mostly-back-online-after-a-series-of-cyberattacks/

6\. Internet Archive hacker claims to still have access, responds to Zendesk support tickets

URL: https://therecord.media/internet-archive-alleged-zendesk-account-breach

7\. Hackers exploited GitLab tokens for Internet Archive breach

URL: https://www.breechingcomputer.com/news/security/internet-archive-breached-again-through-stolen-access-tokens

8\. Hackers steal information from 31 million Internet Archive users

URL: https://www.npr.org/2024/10/20/nx-s1-5159000/internet-archive-hack-leak-wayback-machine

## Help Support Our Non-Profit Mission

If you enjoyed this article or found it helpful please consider making a **U.S. tax-deductible** donation, Secjuice is a non-profit and volunteer-based publication powered by donations. We will use your donation to help cover our hosting costs and **keep Secjuice an advertisement and sponsor free zone**.

[Make a tax-deductible donation](https://opencollective.com/secjuice)
