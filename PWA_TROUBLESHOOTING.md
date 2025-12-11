# PWA Installation Troubleshooting Guide

## Why the Install Button Isn't Showing

### Requirements for PWA Install Prompt:

1. ✅ **HTTPS Connection** - GitHub Pages provides this automatically
2. ✅ **Valid manifest.json** - Check if file is accessible
3. ✅ **Service Worker registered** - Must be properly configured
4. ✅ **Icons** - Must be accessible (SVG or PNG)
5. ❌ **Not already installed** - If already installed, button won't show
6. ❌ **Browser support** - Must use Chrome, Edge, or compatible browser

---

## Quick Checks:

### 1. Test Your Manifest File
Open in browser: `https://bloemsarel.github.io/H-S-Calculator/manifest.json`

**Should show:** JSON file with your app configuration
**If 404 error:** File not uploaded correctly

### 2. Check Service Worker
1. Open your site: `https://bloemsarel.github.io/H-S-Calculator/`
2. Press `F12` (or Right-click → Inspect)
3. Go to **Console** tab
4. Look for: "Service Worker registered"
5. Go to **Application** tab → **Service Workers**
6. Should show: `service-worker.js` as "activated and running"

### 3. Check Icons
Open in browser:
- `https://bloemsarel.github.io/H-S-Calculator/icon-192.svg`
- `https://bloemsarel.github.io/H-S-Calculator/icon-512.svg`

**Should show:** Water drop icons
**If 404:** Icons not uploaded

### 4. Browser Compatibility
**✅ Works on:**
- Chrome (Desktop & Android)
- Edge (Desktop)
- Samsung Internet (Android)
- Opera (Desktop & Android)

**❌ Doesn't work on:**
- Firefox (has limited PWA support)
- Safari on iOS (use "Add to Home Screen" instead)
- Internet Explorer

---

## Solutions:

### Solution 1: Use the Updated Files
I've created updated files with correct paths. Re-upload:
- ✅ manifest.json (updated)
- ✅ index.html (if needed)
- ✅ service-worker.js
- ✅ icon-192.svg
- ✅ icon-512.svg

### Solution 2: Clear Browser Cache
1. Press `Ctrl + Shift + Delete` (or `Cmd + Shift + Delete` on Mac)
2. Select "Cached images and files"
3. Click "Clear data"
4. Refresh the page

### Solution 3: Test in Incognito/Private Mode
1. Open Chrome Incognito window (`Ctrl + Shift + N`)
2. Visit your site
3. Install button should appear if everything is working

### Solution 4: Wait 5-10 Minutes
GitHub Pages can take a few minutes to propagate changes

### Solution 5: Check Console for Errors
1. Press `F12`
2. Go to Console tab
3. Look for red error messages
4. Common errors:
   - "Failed to fetch manifest"
   - "Service worker registration failed"
   - "Icon not found"

---

## Alternative Installation Methods:

### Chrome Desktop:
1. Visit the site
2. Look for ⊕ icon in address bar (right side)
3. Click it → "Install"

OR

1. Click 3 dots menu (⋮) in top right
2. Look for "Install H-S Calculator..."
3. Click to install

### Chrome Android:
1. Visit the site
2. Tap 3 dots menu (⋮)
3. Tap "Add to Home screen"
4. Tap "Install"

### iOS Safari:
1. Visit the site
2. Tap Share button (square with arrow)
3. Scroll down and tap "Add to Home Screen"
4. Tap "Add"

---

## Verify Installation Working:

### Test Checklist:
- [ ] Site loads at correct URL
- [ ] manifest.json accessible (no 404)
- [ ] Icons accessible (no 404)
- [ ] Console shows "Service Worker registered"
- [ ] Using Chrome or Edge browser
- [ ] Not already installed
- [ ] Using HTTPS (GitHub Pages default)

### Expected Behavior:
- Install button appears after 3-5 seconds
- Button is green with text "📲 Install App on Your Device"
- Clicking button shows browser's native install prompt

---

## Still Not Working?

### Debug Steps:

1. **Open Developer Tools** (F12)
2. **Go to Application Tab**
3. **Check Manifest:**
   - Should show app name, icons, colors
   - If errors shown, manifest.json has issues
4. **Check Service Workers:**
   - Should show service-worker.js running
   - If not, check Console for errors
5. **Check Console Tab:**
   - Look for any red errors
   - Common: 404 errors for manifest or icons

### Send me this info if still stuck:
- Browser and version (e.g., "Chrome 120")
- Device (e.g., "Windows 11" or "Android 13")
- Any error messages from Console
- Screenshot of Application tab → Manifest section

---

## Pro Tips:

1. **Test in Chrome first** - Best PWA support
2. **Use Incognito** - Avoids cache issues
3. **Check mobile too** - Installation differs per device
4. **Lighthouse audit** - In DevTools, run Lighthouse PWA audit

---

## Quick Fix: Manual Install Without Button

Even without the install button, users can still install:

**Desktop Chrome:**
- Click ⊕ icon in address bar
- Or: Menu → "Install H-S Calculator"

**Mobile:**
- Tap "Add to Home Screen" from browser menu

The app will work perfectly either way!

---

Need more help? Let me know what error messages you see!
