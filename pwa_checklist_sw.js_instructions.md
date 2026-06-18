# PWA Checklist for GitHub Pages

To make your BTS News Stream app a fully functional Progressive Web App (PWA) on GitHub Pages, ensure the following files are in your repository's root:

## 1. manifest.json
This file tells the browser about your web app and how it should behave when 'installed' on a mobile device or desktop.
- **Action**: Save the generated `manifest.json` to your root.
- **HTML Link**: Add `<link rel="manifest" href="/manifest.json">` to the `<head>` of all your HTML files.

## 2. Service Worker (sw.js)
The service worker handles offline caching so the app works without an internet connection.
- **Action**: Save the generated `sw.js` to your root.
- **Registration**: Add this script before the closing `</body>` tag in your `index.html`:
  ```javascript
  if ('serviceWorker' in navigator) {
    window.addEventListener('load', () => {
      navigator.serviceWorker.register('/sw.js');
    });
  }
  ```

## 3. App Icons
You'll need a few icon sizes (192x192 and 512x512).
- **Tip**: You can use the "ARMY Hub" logo generated earlier or I can create dedicated app icons for you.

## 4. HTTPS (Auto-handled)
GitHub Pages provides HTTPS by default, which is a strict requirement for PWAs. Ensure "Enforce HTTPS" is checked in your GitHub Repository Settings > Pages.

## 5. Deployment Note
When hosting on GitHub Pages, if your repository is named `my-repo`, your URLs might look like `username.github.io/my-repo/`. Ensure your paths in `manifest.json` and `sw.js` account for this subfolder if applicable.