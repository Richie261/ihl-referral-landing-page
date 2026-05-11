# Launch Checklist

## Page Review

- Confirm HealthLink EDI is correct.
- Confirm phone and intake email are correct.
- Confirm referrer guide PDF link or replacement asset.
- Confirm services wording is clinically accurate.
- Confirm "what to include in referral" checklist is accurate and helpful.
- Confirm crisis/emergency caveat is clinically and legally appropriate.
- Confirm availability/funding caveat is present where needed.
- Confirm page works on mobile and desktop.

## Intake Readiness

- Confirm who owns HealthLink referrals.
- Confirm who owns online form referrals.
- Confirm acknowledgement timing for referrers.
- Confirm client contact timing.
- Confirm escalation criteria for Richie/Sathvika.
- Confirm reception script for redirecting referrals from `info@`, phone and fax into intake.

## Data Boundary

- Confirm what goes to intake.
- Confirm what goes to HubSpot.
- Confirm what must never go to HubSpot.
- Confirm campaign sequencing waits until HubSpot sync/contact contamination is controlled.
- Confirm patient/client names, DOB, referral reason, risk details and attachments do not enter marketing CRM.
- Confirm form attribution fields are limited to non-clinical campaign metadata.
- Confirm the final form does not send the full clinical submission to HubSpot.

## Publishing

- Use this GitHub Pages preview for internal review.
- Move approved copy/layout into Webflow.
- Remove the internal review console and internal strip before public Webflow launch.
- Keep `/referrals` canonical unless Max confirms `/refer` is preferable.
- Add `/refer` as a campaign-friendly redirect or alias.
- Publish Webflow page only after Sathvika/Max sign-off.
- Upload/replace GitHub files from `github-upload-ready` until direct GitHub write access is fixed.

## Max / Webflow

- Use `docs/webflow-max-handoff.md` as the implementation brief.
- Confirm the final secure referral form URL.
- Preserve UTM/source parameters from landing page to form.
- Test a dummy submission before campaign traffic starts.

## Source Of Truth

- Keep public landing page material in this repo.
- Keep Practice Brain, Tacklit/vendor, CRM and platform strategy in the strategy chat/master strategy docs.
- Keep old versions as archive; do not delete until the team confirms the new canonical file.
