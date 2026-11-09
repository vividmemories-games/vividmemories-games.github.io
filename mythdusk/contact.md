---
layout: default
title: Contact Us
description: How to contact MythDusk support.
permalink: /contact/
show_updated: true
---

# Contact Us

{% assign legal = site.data.legal %}

Need help with MythDusk, your account, privacy, purchases, or data requests?

## In the app (preferred)

1. Open **MythDusk**
2. Go to **Settings**
3. Under **Legal**, tap **Contact us**
4. Your mail app should open with a pre-filled **MythDusk Support** subject
5. Describe your issue and send — we usually reply within a few business days

If your device cannot open email, use the address below.

## Email directly

Email [{{ legal.contact_email }}](mailto:{{ legal.contact_email }}?subject=MythDusk%20Support).

Include:

- Your display name in the app
- How you sign in (Google, Apple, or guest)
- A short description of your question

## Postal address

**{{ legal.entity_name }}**  
{% if legal.postal_address != "" %}{{ legal.postal_address }}{% else %}A postal address is available on request by email if you need one for a legal or regulatory matter.{% endif %}
