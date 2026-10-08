# Osa Travels — interactive enquiry-management trial

Live demo: https://gautamca.github.io/neeva-homes-trial/osa-travels/

Prepared by Silicon Soul for a prospective workflow discussion. Version 1.1.2.

## What works
Manual fictional enquiries, editable traveller/tour/date/stage details, quotation arithmetic in USD or CRC, printable example proposals, editable Spanish/English response drafts, clipboard copying, notes and activity, follow-up scheduling and completion, agenda, list and stage views, search/filtering, a live sample-data report, CSV export, local persistence, and restoration of eight original samples.

## Accuracy of the trial
All sample travellers and prices are fictional. Storage is local to one browser. Sources marked WhatsApp or Web are illustrative. The trial does not receive/send WhatsApp messages, share users/data across devices, verify availability, create actual reservations, collect payments, or convert currencies. A production implementation would require agreed workflows, authentication/permissions, shared backend storage, operational safeguards, and separately configured integrations.

## Audit and fixes — 8 October 2026
- Preserve drawer scroll and relevant focus when saving; suppress repeated entrance animation on section updates.
- Show navigation destinations immediately at the top of the page.
- Give the stage control a concise accessible label and a separate description.
- Validate nested saved data, actual calendar dates, finite nonnegative quotation amounts, supported currencies, unique IDs and record limits. Safely recover malformed storage.
- Preserve supported previous data versions; acknowledge the welcome screen when dismissed.
- Handle a closed/confirmed enquiry safely in the guided follow-up step.
- Make currency and source disclosures explicit; use English dates in English response drafts.
- Keep quotation totals and activity up to date after preparing a draft or printout.

## Verification
Run: `node osa-travels/verify.cjs`

Regression checks passed for JavaScript syntax, seed validity, calendar dates, quotation arithmetic, terminal stages, corrupted-storage recovery, empty data, duplicate IDs, version migration and HTML escaping.

The live interface was tested through manual creation of Familia Luna, four travellers, an example unit amount of USD95 plus USD20 adjustment (USD400 total), saved stage, tomorrow's follow-up, notes, copied response, printable proposal, downloaded CSV, agenda/report updates, search/stage views, persistence after reload, a 390px responsive viewport, closed-enquiry guided-tour handling and reset. The original eight samples were restored after testing. Browser-extension metadata errors were separate from application code.

Responsive QA viewport: https://gautamca.github.io/neeva-homes-trial/osa-travels/qa-mobile.html

## Showcase
The finished 62-second Spanish film begins with a clearly labelled illustrative WhatsApp enquiry, shows manual entry into the actual trial, quotation editing, follow-up, an editable reply, agenda and sample report, then ends with the exact live demo URL. It uses captured interface states with intentional editing, highlights and gentle camera movement. Instrumental music and interface sounds are original. No integration, booking, revenue or conversion results are invented.
