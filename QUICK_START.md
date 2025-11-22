# Quick Start Guide

## ⚠️ IMPORTANT: You Cannot Open index.html Directly!

This is a **React application** that requires a development server to run. Opening `index.html` directly in a browser will NOT work because:
- The browser cannot compile TypeScript/React code
- Module imports need to be processed by a build tool (Vite)
- The app needs to be "built" before it can run

## ✅ Correct Way to Run the App

### Step 1: Install Node.js
1. Go to **https://nodejs.org/**
2. Download the **LTS version** (recommended)
3. Install it (double-click the installer and follow instructions)
4. **Restart your terminal** after installation

### Step 2: Verify Installation
Open a new terminal and run:
```bash
node --version
npm --version
```
Both should show version numbers (not "command not found")

### Step 3: Install Dependencies
Navigate to the project folder and install:
```bash
cd /Users/rfqhit/Desktop/eop
npm install
```
This will download all required packages (takes 1-2 minutes)

### Step 4: Start the Development Server
```bash
npm run dev
```

### Step 5: Open in Browser
- The app will automatically open at `http://localhost:3000`
- Or manually go to that URL in your browser

## 🎯 What You'll See

After running `npm run dev`, you should see:
```
  VITE v5.x.x  ready in xxx ms

  ➜  Local:   http://localhost:3000/
  ➜  Network: use --host to expose
```

Then the app will work in your browser!

## 🔑 Demo Login

Once the app is running, use these accounts:
- Email: `owner@eops.com` (any password)
- Email: `manager@eops.com` (any password)
- Email: `coach@eops.com` (any password)
- Email: `player@eops.com` (any password)

## ❓ Still Having Issues?

Check `TROUBLESHOOTING.md` for more help!

