PULSE - online mode (Firebase)

SETUP (about 5 minutes, free tier is fine)
1. Go to console.firebase.google.com > Add project.
2. Build > Authentication > Get started > Sign-in method > enable "Anonymous".
3. Build > Firestore Database > Create database (production mode).
4. Firestore > Rules tab > paste the contents of firestore.rules > Publish.
5. Project settings > Your apps > Add web app (</>) > copy the config values into config.js.
6. Serve the folder over http(s) - NOT by double-clicking the file:
   - local test:  npx serve .   (or: python3 -m http.server)
   - public: Firebase Hosting, Netlify, Vercel or GitHub Pages (add your domain under
     Authentication > Settings > Authorized domains).

Until config.js is filled in, the app runs in offline mode (data saved in the browser only).
Each device gets an anonymous account; clearing browser data creates a new identity.
