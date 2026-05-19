# MICH Digital Shop 🛒

Premium PWA Reseller Marketplace — **michshop.vercel.app**

---

## Files
```
mich-digital-shop/
├── index.html          ← Complete app (all-in-one)
├── vercel.json         ← Vercel routing config
├── firestore.rules     ← Firebase security rules
└── public/
    ├── manifest.json   ← PWA manifest
    └── sw.js           ← Service Worker
```

---

## Deploy on Vercel (5 minutes)

### 1. Upload to GitHub
Create a new repo and upload all files maintaining folder structure.

### 2. Connect to Vercel
- Go to [vercel.com](https://vercel.com)
- New Project → Import your GitHub repo
- Framework: **Other**
- Root Directory: `.` (root)
- Click **Deploy**

### 3. Custom Domain
- In Vercel Dashboard → Settings → Domains
- Add: `michshop.vercel.app`

---

## Firebase Setup

### Enable in Firebase Console:
1. **Authentication** → Enable Email/Password + Google
2. **Firestore Database** → Create in production mode
3. **Storage** → Enable (for product images)

### Deploy Security Rules:
```bash
npm install -g firebase-tools
firebase login
firebase init firestore
# Copy contents of firestore.rules
firebase deploy --only firestore:rules
```

---

## Make First User Admin

In Firestore Console:
- Go to `users` collection
- Find your user document
- Change `role` field to `"admin"`

---

## Features Included

- ✅ Google + Email Authentication
- ✅ Role System (Admin, Reseller, Marketer, Customer)
- ✅ Home with animated stats & flash deals
- ✅ Product catalog with share system
- ✅ Multi-language captions (EN/UR/HI/AR)
- ✅ WhatsApp / Telegram / Facebook sharing
- ✅ Order management (Physical + Digital)
- ✅ Earnings dashboard
- ✅ Withdraw system (JazzCash, Easypaisa, Bank, Binance, PayPal)
- ✅ Client management
- ✅ Referral / Invite system
- ✅ Post maker
- ✅ Admin panel
- ✅ Notifications
- ✅ PWA (installable, offline support)
- ✅ Service Worker
- ✅ Firebase Security Rules

---

## Support
MICH Digital Shop — Pakistan's #1 Reseller Platform
