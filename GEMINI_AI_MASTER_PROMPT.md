# Master Prompt for Gemini AI — "العربي (Al-Arabi)" 3D Heritage Registration & Live Program Management App

Copy and paste this entire prompt into **Gemini AI / Google AI Studio** to generate or extend the full production app for **Vercel + Firebase**:

---

```text
Act as a Principal Creative Technologist & Full-Stack Engineer specializing in 3D WebGL/CSS experiences, bilingual Arabic (RTL) / English heritage design, Firebase Firestore real-time `onSnapshot` sync, and Vercel deployment.

Build a breathtaking, production-ready web application for **"العربي — Al-Arabi"**, the Arabic Language Championship organized by the **Department of Arabic Language and Literature, Faculty of Languages and Literatures, Darul Huda Islamic University** (Event Date: **19 December 2026**; Prizes: 1st Place ₹4,444, 2nd Place ₹3,333, 3rd Place ₹2,222; Inquiry Contact: `8590409367`).

### 1. 3D Arabic Heritage & Legacy Design
- **Theme**: Deep burnt-umber / obsidian-espresso (`#120703`, `#1E0C05`, `#2B1208`) with burnished gold (`#FCE7CC`, `#DFA76E`, `#B6763C`), Islamic 8-pointed star (Rub el Hizb) geometry, and classical calligraphy typography (`Amiri`, `Tajawal`, `Inter`).
- **3D Interactive Hero**: Embed a Three.js 3D rotating golden Rub el Hizb / astrolabe sculpture with floating golden dust particles that responds to cursor/touch movement.
- **3D Tilt Medallions & Holographic Pass**: Interactive 3D perspective tilt on the prize medallions and on the generated Digital Candidate Pass (`ARB-2026-XXXX`) with a golden shimmer effect and celebratory particle burst on submission.
- **Live Ticker**: Real-time scrolling/pulsing live registration ticker showing recent entries as they arrive.

### 2. Strictly Ordered 4-Step Candidate Flow
Maintain a clean, numbered, sequential order with a live progress stepper (`01` → `02` → `03` → `04`):
- **Step 01 — بيانات المشارك (Candidate Details)**:
  - `اسم المشارك` (Participant Name — required)
  - `عمر المشارك` (Participant Age — required)
  - `كلية` (College / Faculty — required, with quick-select chips)
  - `رقم الواتساب` (WhatsApp — optional)
- **Step 02 — دفع رسوم الاشتراك (₹50 UPI Payment)**:
  - Scannable UPI ₹50 QR code (`upi://pay?pa=9072584470@upi&pn=Al-Arabi%20Darul%20Huda&am=50&cu=INR&tn=Al-Arabi%20Registration`)
  - Official payment number **`+91 90725 84470`** with 1-tap Copy & Open UPI App button.
- **Step 03 — إرفاق إيصال الدفع (Attach Payment Screenshot)**:
  - Drag-and-drop / file picker with instant preview and compression.
- **Step 04 — تأكيد وإصدار البطاقة (Submit & Reveal 3D Pass)**:
  - Saves immediately to Firestore, triggers real-time `onSnapshot` updates, and reveals the 3D Golden Candidate Pass.

### 3. Real-Time Live Updates & Admin Portal
- **Zero Push/Pull**: Use Firebase Firestore `onSnapshot(query(collection(db, 'al_arabi_registrations'), orderBy('createdAt', 'desc')))` so all organizers see new candidates, screenshots, and status changes instantaneously across all devices in strict chronological order.
- **Admin Login Gate**:
  - Admin Email: `alarabi@dh`
  - Admin Password: `8606971566`
- **Admin Features**: Live KPI cards (Total, Verified, Pending, Revenue ₹), search & status filters, full-size payment screenshot modal, one-click Verify/Reject/Delete, WhatsApp notification trigger, and UTF-8 CSV export.
- **QR Code Studio**: Downloadable PNG QR codes for the live Vercel registration URL and the ₹50 UPI payment QR.
```
