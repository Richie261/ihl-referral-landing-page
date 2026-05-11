# Sitewide Webflow Brand Update Checklist

Use this checklist in Webflow after the messaging system is approved.

## Global Components

- Update nav CTA labels only if needed; default should remain `Book an appointment`.
- Keep the phone number visible in nav/footer.
- Standardise footer contact details.
- Remove any visible placeholder/test blocks, including `This is some text inside of a div block`.
- Keep footer inclusion and cultural safety statements.

## Page Template Updates

### Static Pages

Update in this order:

1. Home.
2. Get Support.
3. Referrals.
4. Fees and Rebates.
5. About.
6. Team.
7. Offerings.
8. Group Therapy.
9. Cognitive Testing.
10. Careers.

For each page:

- Confirm one clear H1.
- Confirm one primary CTA.
- Confirm one secondary CTA where useful.
- Remove duplicate CTA text where Webflow has nested links.
- Check mobile layout after copy updates.
- Check meta title and description.

### CMS Templates

Templates to standardise:

- Team member pages.
- Concern pages.
- Treatment pages.
- Blog pages.
- FAQ pages.

For concern pages:

- H1: `[Concern]`
- Intro: what this can feel like, written in calm plain language.
- Section: how therapy can help.
- Section: how IHL matches care.
- CTA: `Book an appointment`.

For treatment pages:

- H1: `[Treatment] at IHL`
- Intro: what the modality is.
- Section: when it may help.
- Section: how IHL uses it.
- CTA: `Talk to intake` or `Book an appointment`.

## Metadata Formulas

Concern title:

`[Concern] Psychologist Bondi Junction | IHL`

Concern description:

`Evidence-based therapy for [concern] in Bondi Junction and online. IHL helps match clients with the right psychologist for their needs.`

Treatment title:

`[Treatment] Therapy Bondi Junction | IHL`

Treatment description:

`Learn about [treatment] at IHL. Evidence-based psychological care available in Bondi Junction and online.`

Team title:

`[Clinician Name] | [Role] | IHL`

Team description:

`Meet [Clinician Name], [role] at Institute for Healthy Living in Bondi Junction. View focus areas, modalities and availability.`

## Copy QA

Search the Webflow site for:

- `Lorem ipsum`
- `Heading 1`
- `Heading 2`
- `This is some text inside of a div block`
- `unrivalled`
- `always open`
- `get started in minutes`
- `same-day`
- `1 business day`
- `Principle Practitioner`
- `Practicioners`
- `contact@institute4healthyliving.com`

Confirm or replace each instance.

## Referrals Page

- Add `webflow/referrals-landing-webflow-embed.html` above the existing form.
- Replace `REFERRER_GUIDE_URL`.
- Keep the form ID `gp_referral_form` if CTAs anchor to it.
- Confirm the clinical form endpoint and file-upload handling.
- Confirm no patient clinical data is sent to HubSpot.

## Final Review

- Desktop and mobile check for every updated page.
- Form test for client booking/contact paths.
- Dummy referral test for `/referrals`.
- SEO title/description check for static pages and CMS templates.
- Policy check for fees, cancellation, hours and rebates.
