---
layout: default
title: Privacy Policy
description: How MythDusk collects, uses, and protects your information.
permalink: /privacy-policy/
show_updated: true
---

# Privacy Policy

{% assign legal = site.data.legal %}
{% assign privacy_url = site.data.legal.privacy_policy_path | absolute_url %}

{{ legal.entity_name }} ("we," "us," or "our") operates **MythDusk**, a turn-based puzzle RPG for iOS and Android (the "**App**"). This Privacy Policy explains how we collect, use, disclose, and protect information when you use the App.

By using the App, you agree to this Privacy Policy. If you do not agree, do not use the App.

## Who we are

- **App name:** MythDusk
- **Package / bundle ID:** `com.vividmemories.mythdusk`
- **Developer:** {{ legal.entity_name }}
- **Email:** [{{ legal.contact_email }}](mailto:{{ legal.contact_email }})
{% if legal.postal_address != "" %}- **Address:** {{ legal.postal_address }}
{% else %}- **Postal address:** Available on request by email
{% endif %}- **Website:** {{ legal.website_url }}


## Scope

This policy applies to the App and related services (cloud save, in-app purchases{% if legal.ads_enabled %}, advertising{% endif %}). It does not apply to third-party websites or services you open through links in the App.

## Information you provide

- If you sign in with **Google** or **Apple**, we receive identifiers and profile information those providers allow (for example display name and email if shared).
- You may play as a **guest** using anonymous **Firebase Authentication**; we assign a user ID without requiring an email.
- You may set a **display name** stored with your game profile.
- A guest account may later be **linked** to Google or Apple to preserve progress. If an account already exists for that sign-in method, the App may ask you to choose between profiles.
- If you contact us by email, we receive your message and email address.

## Game and profile data (when signed in)

We store gameplay and progression data linked to your account in **Google Firebase Cloud Firestore** under your user ID, including for example:

- Campaign / chapter progress and completed nodes
- Coins, gems/lives (or equivalent soft currency and lives), and XP/mastery if used
- Hero unlocks, equipped skill loadouts, and personality upgrades
- Prep inventory, weekly challenge completion keys, and chapter medal progress/claims
- Cosmetic / owned items if any
- In-app purchase entitlements (for example starter packs{% if legal.ads_enabled %}, Remove Ads{% endif %}) when offered
- Timestamps for rewards, daily/weekly claims{% if legal.ads_enabled %}, and optional ad-based rewards{% endif %}

## Information collected automatically

- Device and app information (device type, OS, app version, language, diagnostics)
- **Firebase Analytics** (how the App is used; may be linked to your user ID when signed in)
- **Firebase Crashlytics** in release builds (crash logs; may be linked to your user ID)
- **Firebase App Check** (helps protect our backend from abuse)
- Local settings on your device (for example sound and haptics preferences)

## Advertising

{% if legal.ads_enabled %}

We use **Google AdMob**, including:

- **Rewarded video ads** (optional; for in-game benefits such as rewards or resources)
- **Interstitial ads** (unless you purchased Remove Ads, where offered)

AdMob and partners may collect or receive:

- Advertising ID on Android and, if you allow it, IDFA on iOS
- IP address (often truncated), device identifiers, ad interactions, coarse location from IP
- Consent choices through **Google User Messaging Platform (UMP)** in the EEA, UK, and Switzerland

{% if legal.personalized_ads %}

We may show **personalized ads** tailored to your interests using advertising identifiers and similar technologies, subject to your consent where required (including **UMP** in the EEA/UK/CH and **App Tracking Transparency** on iOS). You can limit tracking in device settings and through in-app consent prompts.

{% else %}

We use **non-personalized ads** only. Ads are not tailored to you based on cross-app tracking. You may still see contextual ads (for example based on app content or general location from IP).

{% endif %}

If you purchase **Remove Ads** (where offered), interstitial ads stop. Rewarded ads may still appear only if you choose to watch them for in-game benefits.

{% else %}

The current soft-launch / closed-test versions of MythDusk **do not show ads**. We do **not** currently integrate **Google AdMob**, load advertising identifiers for ads, or show UMP consent prompts for advertising.

If we enable advertising in a future update, we expect to use **Google AdMob** (rewarded and/or interstitial ads). Before ads go live we will:

- Update this Privacy Policy and store data-safety / privacy questionnaires
- Update in-app Legal links and the [Privacy Choices]({{ site.data.legal.privacy_choices_path | absolute_url }}) page
- Use consent flows where required (for example UMP in the EEA/UK/CH)
- Default to **non-personalized** ads unless we change that setting and obtain required consent

{% endif %}

## Payments

Purchases are processed by **Apple App Store** or **Google Play**. We do not receive your full card number. We receive purchase confirmation and entitlement status for items you buy (for example gem packs or other shop offers).

## How we use information

We use information to:

- Provide and operate the App (gameplay, saves, campaigns, weekly challenges, hero progression)
- Authenticate you and sync progress when you sign in
- Process in-app purchases and restore purchases
{% if legal.ads_enabled %}- Show ads and measure ad performance (AdMob)
{% endif %}- Analyze usage and improve the App (Firebase Analytics)
- Detect, prevent, and address fraud, abuse, and technical issues (App Check, security rules)
- Fix crashes and improve stability (Crashlytics)
- Comply with law and enforce our Terms
- Respond to your requests

## Legal bases (EEA/UK)

Where GDPR applies, we rely on:

- **Contract** — to provide the App and features you request
- **Legitimate interests** — security, analytics, improving the App{% if legal.ads_enabled %}{% unless legal.personalized_ads %}, non-personalized advertising{% endunless %}{% endif %}
{% if legal.ads_enabled %}- **Consent** — where required for ads (UMP) and, if applicable, personalized ads or iOS tracking
{% endif %}- **Legal obligation** — when we must comply with law

{% if legal.ads_enabled %}You may withdraw consent for ads where applicable; withdrawal does not affect processing already performed.{% endif %}

## Who we share with

We do not sell your personal information for money. We use processors including:

| Provider | Purpose |
|----------|---------|
| **Google Firebase** (Auth, Firestore, Analytics, Crashlytics, App Check, Cloud Functions) | Account, cloud save, analytics, crashes, server logic |
{% if legal.ads_enabled %}| **Google AdMob** (and advertising partners) | Advertising |
{% endif %}| **Google / Apple** | Sign-in and in-app purchase processing |

They may process data in the **United States** and other countries. We use contractual and technical safeguards where required by law.

We may also disclose information if required by law, to protect rights and safety, or in connection with a merger or sale of assets.

## Retention

- **Account data:** while your account is active and for a reasonable period afterward
- **Analytics and crashes:** per Firebase/Google retention settings
{% if legal.ads_enabled %}- **Ad-related data:** governed by Google’s policies and your consent settings
{% endif %}- **Local data:** until you uninstall the App or clear app data

## Your choices and rights

Depending on your location, you may have rights to **access**, **correct**, **delete**, **restrict**, **object**, **portability**, and to **withdraw consent**.

{% if legal.ads_enabled %}

**Advertising choices**

- **EEA/UK/CH:** Use the in-app consent flow (UMP) when shown
- **iOS:** Settings → Privacy & Security → Tracking
- **Android:** Settings → Google → Ads
- **Remove Ads:** Purchase in the shop (where offered) to disable interstitial ads

{% endif %}

**Account and data deletion**

Open MythDusk → **Settings** → **Legal** → **Delete your data**, then email [{{ legal.contact_email }}](mailto:{{ legal.contact_email }}) with subject **"MythDusk Account Deletion"** and include your display name and sign-in method (Google, Apple, or guest). We will process the request within **{{ legal.deletion_sla }}**, except where we must retain data for legal obligations.

See [Delete your data]({{ site.data.legal.delete_data_path | absolute_url }}) for details.

**California (CCPA/CPRA)**

California residents may have rights to know, delete, and correct personal information, and to opt out of “sale” or “sharing” for cross-context behavioral advertising. We do not sell personal information for money. Contact us to exercise your rights.

**Other regions**

Contact [{{ legal.contact_email }}](mailto:{{ legal.contact_email }}) to exercise applicable rights.

## Children

MythDusk is **not directed to children under 13** (or under 16 in some jurisdictions). We do not knowingly collect personal information from children. If you believe a child provided personal information, contact us and we will delete it.

## Security

We use authentication, Firestore security rules, and App Check. No method of transmission or storage is 100% secure.

## International transfers

We and our processors may transfer data outside your country, including the United States, with appropriate safeguards where required (for example Standard Contractual Clauses).

## Changes

We may update this Privacy Policy. We will post the new date at the top of this page and, where required, notify you in the App or through store listings. Continued use after changes means you accept the updated policy.

## Contact

**{{ legal.entity_name }}**  
[{{ legal.contact_email }}](mailto:{{ legal.contact_email }})  
{% if legal.postal_address != "" %}{{ legal.postal_address }}{% else %}Postal address available on request by email.{% endif %}
