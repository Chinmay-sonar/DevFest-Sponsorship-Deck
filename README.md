# GDG Baroda DevFest 2026 — Sponsorship Deck Web Application

This repository contains the complete, production-ready source code for the **GDG Baroda DevFest 2026 Official Sponsorship Deck**.

## 🌟 Features
- **23 Interactive High-Impact Slides**: Designed following Google Brand & DevFest 2026 visual guidelines.
- **Diagonal Marquee Carousel (Slide 1)**: Smooth continuous diagonal photo marquee with high-resolution DevFest moments.
- **Embedded Video Highlights (Slide 2)**: Seamless borderless video player of DevFest 2024.
- **Audience Fit Mobile Optimizations (Slides 16, 19, 22)**: Dedicated responsive layout with uncropped `{ DevFest Baroda }` logos and tier iconography.
- **Interactive Tier Selector & Email CTA (Slide 23)**: One-click email builder pre-filling sponsorship requests for Silver, Gold, Platinum, and Custom packages.
- **Speaker Notes Drawer**: Built-in talking points and pitch tips for speakers/organizers during pitches.
- **Slide Overview Grid**: Thumbnail drawer (`Grid` button / `Esc`) to jump to any slide instantly.
- **Full Responsive Support**: Optimized for desktop widescreen (16:9), tablets, and mobile smartphones (portrait & landscape).
- **Admin CMS (`admin.html`)**: Real-time content editor to customize slide copy, tier details, and publish updates instantaneously across tabs.

---

## 📂 Project Structure
```
GDG-Baroda-DevFest-Deck/
├── index.html                  # Main interactive slide deck application
├── admin.html                  # Admin CMS dashboard for editing slides
├── default_slides_data.js      # Default slide content & structure (JavaScript)
├── default_slides_data.json    # Default slide content (JSON)
├── Sponsorship Deck From Uv.pptx # Downloadable official presentation deck
├── firebase.json               # Firebase Hosting configuration
├── .firebaserc                 # Firebase project mapping
├── fonts/                      # Google Sans typography family
│   ├── GoogleSans-Bold.ttf
│   ├── GoogleSans-Medium.ttf
│   └── GoogleSans-Regular.ttf
└── media/                      # Optimized image & video assets
    ├── devfest_2024_highlights.mp4
    ├── devfest_slide1_*.jpg    # Marquee photo assets
    ├── gdg_logo_*.png          # GDG brand logos
    └── image*.png              # Tier illustrations & graphic motifs
```

---

## 🚀 Running Locally
No build tools, `npm`, or compilation required! 

### Option 1: Direct Browser
Double-click `index.html` to open directly in any modern browser (Chrome, Safari, Edge, Firefox).

### Option 2: Local HTTP Server (Recommended)
Using Python:
```bash
python -m http.server 8000
```
Then visit: `http://localhost:8000`

---

## ⌨️ Keyboard Shortcuts & Navigation
| Key / Gesture | Action |
| :--- | :--- |
| **Right Arrow (→) / Space / PageDown** | Next slide |
| **Left Arrow (←) / PageUp** | Previous slide |
| **Home / End** | Jump to first / last slide |
| **G / Esc** | Toggle Slide Overview Grid |
| **N** | Toggle Speaker Notes Drawer |
| **Swipe Left / Right** | Slide navigation on touch devices |

---

## 🌐 Deployment to Firebase Hosting
To deploy to the live Firebase URL:
```bash
firebase deploy --only hosting
```
Live URL: [https://devfestsponsorshipdeck.web.app](https://devfestsponsorshipdeck.web.app)
