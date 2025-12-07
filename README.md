# 💧 Holliday-Segar Fluid Calculator

A mobile-friendly web application for calculating maintenance fluid requirements using the Holliday-Segar method for all ages (neonates to adults), with additional rehydration volume calculations and diagnosis-specific fluid recommendations.

## 🌟 Features

- **Holliday-Segar Formula**: Automatic calculation using the 100/50/20 ml/kg method
- **Rehydration Calculator**: 20 ml/kg bolus volume calculation
- **Clinical Guidelines**: Diagnosis-specific fluid recommendations for:
  - Blood loss
  - Vomiting
  - Diarrhea
  - Diabetic rehydration (DKA)
  - Excessive burns
  - Diabetes insipidus
- **Mobile-Responsive**: Optimized for use on smartphones and tablets
- **User-Friendly Interface**: Clean, modern design with intuitive controls
- **Accessibility**: WCAG compliant with ARIA labels and keyboard navigation
- **Print-Friendly**: Formatted for easy printing of results

## 🚀 Live Demo

Visit the live calculator at: `https://[your-username].github.io/hs-fluid-calculator/`

## 📱 Mobile Optimization

This calculator is specifically designed for mobile use with:
- Touch-friendly buttons and inputs
- Responsive layout that adapts to any screen size
- Large, easy-to-read text
- Optimized for both portrait and landscape orientations
- No external dependencies - works offline after first load

## 🛠️ Installation & Deployment

### Option 1: Deploy to GitHub Pages (Recommended)

1. **Create a new repository on GitHub**:
   - Go to [GitHub](https://github.com) and log in
   - Click the "+" icon in the top right and select "New repository"
   - Name it `hs-fluid-calculator` (or any name you prefer)
   - Make it public
   - Don't initialize with README, .gitignore, or license (we'll add our own)

2. **Upload the files**:
   - Click "uploading an existing file"
   - Drag and drop the `index.html` file
   - Add a commit message like "Initial commit: Holliday-Segar Calculator"
   - Click "Commit changes"

3. **Enable GitHub Pages**:
   - Go to your repository's Settings
   - Scroll down to "Pages" in the left sidebar
   - Under "Source", select "Deploy from a branch"
   - Select `main` branch and `/ (root)` folder
   - Click "Save"
   - Wait 1-2 minutes for deployment

4. **Access your calculator**:
   - Your calculator will be live at: `https://[your-username].github.io/hs-fluid-calculator/`
   - Share this URL with colleagues or add it to your mobile home screen

### Option 2: Use Git (For Developers)

```bash
# Clone or create your repository
git clone https://github.com/[your-username]/hs-fluid-calculator.git
cd hs-fluid-calculator

# Add the index.html file
cp /path/to/index.html .

# Commit and push
git add index.html README.md
git commit -m "Add Holliday-Segar Fluid Calculator"
git push origin main
```

Then follow step 3 above to enable GitHub Pages.

### Option 3: Local Development

Simply open `index.html` in any web browser. No server required!

```bash
# On Mac/Linux
open index.html

# On Windows
start index.html

# Or use Python's built-in server
python -m http.server 8000
# Then visit http://localhost:8000
```

## 📲 Add to Mobile Home Screen

### iOS (iPhone/iPad)
1. Open the calculator in Safari
2. Tap the Share button (square with arrow)
3. Scroll down and tap "Add to Home Screen"
4. Name it "HS Calculator" and tap "Add"

### Android
1. Open the calculator in Chrome
2. Tap the three-dot menu
3. Select "Add to Home screen"
4. Name it and tap "Add"

## 📖 How to Use

1. **Enter Patient Weight**: Input the patient's weight in kilograms (neonates to adults)
2. **Select Diagnosis** (Optional): Choose a clinical condition for specific fluid recommendations
3. **Click Calculate**: View the maintenance fluid requirements and rehydration volume
4. **Review Results**: See daily requirements (mL/day), hourly rate (mL/hr), and rehydration volume
5. **Reset**: Clear all fields to start a new calculation

## 🧮 Calculation Method

### Holliday-Segar Formula
- **0-10 kg**: 100 mL/kg/day
- **11-20 kg**: 1000 mL + 50 mL/kg for each kg above 10
- **>20 kg**: 1500 mL + 20 mL/kg for each kg above 20

**Note**: The Holliday-Segar method is most accurate for patients 0-70 kg. For adults >70 kg, clinical judgment and alternative fluid calculation methods should be considered.

### Rehydration Volume
- **Standard bolus**: 20 mL/kg

## 📋 Clinical Guidelines Included

The calculator provides evidence-based fluid recommendations for:

- **Blood Loss**: Isotonic crystalloid while preparing blood products
- **Vomiting**: Normal Saline or Ringer's Lactate for rehydration
- **Diarrhea**: Ringer's Lactate to help buffer metabolic acidosis
- **DKA**: Balanced crystalloid with careful glucose and electrolyte monitoring
- **Burns**: Ringer's Lactate using Parkland formula
- **Diabetes Insipidus**: Hypotonic fluids to correct free water deficit

## ⚠️ Medical Disclaimer

**This calculator is for educational and reference purposes only.** Always:
- Consult appropriate clinical guidelines
- Consider individual patient factors (age, comorbidities, clinical condition)
- Monitor patient response to therapy
- Adjust based on clinical condition
- Follow institutional protocols
- Note: The Holliday-Segar formula is most accurate for patients 0-70 kg. For adults >70 kg, consider using alternative fluid calculation methods.

**This tool does not replace clinical judgment or professional medical advice.**

## 🔧 Technical Details

- **Pure HTML/CSS/JavaScript**: No frameworks or dependencies
- **File Size**: < 20 KB (extremely fast loading)
- **Browser Support**: All modern browsers (Chrome, Firefox, Safari, Edge)
- **Offline Capable**: Works after first load without internet
- **Standards Compliant**: HTML5, CSS3, ES6+

## 🎨 Customization

To customize the calculator:

1. **Colors**: Modify the CSS gradient in the `body` style
2. **Formula**: Adjust the `hollidaySegar()` function
3. **Diagnoses**: Add/remove items in the `fluidRecommendations` object
4. **Styling**: Edit the `<style>` section for your preferred look

## 📝 Version History

### Version 1.0 (Current)
- Initial release
- Holliday-Segar calculation
- Rehydration volume (20 mL/kg)
- Six diagnosis-specific fluid recommendations
- Mobile-responsive design
- Accessibility features

## 🤝 Contributing

Contributions are welcome! To suggest improvements:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Create a Pull Request

## 📄 License

This project is open source and available under the MIT License.

## 👥 Credits

Created for healthcare professionals who need quick, reliable fluid calculations on the go.

## 📞 Support

For issues or questions:
- Open an issue on GitHub
- Contact: [Your contact information]

## 🔗 Related Resources

- [Holliday-Segar Method - Wikipedia](https://en.wikipedia.org/wiki/Maintenance_fluid_therapy)
- [Pediatric Fluid Management Guidelines](https://www.aap.org)

---

**Made with ❤️ for healthcare professionals worldwide**

*Remember: Always verify calculations and follow local clinical protocols*
