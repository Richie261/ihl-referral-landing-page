# Referral Page Research Notes

Date: 2026-05-11

Purpose: keep a concise record of why the referrer landing page was simplified after comparing The Banyans and other Australian health referral pages.

## Reference Pages Reviewed

- The Banyans referral form: https://thebanyans.com.au/referral-form/
- The Banyans healthcare professionals page: https://thebanyans.com.au/healthcare-professionals/
- MindSpot GP referral pathway: https://www.mindspot.org.au/mindspot-gp/
- Deakin Private Hospital health professionals page: https://deakinprivate.com.au/health-professionals/
- Deakin Private Hospital referral process: https://deakinprivate.com.au/referral-process/
- Ramsay Psychology referral information: https://www.ramsaymentalhealth.com.au/en/our-locations/Psychology-services/Ramsay-Psychology/for-doctors/Referral-information/
- Gidget Foundation health professional referrals: https://www.gidgetfoundation.org.au/access-services/health-professional-referrals
- Reflective Psychology GP/referrals page: https://www.reflectivepsych.com.au/for-gps-referrals/

## Direction Taken

- Make the page feel like a professional referral reference, not a campaign funnel.
- Lead with referral mechanics and clinical confidence.
- Keep HealthLink EDI visible in the first viewport.
- Present HealthLink, online form, intake email, phone and fax as equally available pathways.
- Remove numbered process cards and heavy guided-tour language.
- Keep clinical scope concise, using the referrer guide PDF for deeper detail.
- Retain conservative emergency wording and avoid unapproved wait-time claims.

## Sana Health Group Learning

- The strongest part of Sana's referrals page is the simple path to action: arrive, understand the page is for healthcare professional referrals, then make a referral.
- The weaker part is the long explanatory process section and a heavy embedded form. IHL should avoid the explanatory middle and invest in the form itself.
- IHL direction after this review: a short doorway, compact referral options, then the form on the same page.
- Form principle: patient contact details first, uploadable source documents second, referrer authority last.

## Human and Referrer Verification

- CAPTCHA or equivalent human verification should be included in the live form and validated server-side.
- CAPTCHA confirms likely human interaction; it does not confirm that the referrer is who they say they are.
- Referrer identity should be supported through professional email, practice details, provider identifiers where available, uploaded documents/letterhead and IHL's permission to verify details before progressing intake.

## HealthLink EDI Lookup

- Official HealthLink pages provide a public Provider Map and a HealthLink Online Directory for subscribers.
- The Provider Map is location-search based. It confirms IHL appears as "Institute For healthy Living" with EDI `inshealh`, but it does not expose a clean, stable provider-specific public profile URL.
- The Online Directory requires a HealthLink login and is intended for HealthLink users to find messaging addresses.
- Page decision: include a simple "Open HealthLink lookup" link to the public Provider Map, but keep `EDI: inshealh` visible and copyable. The link supports discovery; the EDI remains the reliable referral detail.

Sources checked:

- https://www.healthlink.com.au/healthlink-provider-map/
- https://www.healthlink.com.au/products/healthlink-provider-directory/
- https://aupd.healthlink.net/login.php
- https://aupd.healthlink.net/hlkwebmap/
