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

You can delete your MythDusk account and associated cloud data **immediately** from the app.

## Delete in the app

1. Open **MythDusk**
2. Go to **Settings**
3. Scroll to **Legal & privacy**
4. Tap **Delete my account**
5. Confirm — this cannot be undone

We delete:

- Your Firebase Authentication account (guest, Google, or Apple)
- Your Firestore profile (campaign progress, currency, heroes, prep inventory, entitlements, and related cloud data)
- Local settings on that device after sign-out

Deletion is **immediate** once you confirm. We may retain minimal records only where required by law (for example fraud prevention or tax records for purchases).

## Cannot access the app?

If you are locked out or the app will not open, email [{{ legal.contact_email }}](mailto:{{ legal.contact_email }}) with subject **"MythDusk Account Deletion"** and include your display name and sign-in method. We will process the request within **{{ legal.deletion_sla }}**.

See also our [Contact page]({{ contact_url }}).
