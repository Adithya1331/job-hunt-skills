---
name: Job application tracker (Notion)
description: Use this when logging or updating job applications in a Notion tracker database: adding shortlisted jobs, marking them applied, and querying for dedupe.
---
# Job application tracker (Notion)

Use the Notion connector. Find the tracker database by name (commonly "Job Applications") and work with its data source.

## Schema (typical)
- **Role** (title)
- **Company**, **Location**, **Site** (LinkedIn / Naukri)
- **Status**: Shortlisted, Applied, Interview, Offer, Rejected
- **Salary**, **Experience**
- **Link**: the property key is `Link`
- **Found On**, **Applied On** (dates, YYYY-MM-DD)
- **Notes**

If the schema differs, read it first and map the fields. Don't create a second tracker.

## Add a shortlisted job
Create a row with Role, Company, Location, Site, Link, Status Shortlisted, Found On set to today, and a one-line note on why it fits or any caveat.

## Mark applied
Set Status to Applied and Applied On to the date it was submitted. Add anything unusual to Notes, such as a closed posting, a pre-filled answer, or a follow-company box that couldn't be unticked.

## Other statuses
- Posting closed or no longer accepting applications: Rejected, with the reason in Notes.
- Skipped as a weak fit: keep it Shortlisted with the reason, or leave it out.

## Dedupe before adding
Query the data source for the company and role, or the link, and skip anything already there in any status.

## Reporting
When asked, query by Status (e.g. all Applied this week) and return a short list with links to the Notion pages.
