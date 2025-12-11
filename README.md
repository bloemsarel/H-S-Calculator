# Holliday-Segar Fluid Calculator

A comprehensive Progressive Web App (PWA) for calculating fluid requirements using the Holliday-Segar method with integrated diagnosis-based fluid recommendations.

## Features

- ✅ **Holliday-Segar Calculator**: Calculate maintenance fluids based on patient weight
- ✅ **Rehydration Calculator**: Automatic 20ml/kg bolus calculation
- ✅ **Diagnosis-Based Recommendations**: Get specific fluid recommendations for 12+ conditions
- ✅ **Comprehensive Fluid Guide**: Reference table for all major conditions
- ✅ **PWA Support**: Install on desktop, mobile, or tablet
- ✅ **Offline Functionality**: Works without internet connection
- ✅ **Responsive Design**: Mobile-friendly interface

## Installation

### For GitHub Pages Deployment

1. Upload all files to your repository: `bloemsarel.github.io/H-S-Calculator`
2. Ensure the following files are in the repository:
   - `index.html`
   - `manifest.json`
   - `service-worker.js`
   - `icon-192.svg` (or convert to PNG)
   - `icon-512.svg` (or convert to PNG)

3. Enable GitHub Pages in repository settings
4. Access at: `https://bloemsarel.github.io/H-S-Calculator/`

### Installing as PWA

#### On Desktop (Chrome/Edge):
1. Visit the website
2. Click the "📲 Install App on Your Device" button
3. Confirm installation
4. App will appear as standalone application

#### On Mobile (Android):
1. Visit the website in Chrome
2. Tap "Add to Home Screen" from menu
3. Or use the install button if prompted

#### On iOS:
1. Open in Safari
2. Tap Share button
3. Select "Add to Home Screen"

## Usage

### Calculator Tab
1. Enter patient weight in kg
2. Select diagnosis (optional)
3. Click **"Calculate Volume"** for full calculation with fluid recommendations
4. Click **"Get Fluid Recommendation"** for diagnosis-specific fluid protocols only
5. Click **"Reset"** to clear all fields

### Fluid Recommendations Tab
- Browse comprehensive fluid recommendations for all conditions
- Quick reference for:
  - Blood loss
  - Vomiting & Diarrhea
  - DKA
  - Burns
  - Shock states
  - And more...

## Conditions Covered

1. Blood loss (hemorrhage)
2. Vomiting
3. Diarrhea
4. Diabetes & Diabetic Ketoacidosis (DKA)
5. Cardiogenic & Neurogenic Shock
6. Reduced fluid intake (elderly)
7. Heat dehydration
8. Excessive burns
9. Sepsis / Septic shock
10. Post operative patients
11. Renal impairment
12. Hepatic failure

## Formula

**Holliday-Segar Method:**
- First 10 kg: 100 ml/kg/day
- Next 10 kg (11-20 kg): 50 ml/kg/day
- Each kg above 20 kg: 20 ml/kg/day

**Rehydration:**
- 20 ml/kg bolus for dehydration

## Technical Details

- Built with vanilla JavaScript (no dependencies)
- PWA with offline support via Service Worker
- Responsive CSS with gradient design
- LocalStorage not used (session-based)

## License

Free for medical and educational use.

## Disclaimer

This calculator is for educational purposes. Always consult clinical guidelines and senior medical staff for patient care decisions.

---

**Version:** 1.0  
**Last Updated:** December 2024
