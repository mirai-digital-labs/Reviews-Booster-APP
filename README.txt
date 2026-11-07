FRI-CHICKS JHANG — QR OWNER PRESENTATION BUILD

WHAT IS INCLUDED
- Responsive owner-facing dashboard and customer feedback experience.
- English, Urdu and Roman Urdu interface options.
- Real QR code image generation for each campaign (QRCode.js loaded from cdnjs).
- Campaign QR links encode this site's deployed URL with ?campaign=CAMPAIGN_ID.
- QR PNG download and copy-link actions.
- Customer QR link opens a clean customer-only page (no owner sidebar).
- Feedback, branch/campaign editing, complaint status changes and CSV export.
- Browser-local persistence for demonstration.

DEPLOY TO CLOUDFLARE PAGES (STATIC PREVIEW)
1. Create a GitHub repository, e.g. fri-chicks-jhang.
2. Upload index.html and _headers from this folder to the repository root.
3. Cloudflare Dashboard > Workers & Pages > Create > Pages > Connect to Git.
4. Select the repository. Framework preset: None. Build command: leave blank. Build output directory: / (root).
5. Deploy. Open the Cloudflare Pages URL, then open QR Campaigns.
6. Download each QR PNG from the deployed domain. Do not print QR codes generated from localhost or file:// URLs.

IMPORTANT — CURRENT BUILD LIMITATIONS
This is a working front-end presentation prototype, NOT a production multi-user SaaS backend.
- Feedback and settings are stored in each visitor's own browser localStorage. A customer's submission will NOT appear in the owner's browser/dashboard on another device.
- There is no secure owner login, shared database, server-side branch permissions, backups, audit log or server-side rate limiting.
- The QR codes are real and scannable, but their links lead to this front-end-only demo.
- Google Business Profile is not connected. A verified branch-specific Google review URL must be configured before it can open a real review page. No review submission is asserted.
- Email/WhatsApp/SMS notifications are not connected.
- Demo records in the dashboard are illustrative and should be cleared/replaced before any customer-facing pilot.

BEFORE ACCEPTING REAL CUSTOMER FEEDBACK
Add a backend (e.g. Cloudflare Pages Functions + D1), owner authentication, role/branch authorization, input validation, abuse controls, backups, privacy notice/retention policy, monitoring and tests. Configure each branch's official Google review URL. Verify Google Business Profile API access separately if live review synchronization/replies are required.

GOOGLE POLICY
Every customer must receive the same neutral invitation to leave an honest Google review regardless of private feedback rating. Do not gate reviews, offer review incentives, or create fake reviews. Internal feedback is separate from public Google reviews. A click is not proof that a Google review was submitted.
