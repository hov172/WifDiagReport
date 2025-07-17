# Wifi Diagnostics Report

<img width="1023" alt="WifiApp" src="https://github.com/user-attachments/assets/3103d218-9c7b-4279-8b23-cdb0a489afcf" />

## Overview

**Wifi Diagnostics Report** is a professional-grade, open-source macOS app for WiFi/network diagnostics, system info, and technical troubleshooting.

Built for IT professionals, support staff, students, and power users, it empowers anyone to analyze their Mac's connectivity, scan WiFi, map coverage, check speeds, and export rich diagnostics with ease.

> **Note:** This app requires macOS 13.0 (Ventura) or newer.

---

## ✨ What's New - January 2025

### **🎯 Complete State Persistence**
- **Coverage maps now remember zoom, rotation, and pan state** when saved/loaded
- Perfect project restoration for professional workflows

### **📄 Professional PDF Export**
- High-quality PDF generation with measurement data and floor plans
- Professional layouts with statistics and analysis

### **⚡ Performance Optimizations**
- Improved app responsiveness with complex floor plans and large datasets
- Enhanced compilation times and stability

### **🎨 Visual Consistency**
- Signal quality colors now consistent across all UI components
- Green=Excellent, Blue=Good, Orange=Fair, Red=Poor

### **🛡️ Enhanced Stability**
- Crash prevention and error handling improvements
- Better handling of edge cases and empty data

### **📊 Real-Time Signal Monitoring**
- **🆕 Live WiFi signal monitoring** with 1-second interval updates
- Real-time charts showing signal strength, noise levels, and SNR
- Signal stability analysis with trend detection
- Export capability for long-term monitoring data

### **🔧 Improved Diagnostic Flow**
- **🆕 Restored "Run All Diagnostics" workflow** with confirmation popup
- Full-screen diagnostic overlay with animated progress indicator
- Better user feedback during test execution
- Enhanced export process that keeps app open after file saves

### **🎯 Enhanced Dashboard**
- **🆕 Comprehensive dashboard view** with real-time network metrics
- Quick action cards for common diagnostic tasks
- Recent activity tracking and system overview
- Improved metric visualization and status indicators

---

## Features

- 🌐 **Real-Time Device & Network Info**
  - Models, OS version (shown with marketing name & build), CPU/RAM, active interface, MAC/IP/DNS, WiFi details (SSID, channel, band, security)
  - Real-time network monitoring with automatic refresh capabilities
  - **🆕 Enhanced dashboard** with quick stats and system overview

- 📡 **WiFi Scanner**
  - Instantly see all nearby SSIDs, signal quality, channels, security protocols, and export full scans to CSV/text
  - Advanced channel analysis and interference detection
  - **Consistent visual signal strength indicators** with professional color coding
  - Network detail modal with comprehensive technical information
  - Multi-AP network analysis with roaming detection

- 📊 **Real-Time Signal Monitoring** ⭐
  - **🆕 Live WiFi signal monitoring** with continuous 1-second updates
  - Real-time charts showing RSSI, noise levels, and signal-to-noise ratio
  - Signal stability analysis with connection quality assessment
  - Trend detection (improving, stable, declining) over time
  - Export monitoring data to CSV for detailed analysis
  - Up to 5 minutes of historical data retention (300 data points)

- 🗺️ **Advanced Coverage Mapping** ⭐
  - Interactive floor plan upload and visualization with support for PNG, JPEG, PDF, SVG, TIFF formats
  - Multiple coordinate tracking modes:
    - **Manual Entry** - Type coordinates directly
    - **Click to Select** - Point and click on map
    - **Live Mouse Tracking** - Real-time cursor following
    - **Grid Assistant** - Systematic measurement grid with customizable spacing
  - **Full map transform support**: zoom, rotate, pan with precise controls
  - Professional measurement point cards with signal quality indicators
  - Built-in recommendations system with best practices guide
  - **🆕 Complete state persistence** - save and load coverage map projects with **exact zoom/rotation/pan state**
  - **🆕 Professional PDF export** with measurement data and statistics
  - Signal quality legend and coverage statistics
  - Roaming event detection and analysis

- 🚦 **Comprehensive Speed & Network Testing**
  - Visual download/upload speed tests with animated meters
  - Latency and packet loss analysis with real-time monitoring
  - Historical tracking of all test results with automatic logging
  - **🆕 "Run All Diagnostics"** - comprehensive automated testing suite with confirmation popup
  - **🆕 Full-screen diagnostic overlay** with animated progress indicator
  - Real-time progress indicators and detailed result breakdowns

- 📊 **Professional Export System**
  - Export all technical and user info, test results, and network scans
  - Multiple export formats (text reports, CSV data, **high-quality PDF coverage maps**)
  - Coverage map data export with complete measurement points and transform state
  - **🆕 MainActor-optimized PDF generation** for reliable exports
  - **🆕 Enhanced export workflow** - app stays open after successful exports
  - Customizable export templates with user and location information
  - Real-time signal monitoring data export

- 🎨 **Modern Professional UI**
  - Enhanced welcome screen with animated feature cards
  - Modern sidebar with hover effects and smooth animations
  - Dynamic Light/Dark mode with professional color schemes
  - **🆕 Consistent color-blind friendly icons** and accessibility features
  - Extensive keyboard shortcuts and VoiceOver support
  - Adaptive layout for different screen sizes
  - **🆕 Performance-optimized** for large datasets and complex interactions
  - **🆕 Improved dashboard** with metric cards and quick actions

- 🧑‍💻 **Advanced Customization**
  - Hide or show any sidebar feature for deployments
  - Configuration file-based customization (no code changes needed)
  - Perfect for enterprise deployments and non-technical users
  - **🆕 Updated configuration keys** for all current features

- 🔧 **Advanced Technical Features**
  - Real-time WiFi monitoring and comprehensive analysis
  - Advanced visualization with Charts framework
  - Comprehensive network diagnostics orchestration
  - **🆕 Enhanced crash prevention** and error handling
  - Professional-grade measurement accuracy
  - **🆕 Improved diagnostic flow** with better user feedback

- ❓ **Integrated Help & Documentation**
  - Comprehensive in-app help system
  - Step-by-step guides for all features
  - Coverage mapping best practices
  - Troubleshooting guides and technical explanations
  - **🆕 Real-time monitoring usage guide**

---

## 🚀 Quick Start

### **Installation Requirements**
- macOS 13.0 (Ventura) or newer
- Admin privileges for some network diagnostics

### **Basic Usage**
1. **Launch the app** - Modern welcome screen guides you through features
2. **Dashboard** - **🆕 View comprehensive system overview with real-time metrics**
3. **Device Info** - View comprehensive system information
4. **WiFi Scanner** - Scan and analyze nearby networks
5. **Real-Time Monitor** - **🆕 Monitor WiFi signal quality in real-time**
6. **Coverage Mapping** - Upload floor plans and create professional signal maps
7. **Speed Testing** - Run comprehensive network performance tests
8. **Export** - Generate professional reports and data exports

### **Coverage Mapping Workflow** 🗺️
1. **Upload Floor Plan** - Drag & drop or select PNG, JPEG, PDF, SVG, TIFF files
2. **Choose Tracking Mode** - Manual, click, live, or **Grid Assistant** (recommended)
3. **Take Measurements** - Click locations to record real-time WiFi signal data
4. **Transform & Analyze** - Zoom, rotate, pan for perfect alignment
5. **Export Data** - Save as JSON project (with complete state) or generate PDF report

### **Real-Time Signal Monitoring Workflow** 📊
1. **Navigate to Real-time Monitor** - Select from sidebar
2. **Start Monitoring** - Click "Start Monitoring" button
3. **Observe Live Data** - Watch real-time charts and statistics update every second
4. **Analyze Trends** - Monitor signal stability, variation, and connection quality
5. **Export Data** - Save monitoring session data as CSV for further analysis

---

## 🔧 Sidebar Customization (for Techs, Admins, Deployments)

**Wifi Diagnostics Report** makes it easy for technical users to toggle feature visibility for non-technical end-users—**without code changes or custom builds**.

### How It Works

The app loads a bundled configuration file:  
**`WifiDialogReport/Configuration.plist`**

This file uses keys of the form `HideXXXX` for each feature or tool in the sidebar.

- Set the value to `<true/>` to **hide** a sidebar section or tool
- Set the value to `<false/>` to **show** that section/tool

#### Example: `Configuration.plist`
```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
    <key>HideDashboard</key>
    <false/>
    <key>HideNetwork Scanner</key>
    <false/>
    <key>HideSpeed Test</key>
    <false/>
    <key>HideCoverage Map</key>
    <false/>
    <key>HideNetwork History</key>
    <false/>
    <key>HideReal-time Monitor</key>
    <false/>
    <key>HideHelp</key>
    <false/>
    <key>HideExport</key>
    <false/>
    <key>HideRunAll</key>
    <false/>
    <key>HideDebugExport</key>
    <true/>
</dict>
</plist>
```

### Available Configuration Keys

| Key | Description | Default |
|-----|-------------|---------|
| `HideDashboard` | **🆕** Hide dashboard overview | `false` |
| `HideNetwork Scanner` | Hide WiFi scanner tool | `false` |
| `HideSpeed Test` | Hide speed testing tool | `false` |
| `HideCoverage Map` | Hide coverage mapping tool | `false` |
| `HideNetwork History` | Hide network test history | `false` |
| `HideReal-time Monitor` | **🆕** Hide real-time signal monitoring | `false` |
| `HideHelp` | Hide help documentation | `false` |
| `HideExport` | Hide export functionality | `false` |
| `HideRunAll` | Hide "Run All Tests" button | `false` |
| `HideDebugExport` | Hide debug export option | `true` |

### **🆕 Updated Configuration**
The configuration system has been updated to match all current sidebar sections and features. Make sure to use the exact key names shown above (including spaces) for proper functionality.

---

## 🛠️ Technical Details

### **Real-Time Signal Monitoring**
- **Update Frequency**: 1-second intervals
- **Data Retention**: 300 data points (5 minutes)
- **Metrics Tracked**: RSSI, Noise Level, SNR, TX Rate, Signal Quality
- **Export Format**: CSV with timestamps and all measured parameters
- **Performance**: Background processing to avoid UI blocking

### **Enhanced Diagnostic Flow**
- **Confirmation Popup**: Shows before running comprehensive diagnostics
- **Progress Overlay**: Full-screen animated indicator during test execution
- **Concurrent Testing**: Speed, latency, and packet loss tests run simultaneously
- **Export Integration**: Automatic prompt to export results after completion

### **Improved Export System**
- **App Persistence**: Application remains open after successful exports
- **Success Feedback**: Clear confirmation messages with file information
- **Error Handling**: Detailed error messages for troubleshooting
- **Multiple Formats**: Text reports, CSV data, and PDF coverage maps

---

## 🤝 Contributing

We welcome contributions! Whether you're fixing bugs, adding features, or improving documentation, your help makes this tool better for everyone.

### **Development Setup**
1. Clone the repository
2. Open `Wifi Diagnostics Report.xcodeproj` in Xcode
3. Build and run (requires macOS 13.0+)

### **Feature Areas**
- Real-time monitoring enhancements
- Additional export formats
- Advanced network analysis
- UI/UX improvements
- Performance optimizations

---

## 📄 License

This project is open-source and available under the MIT License.

---

## 🙏 Acknowledgments

Built with ❤️ for the macOS community, IT professionals, and anyone who needs reliable network diagnostics.

**Special thanks to:**
- The macOS developer community
- CoreWLAN framework contributors
- SwiftUI Charts framework
- All users providing feedback and suggestions

---

**WiFi Diagnostics Report** • Professional Network Analysis • 2025 Jesus M. Ayala
