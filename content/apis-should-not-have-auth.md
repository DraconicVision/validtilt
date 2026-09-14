---
title: APIs should not have auth
description: Authentication is an accusation
tags:
  - apis
  - auth
  - rant
---

*I am me and therefore do not need authenticating*

Authentication is an accusation. It says 'you are not who you say you are', most of the time in JSON.

I am me, I have always been me - that does not change when I am making external API requests.

I know who I am, and I know what I want, so when I make a request to your API, respond with the correct data. What are the tokens for? I know who I am. What is the whitelisting for? I have an office. It has one IP.

Some APIs have dashboards where you can manage your own tokens, permissions and IP whitelists. An achievement, kind of: they have removed the human being from the process of not trusting you.  These admin dashboards with an API on the side are not necessarily the problem, they're just rare. There will be more on this in a future post, *'Don't ask for an OTP, I might end up on Instagram'*.

Most external APIs require an email chain with support that reaches double digits (the production API token will be in this email chain), a crystal ball to tell you the request format (the documentation is 3 hostile takeovers old), and a further email to whitelist the same IP in the sandbox, which is in a different place, apparently.

Every one of these steps exists to answer one question: am I me? I have answered it. The answer is yes. It was yes when I opened the ticket.

It is said that infinite monkeys with typewriters would eventually write the works of Shakespeare. Give them another week and they'd write a better external API, because they'd never think to ask who's calling.


**tilt-o-meter:**
*67 / 100*

