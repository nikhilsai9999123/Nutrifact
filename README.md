# NutriScan - Smart Health & FSSAI Nutrition Scanner

NutriScan is a modern mobile web application designed to evaluate food safety and provide personalized nutrition limits tailored to individual health profiles (Diabetes, Hypertension, CKD, Celiac, etc.) based on official **FSSAI HFSS (High in Fat, Sugar, Salt)** guidelines and **ICMR-NIN 2024 Dietary Recommendations**.

---

## 🚀 Quick Start (Run Locally)

### Prerequisites
- Node.js (v18 or higher)
- npm or bun or yarn

### 1. Install Dependencies
```bash
npm install
```

### 2. Start Local Development Server
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### 3. Production Build
```bash
npm run build
npm run preview
```

---

## 🌐 Free Deployment Options

### Option 1: Live Hosted AI Studio URL (Already Live!)
This app is already running and accessible via Google Cloud Run:
- **Public Shared App URL**: `https://ais-pre-wj5pigsfftsjwg7q6bdsid-966314289505.asia-southeast1.run.app`

### Option 2: Deploy Free on Vercel
1. Push this project to a GitHub repository.
2. Go to [Vercel](https://vercel.com) and click **"Add New Project"**.
3. Import your GitHub repository.
4. Framework Preset: **Vite**.
5. Click **"Deploy"**. Vercel will provide an instant free `*.vercel.app` URL with SSL and global CDN.

### Option 3: Deploy Free on Netlify
1. Go to [Netlify](https://www.netlify.com).
2. Drag and drop your `dist` folder (created with `npm run build`), or connect your GitHub repository.
3. Build command: `npm run build`.
4. Publish directory: `dist`.
5. Netlify will generate a free `*.netlify.app` URL.

### Option 4: Deploy Free on Cloudflare Pages
1. Go to the [Cloudflare Dashboard](https://dash.cloudflare.com) > **Workers & Pages**.
2. Connect your GitHub repository.
3. Build settings: Framework preset **Vite**, build command `npm run build`, output directory `dist`.

---

## 📱 Features

- **Auth & Health Profile**: Captures age, gender, fasting blood sugar, HbA1c, systolic/diastolic blood pressure, BMI, and conditions (Type 1/2 Diabetes, Hypertension, CKD, Celiac, Lactose intolerance).
- **QR & Barcode Scanner**: Live camera scanning for standard 13-digit EAN/UPC barcodes and FSSAI QR codes.
- **Image Upload & OCR Fallback**: For packages with missing/damaged QR codes, uploads package front or nutrition table photo to extract nutrients.
- **FSSAI HFSS Safety Engine**: Evaluates sugar, sodium, saturated fat, and trans fat against Indian thresholds.
- **Personalized Recommendations**:
  - Medical safety verdict (Safe, Moderate, Caution, Unsafe).
  - Calculated safe consumption quantity in grams.
  - Highlighted medical warnings in red with clinical rationale.
  - Healthy alternative whole-food swaps.
- **Daily Nutri-Tracker**: Tracks daily calories, sugars, sodium, and saturated fat with dynamic progress gauges and daily FSSAI Health Score.
- **Azure Cloud Architecture Blueprint**: Full architectural spec including Azure API Management (APIM), Logic Apps, Blob Storage, Service Bus, and Computer Vision OCR.

---

## 📄 License
Apache-2.0
