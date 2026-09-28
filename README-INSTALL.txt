RAJ ONLINE CENTRE — INSTALLABLE ANDROID WEB APP FILES

Your existing published website remains the main app. These files add installability (PWA) and offline caching.

IMPORTANT: The website currently uses a GitHub Pages project URL:
https://caamit002-cmyk.github.io/Raj-online-center/

HOW TO ADD THESE FILES ON GITHUB (phone):
1. Open your repository: https://github.com/caamit002-cmyk/Raj-online-center
2. Tap Add file > Upload files.
3. Upload manifest.webmanifest, sw.js, icon-192.png, icon-512.png.
4. You must also update index.html to include the PWA tags and service worker registration. See the exact snippet below and add it before </head> and before </body> respectively.

Inside <head>, before </head>:
<link rel="manifest" href="./manifest.webmanifest">
<meta name="theme-color" content="#075985">
<link rel="apple-touch-icon" href="./icon-192.png">

Before </body>:
<script>
if ("serviceWorker" in navigator) {
  window.addEventListener("load", () => {
    navigator.serviceWorker.register("./sw.js").catch(console.error);
  });
}
</script>

5. Commit changes directly to main.
6. Wait a few minutes, then open your site in Chrome:
https://caamit002-cmyk.github.io/Raj-online-center/
7. Chrome menu (three dots) > Add to Home screen or Install app.

This creates an installable web app on Android. It is not a signed standalone APK. Publishing a Play Store app or creating a signed APK requires a separate Android build/signing process.
