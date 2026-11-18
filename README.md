# Free local workflow preflight tools

Browser-local checks for developers and automation operators. Try real synthetic inputs without an account before deciding whether a hosted API is useful. I maintain these tools; development and documentation are AI-assisted.

## Runnable n8n example

Download [workflow.json](workflow.json), inspect its Code node, import into an inactive workflow and run the manual trigger. Native import and execution verified in n8n 2.46.6. No credentials or HTTP nodes. Two synthetic cases show a JSON /status change (ignoring /updatedAt) and a one-unit order/shipment discrepancy. This tutorial is not an approved n8n library template.

## Choose a local checker

| Tool | Use case | Free trial | Optional hosted API |
|---|---|---|---|
| Subtitle Relay | Convert SRT subtitle files to WebVTT locally. Check a free batch example, then automate caption conversion with the Subtitle Relay API. | [Open local checker](https://caption-toolkit.mayasmile.workers.dev/) | [Plans](https://rapidapi.com/didyouseethis212sys/api/subtitle-relay/pricing) |
| JSON Change Relay | Compare JSON snapshots locally, find added, removed and changed fields, and ignore selected JSON Pointer paths. Free checker and recurring API plans. | [Open local checker](https://json-change-relay.mayasmile.workers.dev/) | [Plans](https://rapidapi.com/didyouseethis212sys/api/json-change-relay/pricing) |
| Calendar File Relay | Generate an ICS calendar from 1–25 events with UTC times and optional stable event IDs. Free browser-local generator and hosted automation API. | [Open local checker](https://calendar-file-relay.mayasmile.workers.dev/) | [Plans](https://rapidapi.com/didyouseethis212sys/api/calendar-file-relay/pricing) |
| Redirect Map Guard | Review a Shopify migration redirect CSV before import. Detect loops and conflicts, flatten safe chains and export a two-column CSV for review. | [Open local checker](https://portfolio-tools-relay.mayasmile.workers.dev/redirect-map-guard) | [Plans](https://rapidapi.com/didyouseethis212sys/api/redirect-map-guard/pricing) |
| Order Reconciliation Relay | Compare order and dispatch CSV quantities by order ID and SKU. Aggregate split rows and return missing, short or excess quantities with a CSV discrepancy report. Filter input scope before use. | [Open local checker](https://portfolio-tools-relay.mayasmile.workers.dev/order-reconciliation-relay) | [Plans](https://rapidapi.com/didyouseethis212sys/api/order-reconciliation-relay/pricing) |
| Catalog Import Guard | Shopify product CSV validation with row-level reports and an approved n8n template. | [Open local checker](https://catalog-import-guard.mayasmile.workers.dev/try) | [Plans](https://rapidapi.com/didyouseethis212sys/api/catalog-import-guard/pricing) |
| mail-auth-change-guard | Compare DMARC XML report batches locally. Find newly failing sources, failure-rate changes and repeated reports. Free checker and hosted recurring API. | [Open local checker](https://mail-auth-change-guard-trial.mayasmile.workers.dev/) | [Plans](https://rapidapi.com/didyouseethis212sys/api/mail-auth-change-guard/pricing) |
| webhook-effect-guard | Compare webhook delivery logs with durable workflow effects. Separate normal retries from missing or duplicate effects. Free local JSON audit and recurring API. | [Open local checker](https://webhook-effect-guard.mayasmile.workers.dev/) | [Plans](https://rapidapi.com/didyouseethis212sys/api/webhook-effect-guard/pricing) |
| open-contract-guard | Check selected consumer response fields against proposed OpenAPI changes. Flag watchlist breaks and explicit incomplete coverage. Free local JSON trial and hosted API. | [Open local checker](https://open-contract-guard.mayasmile.workers.dev/) | [Plans](https://rapidapi.com/didyouseethis212sys/api/open-contract-guard/pricing) |

## Free versus hosted

The local checks remain free. The first six tools offer BASIC 100 hosted requests/month free and PRO $5/month for 1,000. Mail Auth, Webhook Effect and Open Contract offer BASIC 25 free requests/month and PRO $9/month for 500. Hard request limits apply; RapidAPI platform bandwidth fees and terms are separate. Follow the current plan page before subscribing.

No API subscription is needed for the local example. An existing script or library may be sufficient. Hosted calls receive the input sent to the API; sanitize it and keep your own credentials private.

## Scope

These tools review supplied inputs. They do not write to stores, send messages, repair webhook queues, import calendars or establish financial truth. Order CSVs require matching export scopes and exclude cancellations/refunds/out-of-scope rows. OpenAPI checks cover selected fields, not the entire specification. DMARC changes are review signals, not proof of spoofing or delivery failure. Review each checker's stated limits.

All example results are synthetic validation, not customer outcomes, traffic or sales. No guaranteed compatibility, savings, search ranking or revenue is claimed.
