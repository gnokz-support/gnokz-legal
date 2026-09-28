# Gnokz for Artists — public pages (Privacy Policy, Artist Terms, Delete your account)

Google Play needs two PUBLIC links (no sign-in): a **Privacy Policy** and a **Delete your account** page.
These pages are generated from the same text the app shows, so they always match:

    python3 tools/build_legal_pages.py

## Put them online (GitHub Pages, free)

1. On github.com create a new PUBLIC repository, for example `gnokz-legal` (account `reymprime`).
2. Upload everything inside this `public_site/` folder (index.html, privacy/, terms/, delete-account/) to the root of that repository.
3. Repository → Settings → Pages → Source: "Deploy from a branch", Branch: `main`, Folder: `/ (root)` → Save.
4. After a minute the pages are live at:
   - https://reymprime.github.io/gnokz-legal/privacy/
   - https://reymprime.github.io/gnokz-legal/terms/
   - https://reymprime.github.io/gnokz-legal/delete-account/
5. Open each link on your phone (not signed in to GitHub) to check they load.

Only upload THIS folder. Never publish the app project, `docs/`, the Worker, keys or `.jks` files.
When the Privacy Policy or Terms change in the app, run the script again and upload the new files.
