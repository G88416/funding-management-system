# funding-management-system
Deep-scan funding intelligence (400 funders) and contract/service leads (200 opportunities) across South Africa, Russia, China, Brazil, and India with mode switching, sector filters, and smart matching.

The search engine now includes Navboost-inspired ranking that learns from user clicks, dwell time, and query variants over a rolling 13-month window to continuously re-rank results.

## Firebase setup
- Update the `firebaseConfig` object in `index.html` with your Firebase project settings.
- The app syncs to Firestore (collections: `funders`, `contractLeads`, `searchIndexes`, `navboostSignals`) when Firebase is configured. Without it, data runs in-memory from the seed dataset only.
