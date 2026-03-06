# funding-management-system
Deep-scan funding intelligence (200 funders) and contract/service leads (100 opportunities) across South Africa, Russia, China, Brazil, and India with mode switching, sector filters, and smart matching.

## Firebase setup
- Update the `firebaseConfig` object in `index.html` with your Firebase project settings.
- The app syncs to Firestore (collection: `funders`) when Firebase is configured. Without it, data is cached locally in the browser.
