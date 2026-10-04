# CountBy5 legal site

Static pages for the app's Privacy Policy and Terms of Use. They are not part of the Flutter build: this folder is not listed under `assets` in pubspec.yaml.

| File | Published URL |
|---|---|
| index.html | https://sofiane-amirouche.github.io/countby5/ |
| privacy.html | https://sofiane-amirouche.github.io/countby5/privacy.html |
| terms.html | https://sofiane-amirouche.github.io/countby5/terms.html |

The app opens the privacy and terms URLs from `lib/config/app_links.dart`.

## Support email

The pages list sofiane.amiro@gmail.com as the support contact, the same address as `lib/config/app_links.dart`. If you change it, change it in all of these places; the store compliance test pins the app's value.

## Publish with GitHub Pages

1. Sign in to GitHub as **Sofiane-Amirouche**.
2. Create a new repository: click **+** → **New repository**.
   - Repository name: `countby5`
   - Visibility: **Public** (GitHub Pages on a free account needs a public repo)
   - Tick **Add a README file** so the `main` branch exists.
   - Click **Create repository**.
3. Upload the pages: in the new repo, click **Add file** → **Upload files**, then drag in `index.html`, `privacy.html` and `terms.html` from this folder. They must go in the repository root, not in a subfolder. Click **Commit changes**.
4. Turn on Pages: go to **Settings** → **Pages**. Under **Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: **main**, folder **/ (root)**
   - Click **Save**.
5. Wait for the URL. After a minute or two, the Pages settings screen shows "Your site is live at https://sofiane-amirouche.github.io/countby5/". You can follow progress under the repo's **Actions** tab.
6. Test on a phone (both links):
   - Open https://sofiane-amirouche.github.io/countby5/privacy.html and https://sofiane-amirouche.github.io/countby5/terms.html in the phone's browser. Check that they load, are readable without zooming, and that the "Back to CountBy5" links work.
   - In the app, go to **Settings** and tap **Privacy Policy** and **Terms of Use**. Each should open the matching page.

## Updating later

Edit the files here, bump the "Effective date" line, then upload the changed files to the `countby5` repo again (**Add file** → **Upload files** replaces files with the same name). GitHub Pages redeploys automatically.
