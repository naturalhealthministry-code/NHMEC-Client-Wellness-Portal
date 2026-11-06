# NHMEC Client Wellness Portal — interactive prototype

This is an **offline-capable, single-file, fictional-data demonstration** for Natural Health Ministries Education Center (NHMEC). It is intentionally separate from the existing NHMEC Herbalist Learning App.

## Open and test

1. Download the `index.html` file and open it in a modern desktop or mobile browser; no account or installation is required.
2. Use the **Client view / Practitioner view** toggle.
3. In Client view, read the current wellness plan, open the Fullscript placeholder, write a journal entry, and complete a 14-day check-in.
4. In Practitioner view, select a fictional client, update their sample plan, reply in the journal, and review check-ins.
5. Switch back to Client view to verify the changes. Click **Reset demo data** in the practitioner dashboard when finished.

**Only two entirely fictional sample clients are included.** Browser localStorage retains demo edits only in the browser where you made them. Client/Practitioner toggles are not authentication. This prototype has **no server-side access restrictions, secure storage, audit logs, encrypted backend, appointment system, real Fullscript cart, or actual PDF uploads.** Do not enter actual client names, wellness plans, messages, health information, or Fullscript links.

## Put the demonstration on GitHub Pages (optional)

1. Create a **separate** GitHub repository named `nhmec-client-portal-demo`, without changing the existing NHMEC Herbalist Learning App repository.
2. Upload `index.html` to the root of the new repository and commit it to the default (`main`) branch.
3. In the new repository, navigate to **Settings → Pages** and select **Deploy from a branch**, `main`, `/ (root)`. Save.
4. Once GitHub provides the Pages URL, open it to test on a phone or computer.

**GitHub Pages serves public website files, not authenticated client data.** Publishing this fictional demo is fine; publishing a genuine client portal with health information to it **without an independently secured application/backend would not be safe**. GitHub itself is for the application code, never private client records.

## What a production system needs

- Real email/password or passwordless login with MFA capability.
- Verified permissions ensuring each client sees only their own plan, journal, and check-in data, and your practitioner role can access authorized clients.
- Protected plan file storage for exported Canva / Google Docs PDFs.
- Secure journal/check-in storage, backups, practitioner notifications, audit logs, file scanning if uploads added.
- Privacy/compliance assessment (including whether HIPAA applies), appropriate contracts and providers, consent and retention policies.
- Optional secure Fullscript personal-link storage and account workflows.
- Security testing before use with real health information. Any backend or service used needs suitability review; a free tier is not automatically acceptable for health records.

## Current demo scope

- Responsive client dashboard with four sections: Current Wellness Plan, Fullscript, Private Journal, and Two-Week Check-In.
- Practitioner dashboard with fictional client roster, editable plan, journal replies, and check-in review.
- Current plan displayed natively, with sample Perspective / Essence / Nutrition sections; no real files embedded.
- Each check-in includes P/E/N ratings, progress update, optional question, and a next-due date 14 days later.

Version: Prototype 1 (fictional records, no network dependency beyond optional Fullscript homepage).
