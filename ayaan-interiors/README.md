# Ayaan Interiors — Enquiry Studio

Client concept prepared independently by Silicon Soul for Ayaan Interiors.

Live demo: https://gautamca.github.io/neeva-homes-trial/ayaan-interiors/

## Trial journey

Explore sample flow → fictional WhatsApp enquiry → review and add manually → assign a sample designer → schedule a discovery call/site visit → complete consultation → edit an indicative LKR quotation → review/print the saved quotation → mark shared manually → schedule follow-up → review and copy a reply → inspect the agenda and studio metrics.

## Working functionality

- Manual enquiry capture, search, stage filter and list/board views.
- Sample designer assignment, notes and activity history.
- Consultation and follow-up scheduling in Asia/Colombo time.
- Project-specific editable quotation starters, line items, discount/tax arithmetic, saved revisions and printable quote content.
- Manual share recording and copyable, editable response drafts.
- Counts and values calculated from the current records.
- CSV generation, browser-local persistence, validated recovery and sample reset.
- Phone-width responsive layout and keyboard dialog focus handling.

## Accurate scope

All records, staff labels, dimensions, prices and results are fictional. Prices do not represent Ayaan’s actual rates. This is a browser-local demonstration. There is no authentication, shared production database, live WhatsApp connection, file upload, automated notification, automatic sending, payment collection, calendar integration or production order system. The initial conversation is illustrative; information is added through a manual action. Do not enter confidential client data.

A live implementation and any WhatsApp Business API connection require a separate agreed scope, implementation, configuration and acceptance.

## Validation

Run `node verify.cjs` alongside `index.html` (or from the local project with `dist/index.html`). Checks cover sample validity; project quotation starters; rounding, discount and tax arithmetic; leap-day/year boundaries; invalid records/quotes; terminal reminders; HTML and CSV escaping; long notes; corrupt storage; duplicate IDs; and schema version handling.

Browser QA exercised manual capture, assignment, consultation scheduling/completion, quotation editing and saving, generated print content, manual share status, copyable reply text, follow-up agenda, list search/board, terminal reminder cleanup, reload persistence and reset/guide restoration. The quotation editor was tested at 390px width without horizontal overflow. CSV download was triggered successfully in-browser. A separate check captures the actual CSV generator bytes and verifies headers, row counts and saved quotation amounts. The browser download bridge did not expose its downloaded file bytes.

Public process reference: https://ayaaninterior.com/services — discovery call, site visit, design proposal and quotation. This is an independently prepared concept, not a claim of endorsement.

Deployment adds only the Ayaan folder to the existing repository. Neeva and Osa trials are unchanged.
