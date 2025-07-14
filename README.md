# Wifi Diagnostics Report

<img width="1680" height="1021" alt="WifiDiagReport" src="https://github.com/user-attachments/assets/a447d6ee-cf05-4acb-b280-9c05a8ff63ba" />

<img width="1676" height="1019" alt="Wifi Scanner" src="https://github.com/user-attachments/assets/76a61591-fe96-4f3c-ba9e-30516367eeca" />

## Overview

**Wifi Diagnostics Report** is a professional-grade, open-source macOS app for WiFi/network diagnostics, system info, and technical troubleshooting.

Built for IT professionals, support staff, students, and power users, it empowers anyone to analyze their Mac's connectivity, scan WiFi, map coverage, check speeds, and export rich diagnostics with ease.

> **Note:** This app requires macOS 13.0 (Ventura) or newer.

---

## ✨ What's New -

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

---

## Features

- 🌐 **Real-Time Device & Network Info**
  - Models, OS version (shown with marketing name & build), CPU/RAM, active interface, MAC/IP/DNS, WiFi details (SSID, channel, band, security)
  - Real-time network monitoring with automatic refresh capabilities

- 📡 **WiFi Scanner**
  - Instantly see all nearby SSIDs, signal quality, channels, security protocols, and export full scans to CSV/text
  - Advanced channel analysis and interference detection
  - **Consistent visual signal strength indicators** with professional color coding
  - Network detail modal with comprehensive technical information

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
  - "Run All Diagnostics" - comprehensive automated testing suite
  - Real-time progress indicators and detailed result breakdowns

- 📊 **Professional Export System**
  - Export all technical and user info, test results, and network scans
  - Multiple export formats (text reports, CSV data, **high-quality PDF coverage maps**)
  - Coverage map data export with complete measurement points and transform state
  - **🆕 MainActor-optimized PDF generation** for reliable exports
  - Customizable export templates

- 🎨 **Modern Professional UI**
  - Enhanced welcome screen with animated feature cards
  - Modern sidebar with hover effects and smooth animations
  - Dynamic Light/Dark mode with professional color schemes
  - **🆕 Consistent color-blind friendly icons** and accessibility features
  - Extensive keyboard shortcuts and VoiceOver support
  - Adaptive layout for different screen sizes
  - **🆕 Performance-optimized** for large datasets and complex interactions

- 🧑‍💻 **Advanced Customization**
  - Hide or show any sidebar feature for deployments
  - Configuration file-based customization (no code changes needed)
  - Perfect for enterprise deployments and non-technical users

- 🔧 **Advanced Technical Features**
  - Real-time WiFi monitoring and comprehensive analysis
  - Advanced visualization with Charts framework
  - Comprehensive network diagnostics orchestration
  - **🆕 Enhanced crash prevention** and error handling
  - Professional-grade measurement accuracy

- ❓ **Integrated Help & Documentation**
  - Comprehensive in-app help system
  - Step-by-step guides for all features
  - Coverage mapping best practices
  - Troubleshooting guides and technical explanations

---

## 🚀 Quick Start

### **Installation Requirements**
- macOS 13.0 (Ventura) or newer
- Admin privileges for some network diagnostics

### **Basic Usage**
1. **Launch the app** - Modern welcome screen guides you through features
2. **Device Info** - View comprehensive system information
3. **WiFi Scanner** - Scan and analyze nearby networks
4. **Coverage Mapping** - Upload floor plans and create professional signal maps
5. **Speed Testing** - Run comprehensive network performance tests
6. **Export** - Generate professional reports and data exports

### **Coverage Mapping Workflow** 🗺️
1. **Upload Floor Plan** - Drag & drop or select PNG, JPEG, PDF, SVG, TIFF files
2. **Choose Tracking Mode** - Manual, click, live, or **Grid Assistant** (recommended)
3. **Take Measurements** - Click locations to record real-time WiFi signal data
4. **Transform & Analyze** - Zoom, rotate, pan for perfect alignment
5. **Export Data** - Save as JSON project (with complete state) or generate PDF report

<img width="1676" height="1025" alt="Converage Mapping" src="https://github.com/user-attachments/assets/0488cc4b-f4a6-42c5-a642-64d821dd0740" />

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
