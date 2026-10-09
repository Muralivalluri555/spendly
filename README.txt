SPENDLY — OFFLINE IPHONE WEB APP

WHAT THIS DOES
- Installable Home Screen web app for iPhone.
- After the first successful online visit, its app shell is cached for offline opening.
- Expense names and amounts are saved in browser local storage on this device.
- Clear Total resets only the running total; the saved item list remains.
- No account, backend, or database is required.

IMPORTANT
A secure HTTPS URL is required for reliable service-worker/offline support. You only need to publish the static files once; hosting is not needed to use the app after its files are cached, but the URL should remain available for reinstalling and updates.

FREE PUBLISHING WITH GITHUB PAGES (WINDOWS)
1. Extract this ZIP.
2. Sign in to GitHub and create a NEW repository named spendly (Public is simplest for GitHub Free Pages).
3. Choose Add file > Upload files and upload ALL files from this folder. Ensure index.html is at the repository root, not inside an extra folder.
4. Commit the upload.
5. Open the repository Settings > Pages.
6. Under Build and deployment, choose Deploy from a branch; select branch main and folder /(root), then Save.
7. Wait a few minutes. The site URL will look like https://YOUR-GITHUB-USERNAME.github.io/spendly/ . Replace YOUR-GITHUB-USERNAME with your actual GitHub username.
8. Open that URL in Safari on your iPhone while online and wait for the page to load fully once.
9. In Safari tap Share > Add to Home Screen. Turn on Open as Web App if shown, then tap Add.
10. Open Spendly once while still online after adding it, then test Airplane Mode. If it opens offline, you are ready.

PRIVACY / DATA
The website is static, but GitHub Pages serves the public files and may log normal website access. Expense entries are stored in local browser storage on this iPhone and are not sent to a Spendly server. They are device/browser-specific; clearing website data or removing app data can erase them. Keep a separate backup if the records matter.

UPDATING
To update the app, upload changed files to the same repository. If a service worker update is delayed, close Spendly fully and reopen it while online. The cache version can be changed in sw.js (spendly-shell-v1) for a forced cache refresh.
