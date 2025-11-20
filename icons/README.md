# PWA Icons Directory

This directory should contain the following icon files for the AidMigraine Progressive Web App:

## Required Icon Sizes

Based on your provided design (purple gradient background with white head profile, brain, and wave patterns):

### Standard Icons (purpose: "any")
- `icon-72.png` - 72x72 pixels
- `icon-96.png` - 96x96 pixels
- `icon-128.png` - 128x128 pixels
- `icon-144.png` - 144x144 pixels
- `icon-152.png` - 152x152 pixels
- `icon-192.png` - 192x192 pixels *(Required for PWA)*
- `icon-384.png` - 384x384 pixels
- `icon-512.png` - 512x512 pixels *(Required for PWA)*

### Maskable Icons (purpose: "maskable")
- `icon-maskable-192.png` - 192x192 pixels with safe zone padding
- `icon-maskable-512.png` - 512x512 pixels with safe zone padding

## Design Guidelines

### Maskable Icons
For maskable icons, ensure your design stays within the safe zone (80% of the icon area centered). The outer 20% (10% on each side) may be cropped on some devices.

### Color Scheme
- Background: Purple gradient (#6b4c9a theme color)
- Foreground: White head profile with brain and wave patterns

## Testing

After adding the icons, you can test them using:
- Chrome DevTools > Application > Manifest
- [Maskable.app](https://maskable.app/) for maskable icon testing
- Lighthouse PWA audit

## File Format
- Format: PNG
- Color mode: RGB with transparency where needed
- Optimization: Recommended for web delivery
