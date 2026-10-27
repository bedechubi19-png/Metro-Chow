# Metro Chow — Food Delivery PWA

A mobile-first Progressive Web App prototype for Metro Chow, a Calabar food-delivery service sourcing meals from Smookies and using local dispatch.

## Included
- Visual meal catalogue with categories, search, prices and stock status
- Cart and checkout with all seven supplied delivery zones/fees
- Order confirmation, order history, status and four-digit pickup code
- Admin dashboard (demo PIN `2468`) with daily order revenue, active orders, customer phone/address, rider pickup codes, product add/edit, image URL and stock controls
- Support chatbot with human-escalation messaging and feedback/complaints form
- Local browser storage and service-worker caching for PWA behavior

## Run locally
Serve this folder over localhost or HTTPS (service workers do not run from `file://`):
- Python: `python -m http.server 8000`
- Open `http://localhost:8000`

## Important before real launch
This is a front-end prototype. Data is stored in the current browser/device only. The admin PIN is a demo convenience, not secure authentication. Orders, reviews and complaints are not sent to a server; no real-time rider dispatch, SMS/WhatsApp alerts, live human support or online payments are connected. For production, add a secure backend/database, server-side admin auth, payment provider, verified Smookies catalogue/images, dispatch workflow and privacy/security controls.

## Pricing assumptions
The provided prices are shown as selling prices. For Rice/Pasta, the initial `cost` field is set to listed price minus ₦500 to reflect the requested +₦500 markup. Protein/side and drink cost fields initially equal the listed price because no separate supplier costs were supplied; replace these with actual Smookies costs in admin before using profit metrics.
