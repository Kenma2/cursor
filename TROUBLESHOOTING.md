# Troubleshooting Guide

## Common Issues and Solutions

### 1. "npm: command not found" or "node: command not found"

**Problem:** Node.js is not installed on your system.

**Solution:**
- Download and install Node.js from https://nodejs.org/
- Choose the LTS (Long Term Support) version
- After installation, restart your terminal
- Verify installation: `node --version` and `npm --version`

### 2. "Cannot find module" errors

**Problem:** Dependencies are not installed.

**Solution:**
```bash
# Delete node_modules and package-lock.json if they exist
rm -rf node_modules package-lock.json

# Install dependencies
npm install
```

### 3. Port 3000 already in use

**Problem:** Another application is using port 3000.

**Solution:**
- Option 1: Stop the other application
- Option 2: Change the port in `vite.config.ts`:
  ```typescript
  server: {
    port: 3001, // or any other available port
    open: true
  }
  ```

### 4. "Failed to resolve import" errors

**Problem:** Missing dependencies or incorrect import paths.

**Solution:**
```bash
# Reinstall all dependencies
npm install

# If that doesn't work, try:
npm install react react-dom react-router-dom lucide-react
npm install -D vite @vitejs/plugin-react typescript
```

### 5. TypeScript errors

**Problem:** TypeScript configuration issues.

**Solution:**
- Make sure `tsconfig.json` exists and is correct
- Run `npm install` to ensure all TypeScript types are installed
- Check that all `.tsx` files have proper imports

### 6. Browser shows blank page or errors

**Problem:** JavaScript errors in the browser console.

**Solution:**
1. Open browser Developer Tools (F12)
2. Check the Console tab for error messages
3. Check the Network tab for failed requests
4. Common issues:
   - Missing CSS files (check if styles are imported)
   - Missing components (check if all files exist)
   - Routing issues (check if routes are correct)

### 7. "Module not found" for specific files

**Problem:** File path is incorrect or file doesn't exist.

**Solution:**
- Verify all files exist in the correct locations
- Check import paths are correct (case-sensitive on some systems)
- Make sure file extensions match (.tsx vs .ts)

## Step-by-Step Setup (Fresh Start)

1. **Verify Node.js is installed:**
   ```bash
   node --version  # Should show v18.x.x or higher
   npm --version   # Should show 9.x.x or higher
   ```

2. **Navigate to project directory:**
   ```bash
   cd /Users/rfqhit/Desktop/eop
   ```

3. **Install dependencies:**
   ```bash
   npm install
   ```
   This may take a few minutes the first time.

4. **Start the development server:**
   ```bash
   npm run dev
   ```

5. **Open browser:**
   - Should automatically open to http://localhost:3000
   - Or manually navigate to that URL

## Still Not Working?

If you're still experiencing issues:

1. **Check the terminal output** - Look for specific error messages
2. **Check browser console** - Open DevTools (F12) and look at Console tab
3. **Share the error message** - The exact error message will help diagnose the issue

## Quick Test

To verify everything is set up correctly, try:

```bash
# Check if all required files exist
ls src/main.tsx
ls src/App.tsx
ls package.json

# Check if node_modules exists (after npm install)
ls node_modules
```

If any of these commands fail, that's likely the source of your problem.

