# PWA Image Requirements for Aid Migraine App

This guide lists all the image files you need to create for a complete Progressive Web App experience.

## Color Scheme
Based on the images you've provided and the app design:
- Primary: Purple/Violet (#7b1fa2, #4a148c)
- Background: Purple gradient
- Icon: White brain/head silhouette with wave elements

---

## 📱 Required PWA Icons (manifest.json)

### Standard Icons
Create these PNG files in the `/icons/` directory:

- **icon-72x72.png** - 72×72px
- **icon-96x96.png** - 96×96px
- **icon-128x128.png** - 128×128px
- **icon-144x144.png** - 144×144px
- **icon-152x152.png** - 152×152px
- **icon-192x192.png** - 192×192px ⭐ (Required for PWA)
- **icon-384x384.png** - 384×384px
- **icon-512x512.png** - 512×512px ⭐ (Required for PWA)

### Maskable Icons (for Android)
These should have extra padding (safe zone) for adaptive icons:

- **icon-192x192-maskable.png** - 192×192px with safe zone
- **icon-512x512-maskable.png** - 512×512px with safe zone

**Safe zone guidance**: Keep important content within the center 80% circle (40% radius from center).

---

## 🍎 Apple Touch Icons

Create these PNG files with NO transparency (solid background):

- **apple-touch-icon-120x120.png** - 120×120px (iPhone)
- **apple-touch-icon-152x152.png** - 152×152px (iPad)
- **apple-touch-icon-167x167.png** - 167×167px (iPad Pro)
- **apple-touch-icon-180x180.png** - 180×180px (iPhone Retina)

---

## 🖼️ Favicons

- **favicon.ico** - 16×16, 32×32, 48×48 (multi-size .ico file)
- **favicon-16x16.png** - 16×16px
- **favicon-32x32.png** - 32×32px

---

## 📲 iOS Splash Screens (Portrait)

Create these splash screens with your app branding centered on a purple gradient background:

### iPhone (Modern)
- **splash-2796x1290.png** - 2796×1290px (iPhone 14 Pro Max, 15 Pro Max)
- **splash-2556x1179.png** - 2556×1179px (iPhone 14 Pro, 15 Pro)
- **splash-2778x1284.png** - 2778×1284px (iPhone 12/13/14 Pro Max)
- **splash-2532x1170.png** - 2532×1170px (iPhone 12/13/14 Pro)
- **splash-2436x1125.png** - 2436×1125px (iPhone X, XS, 11 Pro)
- **splash-2688x1242.png** - 2688×1242px (iPhone XS Max, 11 Pro Max)
- **splash-1792x828.png** - 1792×828px (iPhone XR, 11)
- **splash-1334x750.png** - 1334×750px (iPhone 8, 7, 6s)
- **splash-2208x1242.png** - 2208×1242px (iPhone 8 Plus, 7 Plus, 6s Plus)
- **splash-1136x640.png** - 1136×640px (iPhone SE, 5s)

### iPad
- **splash-2048x1536.png** - 2048×1536px (iPad 9.7", iPad Mini)
- **splash-2224x1668.png** - 2224×1668px (iPad Pro 10.5")
- **splash-2388x1668.png** - 2388×1668px (iPad Pro 11")
- **splash-2732x2048.png** - 2732×2048px (iPad Pro 12.9")

---

## 📸 Screenshots (for App Stores & Install Prompts)

- **screenshot-wide.png** - 1280×720px (Desktop/tablet view)
- **screenshot-narrow.png** - 750×1334px (Mobile view)

These should show your app in use with actual UI.

---

## ✅ Priority List

If you need to prioritize, create these FIRST:

1. **icon-192x192.png** ⭐ CRITICAL
2. **icon-512x512.png** ⭐ CRITICAL
3. **apple-touch-icon-180x180.png** (for iOS home screen)
4. **favicon-32x32.png** (for browser tabs)
5. **icon-192x192-maskable.png** (for Android adaptive icons)
6. **icon-512x512-maskable.png** (for Android adaptive icons)

Then add the rest as needed for better device support.

---

## 🎨 Design Tips

### For Standard Icons:
- Use the full icon area
- Keep important elements away from edges (10% safe margin)
- No transparency required (can use solid purple background)

### For Maskable Icons:
- Place the brain/head logo in center 80% circle
- Fill the corners with your purple gradient
- Ensure no important content in outer 20%

### For Splash Screens:
- Center your logo/brand mark
- Use purple gradient background (#4a148c to #7b1fa2)
- Add app name text below the icon
- Keep overall design minimal for fast loading

---

## 🛠️ Recommended Tools

- **Figma/Sketch**: Design your master icon
- **PWA Asset Generator**: Auto-generate all sizes from one source
  ```bash
  npx pwa-asset-generator [source-image] ./icons
  ```
- **RealFaviconGenerator**: Create comprehensive favicon set
  - https://realfavicongenerator.net/

---

## 📋 Current Status

✅ Manifest file created (`manifest.json`)
✅ HTML meta tags added (`index.html`)
⏳ Icons directory created (`/icons/`)
❌ Image files need to be generated and placed in `/icons/`

---

## 🚀 Testing Your PWA

Once images are in place:

1. **Chrome DevTools**: Application → Manifest (check for errors)
2. **Lighthouse**: Run PWA audit (should score 100%)
3. **iOS Safari**: Add to Home Screen and check icon/splash
4. **Android Chrome**: Install app and check adaptive icon

---

## 📁 File Structure

```
AidMigraineApp/
├── index.html (✅ updated with meta tags)
├── manifest.json (✅ created)
└── icons/
    ├── icon-72x72.png
    ├── icon-96x96.png
    ├── icon-128x128.png
    ├── icon-144x144.png
    ├── icon-152x152.png
    ├── icon-192x192.png ⭐
    ├── icon-384x384.png
    ├── icon-512x512.png ⭐
    ├── icon-192x192-maskable.png
    ├── icon-512x512-maskable.png
    ├── apple-touch-icon-120x120.png
    ├── apple-touch-icon-152x152.png
    ├── apple-touch-icon-167x167.png
    ├── apple-touch-icon-180x180.png
    ├── favicon.ico
    ├── favicon-16x16.png
    ├── favicon-32x32.png
    ├── splash-*.png (14 different sizes)
    ├── screenshot-wide.png
    └── screenshot-narrow.png
```

Total: **33 image files** needed for complete PWA coverage.
