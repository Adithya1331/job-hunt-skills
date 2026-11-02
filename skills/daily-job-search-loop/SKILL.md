---
name: Daily job search loop
description: Use this for a recurring job search: refresh the Naukri profile, find new matching jobs on LinkedIn and Naukri, dedupe them, apply to good fits, log them, and send a short summary.
---
# Daily job search loop

Run this on a schedule (a routine) or on demand. Work in the box browser with computerUse subagents, one at a time. The candidate's target roles, experience, locations, CTC, known answers and tracker live in memory and the routine prompt; read them there.

## 1. Naukri freshness edit
Make one small genuine daily edit using the **Naukri profile optimisation** skill, so the profile shows "updated today".

## 2. Search
Search LinkedIn and Naukri for postings from the **last 24 hours** that match the target roles, experience range, locations and CTC. Naukri's "1 day" filter is unreliable, so keep only listings marked 1 day ago. On LinkedIn, use the Jobs tab search; individual job pages can be flaky over the box network.

## 3. Dedupe
Drop anything already in the tracker (any status), anything already applied to, duplicates across sites, closed postings, and weak fits. Weak fits include experience far above the range, heavy focus on unrelated stacks (e.g. Java-only or ML research), or company-site-only applications for marginal roles.

## 4. Log new matches
Add each new match to the tracker as Shortlisted, with Role, Company, Location, Site, Link, Found On (today) and a short note on why it fits.

## 5. Apply
If the user has given standing permission, apply to the good fits using the **Job applications (LinkedIn and Naukri)** skill. If not, send the shortlist and wait for their yes. When a form needs an answer that isn't known, leave that job Shortlisted and ask.

## 6. Report
Send the user one short chat message: the jobs applied to (title, company, location, site, link), anything that needs an answer from them, and any notable skips. If nothing is new and nothing was applied to, send nothing.
