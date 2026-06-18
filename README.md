#  Farmer Land Area Converter

A simple, intuitive web-based tool designed for farmers, landowners, and real estate professionals to quickly convert between common land measurement units.

![Land Area Converter Screenshot](https://via.placeholder.com/800x400?text=Land+Area+Converter+Preview)

##  Features

- **Instant Conversion** – Convert between 5 common land units in real-time
- **5 Supported Units**:
  - Acres
  - Hectares
  - Square Meters (m²)
  - Square Feet (ft²)
  - Square Yards (yd²)
- **Smart Unit Switching** – Click on unit labels to cycle through available units
- **Quick Presets** – One-click access to common values (0.5, 1, 2.5, 5, 10, 20 acres)
- **Swap Function** – Exchange "From" and "To" units with a single click or keyboard shortcut
- **Keyboard Shortcut** – Press `S` to swap units instantly
- **Mobile Responsive** – Works seamlessly on desktop, tablet, and smartphone
- **Clean UI** – Farmer-friendly design with clear visual hierarchy

## 🚀 Live Demo

[View Live Demo](https://your-demo-link.com) *(Replace with your actual deployment link)*

## 🛠️ How to Use

1. **Enter a value** in the "From" input field
2. **Select units** by:
   - Clicking on the unit labels (Acres, Hectares, etc.)
   - Or using the "Swap units" button to exchange From/To units
3. **Read the result** instantly in the "To" field and the Result box
4. **Use presets** for quick entry of common values
5. **Keyboard shortcut**: Press `S` to swap units without lifting your hands from the keyboard

## 📦 Installation

### Option 1: Direct Download
```bash
# Clone the repository
git clone https://github.com/yourusername/land-area-converter.git

# Navigate to the project folder
cd land-area-converter

# Open index.html in your browser
open index.html
```

### Option 2: Quick Start
Copy the entire `index.html` file and open it directly in any modern web browser. No server or build process required.

## 🧮 Conversion Logic

The converter uses square meters as the base unit for all conversions:

| Unit | Conversion Factor (to m²) |
|------|---------------------------|
| Acres | 4046.8564224 |
| Hectares | 10000 |
| Square Meters | 1 |
| Square Feet | 0.09290304 |
| Square Yards | 0.83612736 |

All conversions happen in real-time as you type.

## 🎨 Customization

### Adding New Units
To add a new land measurement unit, modify the `UNIT_FACTORS` and `UNIT_LABELS` objects in the JavaScript section:

```javascript
const UNIT_FACTORS = {
  'acres': 4046.8564224,
  'hectares': 10000,
  'sqm': 1,
  // Add your new unit here
  'sqkm': 1000000  // Square Kilometers
};

const UNIT_LABELS = {
  'acres': 'Acres',
  'hectares': 'Hectares',
  // Add corresponding label
  'sqkm': 'km²'
};
```

### Styling
The converter uses CSS custom properties and modern styling. Modify the color scheme in the `<style>` section:

```css
/* Change the primary color scheme */
background: linear-gradient(145deg, #f5f2e8 0%, #e8e0d0 100%);
/* Modify accent colors */
background: #5b7a4b;  /* Farm green accent */
```

## 🌐 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Android Chrome)

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📧 Contact

- **Author**: [Your Name]
- **Email**: [your.email@example.com]
- **GitHub**: [@yourusername](https://github.com/yourusername)

## 🙏 Acknowledgments

- Built with vanilla HTML, CSS, and JavaScript – no external dependencies
- Designed with farmers and rural communities in mind
- Iconography uses standard emojis for universal compatibility

---

**Made with ❤️ for farmers and land stewards everywhere**
