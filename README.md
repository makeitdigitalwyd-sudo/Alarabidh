# العربي (Al-Arabi) — Arabic Language Competition Portal

Official registration, UPI payment verification, and zero-refresh live program management suite for **مسابقة العربي (Al-Arabi)** organized by the **Department of Arabic Language and Literature, Faculty of Languages and Literature, Darul Huda Islamic University (جامعة دار الهدى الإسلامية - قسم اللغة العربية وآدابها)** — **19 December 2026 (١٩ ديسمبر ٢٠٢٦)**.

## Features

- **Royal Mahogany & Burnished Gold 3D Design System**: Full RTL (`dir="rtl"`) Arabic interface pairing **Amiri** & **Cairo** typography, Mashrabiya latticework overlay, 8-pointed Islamic geometric star ornaments, and 3D perspective tilt prize medallions (`4444` / `3333` / `2222`).
- **Live Stage Announcement Ticker**: Real-time pulsing ticker synced across all open browsers.
- **Candidate Registration & UPI Payment Portal**:
  - ₹50 registration fee with scannable white-framed QR Code (`qrcode.react`) and one-click UPI app launcher.
  - Automatic HTML5 Canvas payment screenshot compression (`800px` max width, JPEG `0.72` quality) for fast Firestore storage.
  - Instant 3D Digital Entry Pass with unique `ARB-XXXX` registration code upon submission.
- **Zero-Refresh Live Program Management Suite**:
  - PIN-protected organizer console (default PIN: `2026`).
  - Real-time `onSnapshot` sync via Firebase Firestore (`registrations` & `settings/live`) with automatic `BroadcastChannel` + `localStorage` fallback when Firebase `.env` keys are not yet configured.
  - Live KPI cards, stage announcement broadcaster, search & status filter pills, full-screen receipt lightbox, auto-saving inline Chest Number (`رقم الصدر`) assignment, one-click Approve/Reject/Delete, and UTF-8 BOM Excel/CSV export.

## Local Development

```bash
npm install
npm run dev
```

## Firebase Setup (Optional for Cloud Sync)

1. Create a Firebase project and enable **Cloud Firestore**.
2. Copy `.env.example` to `.env` and fill in your `VITE_FIREBASE_*` keys.
3. Recommended Firestore collections:
   - `registrations` (auto-created on first submission)
   - `settings/live` (auto-created when broadcasting an announcement)

> Without `.env` keys, the app automatically runs in **Local Live Sync** mode using `BroadcastChannel` + `localStorage`, syncing instantaneously across open browser tabs.

## Vercel Deployment

1. Push this repository to GitHub/GitLab/Bitbucket or import directly in Vercel.
2. Add your `VITE_FIREBASE_*` environment variables in Vercel Project Settings (and optionally `VITE_ADMIN_PIN`).
3. Deploy — `vercel.json` handles SPA rewrites automatically.
