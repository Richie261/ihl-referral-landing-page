# Decisions

## Current Direction

- The referrer landing page is the active priority. Broader site-wide brand work is useful background, but not the current build focus.
- The page should now be form-first. The public experience is a simple, professional and warm gateway into the referral form, not a full landing-page brochure.
- The form should prioritise patient contact details first: name, date of birth, mobile, email, preferred contact and guardian details where relevant.
- The form should allow signed referral letters, Mental Health Treatment Plans, specialist referrals, Medicare plans, insurance/workplace documents and reports to be uploaded without forcing referrers to duplicate the same content.
- Public copy should not imply that a Mental Health Treatment Plan alone is the referral; it is a supporting document unless paired with a written referral.
- Referrer details should stay minimal but sufficient to identify the referrer, contact them, and support referral validity where the online form itself is used as the referral.
- The page should feel like a calm professional referral reference, not a sales funnel or guided tour.
- Avoid numbered process cards and heavy explanatory blocks unless they are required for clinical safety or form completion.
- HealthLink EDI `inshealh` must remain easy to find and copy.
- The online form, intake email, phone and fax should be presented as available referral options.
- HubSpot should be treated as referrer/campaign CRM only unless a separate data policy approves otherwise.
- Clinical referral details should not be placed into marketing systems by default.
- Campaign attribution can be captured as hidden non-clinical metadata and passed to HubSpot only as referrer relationship/source data.
- The public page can include a "what to include in referral" checklist because it improves referral quality without exposing internal operating detail.
- Emergency/crisis wording must remain conservative: this is a routine referral pathway, not an acute-risk pathway.
- `/referrals` is the recommended canonical page, with `/refer` as a short campaign alias or redirect unless Max confirms a better live-site constraint.

## Review Notes

- Sathvika to review intake logic and operational fit.
- Sathvika to review crisis/risk wording before public launch.
- Max to keep the Webflow implementation simple and avoid overbuilding the first release.
- Max to remove internal review sections from the GitHub prototype before Webflow public launch.
- Team to confirm acknowledgement, escalation, and intake ownership rules before launch.
- Team to confirm whether the referrer guide is a direct download or "request guide" action.

## Feed Back To Strategy Chat

- Clinician matching logic as IHL IP.
- Future Practice Brain/internal console implications.
- Custom layer versus Tacklit/Halaxy/Webflow boundaries.
- HubSpot contamination controls and source-of-truth governance.
