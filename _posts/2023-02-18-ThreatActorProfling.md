---
title: Threat Actor Profiling
date: 2023-02-18 +0800
categories: [CTI]
tags: [CTI]
render_with_liquid: false
---

## Threat actor profiling 

A fast and straightforward description of threat actor profiling. 

Before getting into what Threat Actor Profiling is, it's worthwhile to define what a threat actor is to me. I describe the term as any person or organization that intentionally causes harm in the digital sphere. Some examples of threat actors are Conti, Lazarus, and Anonymous. Threat actors can have multiple names due to different naming conventions across the security field. A prime example is how the North Korean group Lazarus is called Hidden Cobra, Guardians of Peace, APT38, Whois Team, and Zinc. Threat actors are going to have different motivations. Nation states may want secrets and intellectual property, Cybercriminals will attempt to profit, Hacktivists wish to make a statement, and some people do it for the lulz.

Threat Actor Profiling is discovering which threat actors are likely to attack your organization, documenting their techniques, tactics, and procedures(TTPs), and understanding their objectives in your network. Once you have all this information, you can compare your defenses to what a threat actor has a history of doing. 


## Finding our Threat Actors
Finding out who will likely attack your organization starts with some self-reflection. Understand what industry you are in, what type of data you hold, your customers, and your competitors. I monitor the news for cyber attacks involving those competitors, as well as anything happening in my industry. Once you have all this, you can start asking questions like who are the threat actors attacking my industry and/or my competition.

When researching these questions, scope out a time in which the event occurred. You want enough data to work with but don't want to overwhelm yourself with research. For example, who are the threat actors attacking my industry in the last three years? What competitors have suffered a breach within the previous year? Another question worth brainstorming is, "Will my organization be attacked due to my customers." This is something that takes more time to unravel. Understanding who your customers are and what data/access you have to them could allow you to properly scope if you would be a target of a supply chain attack. This is extreme thinking, and most companies will not meet these criteria, but no one wants to be the next Fazio Mechanical Services or Solarwinds.

![Desktop View](/assets/images/taprofiling/allgroups.png){: width="972" height="589" .w-50 .right}

These are the topics I chose within a two-year time frame of performing the research: 
* Any Threat Actor attacking my industry
* Any Threat Actor attacking my competitors
* Any Threat Actor using Supply Chain Attacks as a Tactic 

![Desktop View](/assets/images/taprofiling/vandi.png){: width="972" height="589" .w-50 .right}

I also limited the research to each category's top eight threat actors. Giving me a total of 24 data points to work with. I expected a large amount of overlap in the data, and there was. I also had to prune out actors who were not actively attacking my nation. From those 24, I was left with 13 unique threat actors. ![Desktop View](/assets/images/taprofiling/excelf.png){: width="972" height="589" .w-50 .right}

I researched these 13 threat actors heavily. Documenting their TTPs, understanding their capabilities, and gauging their possible intent of attacking my organization. This was a challenging task and required a large amount of reading and excel spreadsheets. Once finished, I could ascertain which actors to prioritize intelligence actions around. I also created a MITRE ATT&CK map to visualize the most common TTPs to prioritize creating defenses. 


![Desktop View](/assets/images/taprofiling/map.png)

## How I did it
In researching the threat actors, I used both closed and open-source tools. This quick blurb will point you toward two good resources to perform the operation above. 

[MITRE ATT&CK GROUPS](https://attack.mitre.org/groups/) 
	
Attack Groups is an excellent resource for finding TTPs, and articles pivot from to find more information. With the vast amounts of reports, knowledge, and pre-made attack maps leveraging ATT&CK is a no-brainer. I highly suggest checking out the [ATT&CK browser app](https://mitre-engenuity.org/cybersecurity/center-for-threat-informed-defense/attack-powered-suit/) as well. It wasn't around when I performed this, but I'm an avid user now. 

[APT Groups and Operations](https://docs.google.com/spreadsheets/d/1H9_xaxQHpWaa4O_Son4Gx0YOIzlcBWMsdvePFX68EKU/edit#gid=1864660085) 

This spreadsheet was put together by several researchers and holds excellent information. Make sure to look through all the columns and the different sheets. 

Several vendors offer information for free if you visit their sites or create free accounts. These vendors hold some excellent information, but I don't want to recommend anyone over the others or provide links. Some change their offerings and are no longer very viable. 

##  Resources
I wanted to provide a couple of interesting resources that may help you with threat actor profiling. It goes from basic description to in-depth frameworks. 


[Understanding the Value and Use of Threat Profiles by Christoffer Strömblad](https://www.truesec.com/hub/blog/understanding-the-value-and-use-of-threat-profiles)


[Quantifying Threat Actors with Threat Box by Andy Piazza](https://klrgrz.medium.com/quantifying-threat-actors-with-threat-box-e6b641109b11)

[Creating a Threat Profile for Your Organization By Stephen Irwin](https://www.giac.org/paper/gcih/1772/creating-threat-profile-organization/110995)












