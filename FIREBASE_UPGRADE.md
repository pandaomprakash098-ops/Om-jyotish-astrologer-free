# Optional Firebase upgrade

To make question/answer history shared across all devices:

1. Create a Firebase project.
2. Enable Firestore Database.
3. Add a Web App and copy its Firebase config.
4. Replace the localStorage persistence in `app.js` with Firestore calls.
5. Enable Firebase Authentication for the host dashboard.
6. Add Firestore security rules so only authenticated hosts can read all consultation records and users can read only their own records.

Do not publish a service-account private key or any server credential in GitHub.
