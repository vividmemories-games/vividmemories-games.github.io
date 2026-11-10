---
layout: default
title: Terms and Conditions
description: Terms of service for using the MythDusk mobile app.
permalink: /terms-and-conditions/
show_updated: true
---

# Terms and Conditions

{% assign legal = site.data.legal %}
{% assign privacy_url = site.data.legal.privacy_policy_path | absolute_url %}

These Terms and Conditions ("**Terms**") govern your use of **MythDusk** (the "**App**") published by **{{ legal.entity_name }}** ("**we**," "**us**"). By downloading, installing, or using the App, you agree to these Terms and our [Privacy Policy]({{ privacy_url }}). If you do not agree, do not use the App.

## Eligibility

You must be at least **13 years old** (or the minimum age required in your country to consent to online services without parental consent). If you are under 18, you represent that your parent or guardian has reviewed these Terms with you.

## The App

MythDusk is a **turn-based puzzle RPG** for iOS and Android. Gameplay includes:

- Matching tiles to generate resources (**Attack**, **Mana**, **Healing**, **Shield**, **Ultimate**). Matching tiles does **not** deal direct damage.
- Spending resources and action points (AP) on hero skills
- **Campaign** chapters, bosses, and chapter medals
- **Weekly challenges**, prep items, hero unlocks, and skill loadouts

**Online real-time multiplayer against other players over the internet is not offered** unless we announce otherwise in the App or release notes.

## Accounts and guest play

- You may play as a **guest** (anonymous Firebase account) or sign in with **Google** or **Apple**.
- You are responsible for maintaining access to your sign-in method.
- You may link a guest account to Google or Apple to preserve progress; if an account already exists, the App may ask you to choose between profiles.
- You must not impersonate others or use offensive display names.

## Virtual items and game economy

The App includes virtual items such as **coins**, **lives** (or equivalent soft currency), **prep items**, **hero upgrades**, **skill loadouts**, **cosmetics**, and progression rewards. These items:

- Are **licensed, not owned** by you
- Have **no real-world cash value**
- Are **not transferable** outside the App
- May be **modified, balanced, or removed** by us at any time
- Do not create any property right in your favor

We may grant items through gameplay, daily/weekly rewards{% if legal.ads_enabled %}, optional ads{% endif %}, or purchases.

## In-app purchases

The App may offer digital purchases such as gem packs, starter offers, and other shop items described in the App{% if legal.ads_enabled %}, including **Remove Ads** (a non-consumable that removes **interstitial** advertisements where offered){% endif %}.

- Purchases are processed by **Apple** or **Google**; their terms apply to billing and refunds.
- Prices are shown in your local currency before purchase.
- **Restore purchases** is available where supported by the platform (Settings → Restore purchases).
- Except as required by law or store policy, **all sales are final** for digital content delivered immediately. Refunds, if any, are handled solely by Apple or Google under their policies.

## Advertising

{% if legal.ads_enabled %}

The free version of the App may display ads via **Google AdMob**. Ad availability is not guaranteed. In the EEA/UK/CH you may be asked for consent through **UMP** where required.

If you purchase Remove Ads (where offered), interstitial ads are disabled as described in the App. Misuse of ad rewards (for example exploiting bugs to obtain rewards without completing ads) is prohibited.

{% else %}

Current soft-launch / closed-test versions of MythDusk **do not display ads**. If we enable advertising later (for example via Google AdMob), we will update these Terms and the Privacy Policy before ads go live.

{% endif %}

## Acceptable use

You agree **not** to:

- Cheat, exploit bugs, use bots, or manipulate game logic or cloud functions
- Reverse engineer, decompile, or attempt to extract source code except as allowed by law
- Interfere with servers, Firestore, or App Check
- Use the App for any illegal purpose
- Circumvent {% if legal.ads_enabled %}ad or {% endif %}purchase systems

We may suspend or terminate access for violations.

## Intellectual property

The App, including graphics, text, software, and trademarks, is owned by **{{ legal.entity_name }}** or licensors and is protected by intellectual property laws. We grant you a limited, non-exclusive, non-transferable, revocable license to use the App for personal, non-commercial entertainment.

You do not acquire ownership of any virtual items or content.

## Third-party services

The App integrates third-party services (Firebase, Google Sign-In, Apple Sign-In, app stores{% if legal.ads_enabled %}, AdMob{% endif %}). Your use of those services is subject to their terms and privacy policies.

## Disclaimer of warranties

THE APP IS PROVIDED **"AS IS"** AND **"AS AVAILABLE."** TO THE MAXIMUM EXTENT PERMITTED BY LAW, WE DISCLAIM ALL WARRANTIES, EXPRESS OR IMPLIED, INCLUDING MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT.

We do not warrant uninterrupted, error-free, or secure operation, or that progress will never be lost.

## Limitation of liability

TO THE MAXIMUM EXTENT PERMITTED BY LAW, **{{ legal.entity_name }}** AND ITS OFFICERS, DIRECTORS, EMPLOYEES, AND AGENTS WILL NOT BE LIABLE FOR ANY INDIRECT, INCIDENTAL, SPECIAL, CONSEQUENTIAL, OR PUNITIVE DAMAGES, OR LOSS OF DATA, PROFITS, OR GOODWILL, ARISING FROM YOUR USE OF THE APP.

OUR TOTAL LIABILITY FOR ANY CLAIM ARISING FROM THESE TERMS OR THE APP WILL NOT EXCEED THE GREATER OF **(A)** THE AMOUNT YOU PAID US IN THE **12 MONTHS** BEFORE THE CLAIM OR **(B) TEN GBP / TEN US DOLLARS** (or local equivalent).

Some jurisdictions do not allow certain limitations; in those cases, our liability is limited to the fullest extent permitted by law.

## Indemnity

You agree to indemnify and hold us harmless from claims arising from your misuse of the App or breach of these Terms, except where caused by our gross negligence or willful misconduct.

## Termination

You may stop using the App at any time by uninstalling it. We may suspend or terminate your access if you violate these Terms or if we discontinue the App. Sections that by nature should survive (for example intellectual property, disclaimers, limitation of liability) will survive.

## Changes

We may modify the App or these Terms. Material changes will be indicated by updating the "Last updated" date and, where appropriate, in-App notice. Your continued use after changes constitutes acceptance.

## Governing law and disputes

These Terms are governed by the laws of **{{ legal.governing_law }}**, without regard to conflict-of-law rules.

Courts in **{{ legal.jurisdiction }}** have exclusive jurisdiction, except where consumer protection laws in your country require disputes to be heard in your local courts.

If you are an EU consumer, you may also use the [EU Online Dispute Resolution platform](https://ec.europa.eu/consumers/odr).

## Apple and Google specific terms

**Apple (iOS):** If you use the iOS App, Apple is not a party to these Terms and is not responsible for the App or its content. Apple has no obligation to provide maintenance or support. In case of failure to conform to warranty, you may notify Apple for a refund of the purchase price where applicable. Apple and its subsidiaries are third-party beneficiaries of these Terms.

**Google Play:** If you use the Android App, Google is not responsible for the App except as the billing agent for purchases.

## Contact

**{{ legal.entity_name }}**  
[{{ legal.contact_email }}](mailto:{{ legal.contact_email }})  
{% if legal.postal_address != "" %}{{ legal.postal_address }}{% else %}Postal address available on request by email.{% endif %}

Privacy Policy: [{{ privacy_url }}]({{ privacy_url }})
