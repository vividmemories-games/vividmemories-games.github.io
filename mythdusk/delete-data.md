---
layout: default
title: Delete Your Data
description: How to delete your MythDusk account and game data.
permalink: /delete-data/
show_updated: true
---

# Delete Your Data

{% assign legal = site.data.legal %}
{% assign contact_url = site.data.legal.contact_path | absolute_url %}

You can request deletion of your MythDusk account and associated cloud data.

## From the app

1. Open **MythDusk**
2. Go to **Settings**
3. Under **Legal**, tap **Delete your data** (opens this page)
4. Email [{{ legal.contact_email }}](mailto:{{ legal.contact_email }}?subject=MythDusk%20Account%20Deletion) with subject **"MythDusk Account Deletion"**
5. Include your display name and sign-in method (Google, Apple, or guest)

We will process the request within **{{ legal.deletion_sla }}**, except where we must retain data for legal obligations (for example fraud prevention or tax records for purchases).

## What we delete

When we fulfill a valid deletion request, we delete or irreversibly anonymize:

- Your Firebase Authentication account (guest, Google, or Apple)
- Your Firestore profile (campaign progress, currency, heroes, prep inventory, entitlements, and related cloud data)

Local settings on a device are cleared when you uninstall the app or clear app data.

## Cannot access the app?

Email [{{ legal.contact_email }}](mailto:{{ legal.contact_email }}?subject=MythDusk%20Account%20Deletion) with the same subject and details. See also our [Contact page]({{ contact_url }}).

## Future in-app deletion

One-tap in-app account deletion may be added in a later update. Until then, email is the supported path and is sufficient for store data-deletion requirements.
