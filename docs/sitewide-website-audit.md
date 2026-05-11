# IHL Sitewide Website Audit

Date: 2026-05-11

Purpose: capture the first pass of the live website audit for brand, messaging and Webflow cleanup.

Current status: parked as background context. Referrer landing page work remains the core focus.

## Scope Checked

Core pages:

- Home.
- Team.
- Offerings.
- Fees and rebates.
- About.
- Referrals.
- Get support.
- Group therapy.
- Cognitive testing.
- Careers.

CMS samples:

- Anxiety concern page.
- Cognitive Behavioural Therapy treatment page.

Sitemap groups:

- Core pages.
- Team CMS.
- Concern CMS.
- Treatment CMS.
- Blog CMS.
- FAQ CMS.

## Executive Summary

The site already has a strong foundation: right-fit clinician matching, online/in-person care, evidence-based treatment and a warm practice voice.

The main issue is consistency. The same ideas appear across the site, but the wording, risk level and polish change from page to page. Some pages are refined and client-facing; others contain placeholder content, older wording, inconsistent policy details or generic SEO titles.

The brand should be unified around:

`Right-fit psychological care, evidence-based support and long-term wellbeing.`

## Strong Existing Brand Assets

Keep and strengthen:

- The emphasis on therapist fit and safe connection.
- The clear online/in-person service model.
- The broad, multidisciplinary psychology team.
- The warm practice values: connection, accessibility and self-discovery.
- The Bondi Junction location signal.
- The inclusion and cultural safety statements in the footer.

## Messaging Drift

### 1. Tone moves between warm clinical and generic marketing

Examples of drift:

- Some pages are grounded in fit, care and evidence.
- Some pages use higher-intensity claims such as "unrivalled appointment access" or "results-driven".
- Some CMS pages read like generic treatment explainers rather than IHL-specific care pages.

Recommendation:

Use the sitewide brand spine from `docs/sitewide-brand-messaging-system.md` and rewrite section intros to connect each page back to fit, evidence and care.

### 2. Consumer and referrer audiences are mixed

The live `/referrals` page is currently mostly a form. It needs a referrer-facing landing layer above the form.

Recommendation:

Use `webflow/referrals-landing-webflow-embed.html` above the existing form. Keep "patient" language only on referrer pages and "client" language on consumer pages.

### 3. CTA language varies

The main CTA is usually "Book an appointment", but pages also use "Book online", "Talk to intake", "See upcoming programs", "Join our team" and form-specific actions.

Recommendation:

Create CTA rules:

- Client pages: `Book an appointment`.
- Service pages: `Book an appointment` plus `Meet the team`.
- Group pages: `See upcoming programs`.
- Referrer pages: `How to refer`, `Start online referral`, `Email intake`.
- Careers: `Join our team`.

## High-Priority Issues

### Careers page has placeholder content

The careers page includes generic headings and lorem ipsum-style content. This weakens trust and should be cleaned before broader brand work.

Fix:

- Remove placeholder sections.
- Keep recruitment copy focused on clinical independence, support, warmth and professional standards.

### Cancellation policy appears inconsistent

Fees content references a 24-hour cancellation/rescheduling policy. About FAQ references a 48-hour policy with partial/full fee wording.

Fix:

- Confirm the current policy operationally.
- Update all instances to one approved version.
- Check FAQ CMS pages if they repeat older wording.

### Contact emails differ

Observed patterns:

- Public footer uses `info@institute4healthyliving.com`.
- Referral content and referrer campaign use `intake@institute4healthyliving.com`.
- Live referrals schema/privacy text references `contact@institute4healthyliving.com`.

Fix:

- Decide official use by context:
  - General/public: `info@...`
  - Referrer/intake: `intake@...`
  - Avoid `contact@...` unless it is actively monitored.
- Update schema, forms and public copy.

### Hours and response claims need confirmation

Observed patterns include reception hours, consulting hours, Saturday availability and response timing. Some claims may be true in different contexts but should not conflict.

Fix:

- Define:
  - Reception hours.
  - Consulting hours.
  - Intake review hours.
  - Online/in-person availability.
  - Group program availability.
- Use conservative public phrasing where needed.

### CMS SEO titles/meta descriptions are incomplete

Concern and treatment sample pages use generic titles or blank descriptions.

Fix:

- Create a CMS formula for titles and descriptions.
- Example title formula: `[Concern] Psychologist Bondi Junction | IHL`.
- Example treatment title formula: `[Treatment] Therapy Bondi Junction | IHL`.
- Include online and in-person where appropriate.

## Page-Level Recommendations

### Home

Current role:

Brand promise and path into care.

Recommended emphasis:

- Right-fit clinician matching.
- Online and in-person care.
- Warm, evidence-based support.

Potential hero direction:

`Psychological care matched to you.`

### Team

Current role:

Therapist discovery and credibility.

Recommended emphasis:

- "Find your fit" should become the organizing idea.
- Filter labels are useful but should feel less mechanical.
- Clinician cards should use consistent title, focus areas, modalities and availability formatting.

### Offerings

Current role:

Service overview across adults, child/adolescent, couples, group therapy and assessments.

Recommended emphasis:

- Keep the service architecture.
- Bring each service back to fit, goals and evidence-based support.
- Use consistent CTA hierarchy.

### Fees and Rebates

Current role:

Practical policy clarity.

Recommended emphasis:

- Plain, precise, policy-led.
- Avoid soft brand flourishes here.
- Check rebate rates and cancellation policy before publishing updates.

### About

Current role:

Practice story, values and leadership.

Recommended emphasis:

- Keep the 2010 origin story and values.
- Correct spelling and older phrasing.
- Make "The Healthy Living Way" less slogan-heavy and more operationally clear.

### Referrals

Current role:

Clinical referral capture.

Recommended emphasis:

- Add landing sections before the form.
- Present all referral pathways.
- Keep clinical data boundary and emergency caveat.

### Get Support

Current role:

Conversion and booking pathway.

Recommended emphasis:

- Use this as the clearest "what happens when I enquire" page.
- Explain intake/matching briefly.
- Keep CTAs simple.

### Group Therapy

Current role:

Program-specific pathway.

Recommended emphasis:

- Keep program details current.
- Avoid listing programs that are not available.
- Make group entry criteria and next steps clearer.

### Cognitive Testing

Current role:

Assessment service page.

Recommended emphasis:

- Strong practical framing: assessment for clearer support planning.
- Confirm launch timing and availability before promoting.

### Concerns CMS

Current role:

Presenting-concern education and SEO.

Recommended emphasis:

- Add IHL-specific care pathway to each page.
- Use consistent structure:
  - What this can feel like.
  - How therapy can help.
  - How IHL matches care.
  - Online/in-person options.
  - CTA.

### Treatments CMS

Current role:

Modality education and SEO.

Recommended emphasis:

- Avoid implying modality fit before assessment.
- Use consistent structure:
  - What the modality is.
  - Who it may help.
  - How IHL uses it.
  - Talk to intake.

## Proposed Rewrite Order

1. Careers placeholder cleanup.
2. Referrals landing layer.
3. Global CTA and footer/contact cleanup.
4. Fees/About policy consistency.
5. Homepage hero and first two sections.
6. Get Support conversion page.
7. Team page intro and card consistency.
8. Offerings page intro and service cards.
9. Concerns CMS template.
10. Treatments CMS template.
11. Blog and FAQ cleanup.

## Open Decisions

- Current official cancellation policy.
- Current official reception and consulting hours.
- Approved general email and intake/referrer email.
- Whether "free 15-minute consultation" is still offered and who conducts it.
- Whether current rebate amounts should be shown dynamically or manually reviewed.
- Whether careers is active, paused or should be hidden until rewritten.
