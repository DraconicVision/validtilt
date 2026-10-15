---
title: You have built a census
description: Country blocklists are prejudice with a config file
tags:
  - cloudflare
  - security
  - rant
---

*Vladimir Putin is not coming for your horse tinder*

The second thing most people do when they add their website to Cloudflare (after DNS, it's always DNS) is set up a custom security rule blocking whatever list of countries they decided are coming for their new project.

Assigning a threat level to a hundred million people because a database has an opinion about their IP range is prejudice with a config file. Your rule knows exactly which country an IP is registered in, and that fact has no bearing whatsoever on whether the person behind it wants to buy your product or take down your site. You have not built a threat model. You have built a census.

An IP from Kent costs pennies. A VPN costs less than lunch. Your blocklist is a list of places your attacker does not live. The only person you're blocking is a legitimate user on holiday, and, if you're unlucky, your own uptime monitor.

I have news for you: Vladimir Putin is not coming for your horse tinder.

Even if someone in one of your blocked countries did come for you, do you imagine they'd give up at the first 403? They will come at you from a botnet in Rhodes, a VM in Killybegs, a residential IP in France (more on that in my next post, *Remove France from the internet*). And if your blocklist is meant to stop North Korea specifically: the entire country has fewer IP addresses than the average office, and the people you're worried about left it years ago.

## When a rule does make sense

I know these rules make sense sometimes. Maybe only residents of certain countries are allowed to use your site. Maybe you want to sanction certain regimes. But if your rule is really about who you serve, you don't want a blocklist at all. You want an allowlist.

- Running a shop that only ships domestically? Allow your country.
- A window cleaner's site for one town? Allow your country.

Same rule, smaller list. It is not a security rule, and it will not stop anyone, because the attacker is already inside the country you just allowlisted.

## The real threat

The most likely person to take down your website is you. Your own deploy, your own migration, your own load test you forgot to stop. Add your own IP to the rule and see how much safer it feels.


**tilt-o-meter:**
*72 / 100*
