# funding-management-system
Search for funders across South Africa, Russia, China, Brazil, and India with country/category filters and smart matching.

## Firebase setup
- Update the `firebaseConfig` object in `index.html` with your Firebase project settings.
- The app syncs to Firestore (collection: `funders`) when Firebase is configured. Without it, data is cached locally in the browser.
