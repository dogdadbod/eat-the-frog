# Eat the Frog! app

A private daily journal for the Eat the Frog strategy. Students pick a frog, check in, and earn streak badges. Entries are saved only on the student's own phone. There are no accounts and no server.

## Files

| File | What it is |
|---|---|
| `index.html` | The app |
| `manifest.webmanifest` | Tells phones the app's name, icon and full-screen mode |
| `sw.js` | Offline helper, so the app opens without internet |
| `icon-180.png` | iPhone home screen icon |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` | Android home screen icons |

## Put it on GitHub Pages

1. Sign in at github.com and click **New repository**. Name it something short, such as `eat-the-frog`. Set it to **Public**, then click **Create repository**.
2. On the new repository page, click **uploading an existing file**. Drag in all the files from this folder (not the folder itself), then click **Commit changes**.
3. Open **Settings → Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main**, folder **/ (root)**, then click **Save**.
4. Wait a minute or two and refresh the page. Your web address appears at the top, for example `https://yourname.github.io/eat-the-frog/`.
5. Open that address on your phone to check it works.

## Tell students

1. Scan the QR code (or open the link) **in Safari on iPhone or Chrome on Android**.
2. Add it to the home screen:
   - **iPhone:** tap Share, then **Add to Home Screen**.
   - **Android:** tap the ⋮ menu, then **Add to Home screen** or **Install app**.
3. **Always open the app from the home screen icon.** On iPhone, the home screen app keeps its own saved journal, separate from Safari.
4. Set the daily reminder on the Today tab.

## Updating the app later

Upload the new `index.html` over the old one. Then open `sw.js` on GitHub, change `eat-the-frog-v1` to `eat-the-frog-v2` (then v3, and so on), and commit. Students get the update the next time they open the app with internet. Their journal entries are not affected.

## Good to know

- Students' journals live only on their phones. Clearing browser data, deleting the home screen icon on iPhone, or switching phones removes the journal unless they use **Help → Back up your journal** first.
- The Google Calendar button sends only the reminder title and time to Google, and only when tapped.
