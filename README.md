# funding-management-system
Search results intelligence engine that explains how crawling, understanding, retrieval, scoring, and re-ranking combine to improve relevance across contexts.

The search engine now includes Navboost-inspired ranking that learns from user clicks, dwell time, and query variants over a rolling 13-month window to continuously re-rank results.

## Firebase setup
- Update the `firebaseConfig` object in `index.html` with your Firebase project settings.
- The app syncs Navboost signals and search state to Firestore (collections: `navboostSignals`, `searchState`) when Firebase is configured. The search pipeline guidance stays in-memory and is rebuilt for every query.
- Deploy the Firestore and Storage security rules from this repo using the Firebase CLI (`firebase deploy --only firestore:rules,storage:rules`), which reads `firebase.json`.
- Firestore rules require authenticated users with the `admin` custom claim for analytics collections.
- Storage rules require authenticated admin access for all paths.
