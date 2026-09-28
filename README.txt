# Raj Online Centre app

This is a mobile-friendly installable web app (PWA) prototype.

## Run on your phone
1. Extract this ZIP.
2. Upload the files to a static host (for example GitHub Pages or Netlify) so they are served over HTTPS.
3. Open the published URL in Chrome on Android.
4. Tap Chrome menu (⋮) → Install app or Add to Home screen.

## WhatsApp setup
Open `index.html` in a text editor and find:
`const SHOP_WHATSAPP = "8271526030";`
Replace it with the shop's WhatsApp number including country code, digits only. For India, use 91 followed by the 10-digit number (example format: 919876543210).

## Notes
- This package is a working web app/PWA starter, not a signed APK.
- Booking enquiries open WhatsApp; no payments or customer database are configured.
- Add your actual shop address, prices, opening hours, and photos before publishing.
- Avoid collecting or sending OTPs, passwords, or sensitive identity details through the enquiry form.
