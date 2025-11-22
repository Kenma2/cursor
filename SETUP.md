# Setup Instructions

## Prerequisites

Make sure you have Node.js installed (version 18 or higher).

Check if Node.js is installed:
```bash
node --version
npm --version
```

If not installed, download from: https://nodejs.org/

## Installation Steps

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Start the development server:**
   ```bash
   npm run dev
   ```

3. **Open your browser:**
   The app should automatically open at `http://localhost:3000`

## Troubleshooting

### If npm is not found:
- Make sure Node.js is installed
- Try using `npx` instead: `npx npm install`
- Or use `yarn` if you have it: `yarn install` then `yarn dev`

### If you see port errors:
- The default port is 3000
- Change it in `vite.config.ts` if needed

### If you see module errors:
- Delete `node_modules` folder and `package-lock.json`
- Run `npm install` again

## Demo Login

Use any of these accounts (password can be anything):
- `owner@eops.com` - Team Owner
- `manager@eops.com` - Team Manager  
- `coach@eops.com` - Team Coach
- `player@eops.com` - Player

