TRUCK OR SHOP? — standalone app files
=====================================

These files run on their own. 

  settings.js            THE FILE YOU EDIT: donation link, prices, date
  index.html             the app itself (no need to touch)
  manifest.webmanifest   makes it installable
  sw.js                  makes it work offline
  icon-*.png             app icons


EDITING IT YOURSELF (recommended setup: GitHub Pages, free)
-----------------------------------------------------------
One-time setup, about 15 minutes:
  1. Make a free account at github.com.
  2. Tap + > New repository. Name it truck-or-shop, set it to Public,
     tick "Add a README", and create it.
  3. Tap Add file > Upload files and upload everything in this folder
     (unzipped). Tap Commit changes.
  4. Go to Settings > Pages. Under "Branch" choose main, then Save.
     After a minute or two your app is live at:
         https://YOUR-USERNAME.github.io/truck-or-shop/

To change a price, add a product, or add your donation link later:
  1. Open your repository on github.com (works in a phone browser).
  2. Tap settings.js, then the pencil icon (Edit).
  3. Change what you need, then tap Commit changes.
  The live app updates within a couple of minutes.

Tips for editing settings.js:
  - Each product is one line:   Name|Where it's made|Unlock level|Max price
  - Keep the quote marks "" around the donation link and the date.
  - Keep the backtick ` at the start and end of the product list.
  - If the app ever shows no products after an edit, a | or ` was
    probably deleted by accident. GitHub's History button lets you
    restore the previous version.


DONATIONS
---------
  1. Make a free Ko-fi (ko-fi.com) or Buy Me a Coffee page.
  2. Paste your page link into DONATE_URL in settings.js.
  The button only appears on the website. It hides itself inside a
  Google Play version, because Google Play doesn't allow individuals
  to ask for donations inside an app.
  Supercell's Fan Content Policy allows donations only if they are
  purely donations: never unlock features or extras for donors.


INSTALL ON YOUR PHONE
---------------------
  Open your web address in Chrome (Android) or Safari (iPhone).
  Android: menu > Install app.   iPhone: Share > Add to Home Screen.
  It opens full-screen and works offline after the first visit.


GOOGLE PLAY (optional)
----------------------
  1. Go to pwabuilder.com, paste your web address, choose
     Package for stores > Android. Download the package and keep the
     signing key safe (you need it for every update).
  2. Upload the assetlinks.json file PWABuilder gives you into a
     folder called .well-known in your repository.
  3. Create a Google Play Console developer account (one-time fee).
  4. New personal accounts must run a closed test with at least 12
     testers opted in for 14 days in a row before going public.
  5. You'll need a privacy policy page. The app only stores data on
     the user's own phone, so say that.
  Price edits on GitHub also reach the Play version automatically,
  because it loads your website.

Keep the app free. Don't put "Hay Day" in the store name or icon;
describe it as "an unofficial helper for Hay Day players" instead.
Keep the disclaimer at the bottom of the app.
