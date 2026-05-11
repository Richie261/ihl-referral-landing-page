# Webflow Transfer Notes

Date: 2026-05-11

Purpose: make the referrer landing page easy to move into the live IHL Webflow site.

## Live Website Reference

Checked:

- https://www.institute4healthyliving.com/
- https://www.institute4healthyliving.com/referrals

The live site is a Webflow build using:

- Site ID: `66fb6bc216ae048b2c95647d`
- Webflow CSS: `ihl-therapy.webflow.shared.184e2839d.min.css`
- Primary green: `#2d4f37`
- Dark green: `#114733`
- Light section background: `#f7f8f5`
- Section border: `#e2e6df`
- Primary font: `Calibre`
- Heading font: `Family`

The homepage positioning to stay close to is:

- "A clinical psychology practice that matches you with the right therapist..."
- Online and in-person therapy.
- Safe fit, connection, timely access, and personalised care.

The existing `/referrals` page already has an embedded GP referral form with `id="gp_referral_form"`. The new landing sections should sit above that form and link to it using `#gp_referral_form`.

## Files To Use

- Pasteable Webflow section: `webflow/referrals-landing-webflow-embed.html`
- Local prototype: `index.html`
- Online form prototype: `online-referral-form-v1.html`
- Logo extracted from referrer PDF: `assets/ihl-logo.png`
- Referrer guide PDF: `assets/ihl-referrer-guide.pdf`

## Recommended Webflow Build

1. Open the live Webflow `/referrals` page.
2. Keep the existing site nav and footer.
3. Add the landing sections above the current referral form embed.
4. Paste `webflow/referrals-landing-webflow-embed.html` into a Webflow Embed element, or rebuild the same structure as native Webflow sections using the `rf-` class names.
5. Upload `assets/ihl-referrer-guide.pdf` to Webflow assets.
6. Replace `REFERRER_GUIDE_URL` in the embed with the Webflow asset URL.
7. Keep the online referral CTA pointed to `#gp_referral_form` if the form remains on the same page.
8. Keep HealthLink, online form, intake email, phone and fax as equal referral options.

## Design Notes

- Do not include "boutique", "Eastern Suburbs", or other vibe/context notes as public copy.
- Keep the page useful and direct, with no guided-tour explanation.
- Use the existing Webflow site palette and typography inheritance.
- Keep rounded corners restrained and clinical.
- Keep HealthLink EDI `inshealh` visible in the first viewport.
- Keep the emergency/crisis caveat concise.

## Data Boundary

Full clinical referral data should only go to the approved secure intake workflow.

HubSpot or marketing reporting may receive only non-clinical campaign/referrer metadata after approval:

- Referrer name.
- Practice or organisation.
- Profession or role.
- Email.
- Phone.
- Campaign/source attribution.
- Submission date.

Do not send patient/client name, DOB, referral reason, risk notes, attachments or clinical documents to HubSpot.
