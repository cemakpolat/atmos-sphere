# atmos sphere - Advanced Weather Application

A beautiful, feature-rich cross-platform Electron weather application that provides comprehensive weather information for cities worldwide with stunning animations and an intuitive interface.

![atmos sphere app](./docs/atmossphere.png 'atmos sphere app')

---

## ✨ Features

### 🌍 Core Weather Features

- **Multi-City Management**: Add, remove, and track weather for multiple cities simultaneously
- **Autocomplete Search**: Smart city search with real-time suggestions
- **7-Day Forecast**: View detailed 7-day weather outlook with hourly and daily views
- **Extended Weather Details**:
  - Current temperature with "feels like"
  - Humidity percentage
  - Wind speed and direction
  - UV index with safety recommendations
  - Sunrise/sunset times
  - Precipitation probability
- **Historical Weather Data**: View past 7 days of weather history
- **Temperature Units**: Toggle between Celsius and Fahrenheit

### 🗺️ Weather Radar & Maps

- **Interactive Maps**: Integrated Leaflet maps with city markers
- **Weather Overlays**: Toggle precipitation, clouds, and temperature layers
- **Zoom & Pan**: Full map controls for detailed exploration

### 📍 Geolocation

- **Auto-Detect Location**: Automatically detect and add your current location
- **Location Badge**: Visual indicator for current location cities

### 🎨 Visual Experience

- **Weather-Based Animations**: Dynamic background animations that match weather conditions:
  - ☀️ Sunny - Gradient with light beams
  - 🌧️ Rainy - Rain animation with droplets
  - ❄️ Snowy - Snowflake animation
  - ☁️ Cloudy - Drifting clouds
  - ⛈️ Thunderstorm - Heavy rain with lightning flashes
- **Multiple Themes**: 8 beautiful gradient themes to choose from
- **Compact & Grid Views**: Switch between list and card layouts
- **Drag & Drop**: Reorder cities by dragging cards
- **Masonry Layout**: Optimized card positioning for better space usage

### 🔔 Alerts & Notifications

- **Weather Alerts**: Automatic detection of severe weather conditions
- **Native Notifications**: System notifications for weather alerts
- **Customizable Alerts**: Configure which alert types you want to receive:
  - Thunderstorms
  - Heavy rain
  - Heavy snow
  - Extreme temperatures
  - High precipitation

### ⚙️ Settings & Customization

- **Auto-Refresh**: Configurable auto-refresh interval (1-60 minutes)
- **Animation Controls**: Enable/disable weather animations
- **Alert Preferences**: Fine-tune notification settings
- **Theme Selection**: Choose from 8 gradient themes
- **Persistent Settings**: All preferences saved across sessions

### ⌨️ Keyboard Shortcuts

- `Ctrl/Cmd + F` - Focus search bar
- `Ctrl/Cmd + R` - Refresh all cities
- `Ctrl/Cmd + N` - Add new city
- `Escape` - Close search/autocomplete

### 🔄 Additional Features

- **Manual Refresh**: Refresh individual cities or all at once
- **Toast Notifications**: In-app notifications for actions and errors
- **Custom Title Bar**: Headless window with custom controls
- **Responsive Design**: Adapts to different window sizes
- **Loading States**: Visual feedback during data fetching
- **Error Handling**: Comprehensive error messages and recovery

---

## 🛠️ Technologies

- **Electron**: Cross-platform desktop framework
- **Bootstrap 5**: Modern, responsive UI components
- **Font Awesome 6**: Icon library
- **Leaflet**: Interactive maps
- **Open-Meteo API**: Weather and geocoding data
- **Jest**: Unit and integration testing
- **ESLint & Prettier**: Code quality and formatting

---

## 📦 Installation

### Download Pre-built Binaries

Download the latest release for your platform from the [Releases](https://github.com/cemakpolat/atmos-sphere/releases) page:

- **Windows**: `atmos-sphere-Setup-*.exe`
- **macOS**: `atmos-sphere-*.dmg`
- **Linux**: `atmos-sphere-*.AppImage`

### Build from Source

1. **Clone the repository**:

   ```bash

   git clone https://github.com/cemakpolat/atmos-sphere.git
   cd atmos-sphere
   ```

````

2. **Install dependencies**:
 ```bash
 npm install
````

3. **Run in development mode**:

   ```bash
   npm start
   ```

4. **Build for production**:

   ```bash
   # Build for all platforms
   npm run build

   # Or build for specific platform
   npm run build:win    # Windows
   npm run build:mac    # macOS
   npm run build:linux  # Linux
   ```

---

## 🧪 Testing

```bash
# Run all tests
npm test

# Run tests in watch mode
npm run test:watch

# Run linter
npm run lint

# Format code
npm run format

# Check formatting
npm run format:check
```

---

## 📚 Documentation

- [Architecture Guide](./ARCHITECTURE.md) - SOLID principles and code structure
- [Animations System](./ANIMATIONS.md) - Weather animation implementation
- [Weather Alerts](./WEATHER_ALERTS_FEATURE.md) - Alert system documentation
- [CI/CD Guide](./CI_CD_GUIDE.md) - Build and deployment pipelines
- [TODO List](./TODO.md) - Future features and roadmap
- [Improvements](./IMPROVEMENTS.md) - Changelog and feature history

---

## 🎯 Project Structure

```
atmos-sphere/
├── src/
│   ├── main/           # Electron main process
│   ├── preload.js      # Preload script
│   ├── renderer/       # Renderer process
│   │   ├── services/   # Business logic
│   │   │   ├── animations/    # Weather animations
│   │   │   └── providers/     # Weather API providers
│   │   ├── utils/      # Helper functions
│   │   ├── index.html  # Main UI
│   │   ├── renderer.js # UI logic
│   │   └── styles.css  # Styling
│   └── storage.js      # Settings storage
├── .github/workflows/  # CI/CD pipelines
└── docs/              # Screenshots and assets
```

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the ISC License - see the package.json file for details.

---

## 🙏 Acknowledgments

- Weather data provided by [Open-Meteo API](https://open-meteo.com/)
- Icons by [Font Awesome](https://fontawesome.com/)
- Maps by [Leaflet](https://leafletjs.com/) and [OpenStreetMap](https://www.openstreetmap.org/)

---

## 📧 Contact

Cem Akpolat - akpolatcem@gmail.com

Project Link: [https://github.com/cemakpolat/atmos-sphere](https://github.com/cemakpolat/atmos-sphere)

---

**Built with ❤️ using Electron**
