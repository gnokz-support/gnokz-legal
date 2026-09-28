# Gnokz for Artists — public pages (Privacy Policy, Artist Terms, Delete your account)

Google Play needs two PUBLIC links (no sign-in): a **Privacy Policy** and a **Delete your account** page.
These pages are generated from the same text the app shows, so they always match:

    python3 tools/build_legal_pages.py

The folder has 4 pages side by side (no sub-folders, so an upload on the GitHub website cannot mix them up):

    index.html   privacy.html   terms.html   delete-account.html

## Put them online (GitHub Pages, free)

1. Open your public repository (e.g. `gnokz-legal`).
2. Delete any old `index.html` and the old `privacy/`, `terms/`, `delete-account/` folders if they are there.
3. Add file → Upload files → select the 4 `.html` files (not the folder, not README.md) → Commit changes.
4. Settings → Pages: Source "Deploy from a branch", Branch `main`, Folder `/ (root)`. Wait 1–2 minutes.
5. The links (example for account `gnokz-support`, repository `gnokz-legal`):
   - https://gnokz-support.github.io/gnokz-legal/privacy.html   ← Play: Privacy Policy
   - https://gnokz-support.github.io/gnokz-legal/delete-account.html   ← Play: Delete account URL
   - https://gnokz-support.github.io/gnokz-legal/terms.html
6. Open each link on your phone in a private tab to check it loads.

Only upload these pages. Never publish the app project, `docs/`, the Worker, keys or `.jks` files.
When the Privacy Policy or Terms change in the app, run the script again and upload the 4 files again.
