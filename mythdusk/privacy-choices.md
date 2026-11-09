---
layout: default
title: Privacy Choices
description: Manage privacy settings and future ad consent in MythDusk.
permalink: /privacy-choices/
show_updated: true
---

# Privacy Choices

{% assign legal = site.data.legal %}
{% assign privacy_url = site.data.legal.privacy_policy_path | absolute_url %}
{% assign contact_url = site.data.legal.contact_path | absolute_url %}
{% assign delete_url = site.data.legal.delete_data_path | absolute_url %}

## MythDusk mobile app

{% if legal.ads_enabled %}

### Advertising consent (EEA, UK, Switzerland)

When required, MythDusk shows Google's **User Messaging Platform (UMP)** consent form before ads load.

To change your choices later:

1. Open **MythDusk**
2. Go to **Settings**
3. Tap **Manage ad consent** (shown when required in your region)

### Device settings

You can also limit ad personalization and tracking in your device settings:

- **iOS:** Settings → Privacy & Security → Tracking
- **Android:** Settings → Google → Ads

### Remove ads

Purchase **Remove Ads** in the in-app shop (where offered) to disable interstitial ads.

{% else %}

### Advertising

The current soft-launch / closed-test builds of MythDusk **do not show ads** and do not load AdMob or UMP consent prompts.

If advertising is enabled in a future update, we will:

- Update the [Privacy Policy]({{ privacy_url }}) and store listings before ads go live
- Use consent flows where required (for example UMP in the EEA/UK/CH)
- Keep this page updated with in-app controls

### Device settings

You can still limit tracking and ad personalization in your device settings for other apps:

- **iOS:** Settings → Privacy & Security → Tracking
- **Android:** Settings → Google → Ads

{% endif %}

### Account and data

- **Delete account / data:** Settings → **Legal** → **Delete your data** — see [Delete your data]({{ delete_url }})
- **Privacy Policy:** [{{ privacy_url }}]({{ privacy_url }})
- **Contact:** Settings → **Legal** → **Contact us**, or [Contact page]({{ contact_url }})

## This website

This legal site does **not** use advertising cookies or analytics at this time. See our [Cookie Policy]({{ site.data.legal.cookie_policy_path | absolute_url }}).

## Questions

Use **Contact us** in the app Settings, or visit our [Contact page]({{ contact_url }}).
