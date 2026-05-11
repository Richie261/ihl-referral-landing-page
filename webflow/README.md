# Webflow Transfer

Use `referrals-landing-webflow-embed.html` as the direct transfer artifact.

Active priority: the referrer landing page. Broader site-wide brand cleanup is parked until this page is approved.

Recommended placement:

1. Open the live Webflow `/referrals` page.
2. Keep the existing Webflow nav and footer.
3. Paste the embed above the current GP referral form embed.
4. Upload `assets/ihl-referrer-guide.pdf` to Webflow assets.
5. Replace `REFERRER_GUIDE_URL` with the uploaded PDF asset URL.
6. Keep online form CTAs pointing to `#gp_referral_form` if the form remains on the same page.

The embed uses `rf-` prefixed classes so it should not conflict with existing Webflow classes.

For the wider site cleanup, use `sitewide-brand-update-checklist.md` alongside:

- `docs/sitewide-brand-messaging-system.md`
- `docs/sitewide-website-audit.md`
- `sitewide-unified-preview.html`
