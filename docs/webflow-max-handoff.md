# Webflow + Max Handoff

Date: 2026-05-07

Purpose: give Max a clean, buildable Webflow brief for the IHL referrer campaign landing page and online referral pathway.

Active priority: referrer landing page first. Broader site-wide brand work should remain background context until this page is approved.

## Current Build Source

- Live preview: https://richie261.github.io/ihl-referral-landing-page/
- Landing page prototype: `index.html`
- Form prototype: `online-referral-form-v1.html`
- Pasteable Webflow section: `webflow/referrals-landing-webflow-embed.html`
- Decisions: `docs/decisions.md`
- Launch checklist: `docs/launch-checklist.md`
- Source inventory: `docs/landing-page-source-inventory.md`
- Live-site transfer notes: `docs/webflow-transfer-notes.md`

## Live IHL Website Alignment

Checked on 2026-05-11:

- https://www.institute4healthyliving.com/
- https://www.institute4healthyliving.com/referrals

The live site is already Webflow. The referrer landing sections should use the existing site nav/footer and sit above the current `/referrals` form embed.

Match:

- Primary green `#2d4f37`.
- Dark green `#114733`.
- Light section background `#f7f8f5`.
- Hairline border `#e2e6df`.
- Primary font `Calibre`.
- Heading font `Family`.
- Current site language around right-fit clinician matching, online/in-person care and safe therapeutic connection.

## Launch Decision

Use `/referrals` as the canonical public page unless the current IHL site already has a stronger reason to use `/refer`.

Create `/refer` as a short campaign alias or redirect to `/referrals`, so printed material, QR codes and verbal instructions remain easy.

Do not point the campaign to the page until the form destination, intake notification, attachment handling and HubSpot boundary are confirmed.

## Page Build Order

Build the Webflow page in this order:

1. Hero: "Refer a patient to IHL."
2. First-viewport referral card with HealthLink EDI `inshealh`.
3. Referral options: HealthLink, online form, intake email, phone/fax.
4. What to include in a referral.
5. Referral pathway: submit, intake review, clinician matching, appointment/feedback.
6. Clinical scope.
7. Referrer guide CTA.
8. Footer with address, intake email, phone and HealthLink EDI.

HealthLink must be visible in the first viewport:

`HealthLink EDI: inshealh`

Suggested supporting copy:

`Search for Institute for Healthy Living or use EDI inshealh from compatible clinical software.`

## Public Webflow Content Rules

Do not include:

- "Boutique", "Eastern Suburbs", or other vibe/context notes as literal page copy.
- Guided-tour or explanatory process commentary.
- "Preferred referral method" language.
- Detailed HubSpot or internal pipeline wording.
- Time-based claims such as same-day triage or 1-2 week availability unless operationally approved.

Keep:

- HealthLink EDI `inshealh`.
- Online form.
- Intake email.
- Phone and fax.
- Routine referral / not-for-emergency wording.
- Conservative availability and funding language.

## Webflow Form Decision

Recommended phase-one approach:

Use the landing page in Webflow, but send the actual clinical referral form to a secure approved intake workflow or a custom form endpoint. Do not connect a clinical Webflow form directly to HubSpot.

The online form can collect clinical referral content only if the storage, notification, file upload, access control and privacy/security workflow are approved.

HubSpot may receive only referrer and campaign metadata:

- Referrer name.
- Practice or organisation.
- Profession or role.
- Email.
- Phone.
- Source = website referral form.
- Campaign/source tag.
- Date submitted.
- First referral yes/no, if available.

HubSpot must not receive:

- Patient/client name.
- Date of birth.
- Clinical notes.
- Referral reason.
- Risk details.
- Attachments.
- Medicare number or health identifiers.

## Campaign Attribution

The prototype now preserves whitelisted campaign query parameters from the landing page into the form preview.

Allowed parameters:

- `utm_source`
- `utm_medium`
- `utm_campaign`
- `utm_content`
- `utm_term`
- `gclid`
- `fbclid`
- `msclkid`
- `campaign`
- `source`
- `ref`

Default values if no campaign parameters exist:

- `utm_source=ihl_referrer_campaign`
- `utm_medium=landing_page`
- `utm_campaign=referrer_growth_2026`
- `landing_page=/referrals`

Final form should store these as hidden non-clinical fields. They can sync to HubSpot as referrer relationship and campaign attribution metadata.

## Webflow Implementation Notes

Use simple Webflow sections rather than overbuilding:

- One main page.
- Clean anchor links.
- Clear CTA buttons.
- Mobile-first check.
- No complex animations required.
- Keep HealthLink and intake contact details easy to copy.
- Prefer native Webflow sections if Max wants to maintain visually in Designer.
- If speed matters, paste `webflow/referrals-landing-webflow-embed.html` into an Embed element above the existing GP referral form.
- Replace `REFERRER_GUIDE_URL` with the uploaded Webflow asset URL for the referrer guide PDF.

If using Webflow native forms for any non-clinical contact or request-guide action, confirm where submissions are stored and who receives notifications.

If using file upload, confirm the file upload plan limits and the security/privacy workflow before accepting referral letters, MHTPs or reports.

Official Webflow references checked on 2026-05-07:

- Forms overview: https://help.webflow.com/hc/en-us/articles/33961347548563-Forms-overview
- Form file upload: https://help.webflow.com/hc/en-us/articles/33961307228947

## Max Build Checklist

- Create or update `/referrals`.
- Create `/refer` redirect or alias.
- Port approved public sections from `index.html`.
- Remove internal review content.
- Confirm HealthLink EDI is exactly `inshealh`.
- Replace form preview links with final secure form URL.
- Add hidden attribution fields to the final form workflow.
- Confirm intake notification destination.
- Confirm attachment handling.
- Confirm HubSpot sync excludes all patient and clinical fields.
- Add final PDF guide link only after the current guide is approved.
- Test desktop and mobile.
- Test one full dummy submission before campaign traffic is sent.

## Message To Max

Max, the page is ready to build as a simple referrer landing page above the existing `/referrals` form. Use `/referrals` as canonical unless there is a live-site reason not to, and add `/refer` as a campaign-friendly redirect. Please present HealthLink, online form, intake email, phone and fax clearly so referrers can choose what works for them. Route full clinical referral data to the approved secure intake workflow, and only pass referrer/campaign metadata to HubSpot.
