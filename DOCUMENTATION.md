# Wifi Diagnostics Report

<img width="1023" alt="WifiApp" src="https://github.com/user-attachments/assets/3103d218-9c7b-4279-8b23-cdb0a489afcf" />

## Overview

**Wifi Diagnostics Report** is a professional-grade, open-source macOS app for WiFi/network diagnostics, system info, and technical troubleshooting.

Built for IT professionals, support staff, students, and power users, it empowers anyone to analyze their Mac's connectivity, scan WiFi, map coverage, check speeds, and export rich diagnostics with ease.

> **Note:** This app requires macOS 13.0 (Ventura) or newer.

---

## Features

- 🎯 **Enhanced Dashboard** ⭐
  - **🆕 Comprehensive system overview** with real-time network metrics
  - Quick action cards for common diagnostic tasks (Speed Test, Network Scan, Ping Test)
  - Recent activity tracking with historical test results
  - Connection status indicators with signal quality badges
  - Improved metric visualization and status indicators

- 🌐 **Real-Time Device & Network Info**
  - Models, OS version (shown with marketing name & build), CPU/RAM, active interface, MAC/IP/DNS, WiFi details (SSID, channel, band, security)
  - Real-time network status monitoring with automatic refresh
  - Comprehensive system information collection
  - **🆕 Enhanced dashboard integration** with quick stats and system overview

- 📊 **Real-Time Signal Monitoring** ⭐
  - **🆕 Live WiFi signal monitoring** with continuous 1-second updates
  - Real-time charts showing RSSI, noise levels, and signal-to-noise ratio
  - Signal stability analysis with connection quality assessment
  - Trend detection (improving, stable, declining) over time
  - Export monitoring data to CSV for detailed analysis
  - Up to 5 minutes of historical data retention (300 data points)
  - Current signal status cards with real-time metrics
  - Signal variation analysis with stability ratings

- 📡 **WiFi Scanner**
  - Instantly see all nearby SSIDs, signal quality, channels, security protocols, and export full scans to CSV/text
  - Advanced channel analysis and interference detection
  - Visual signal strength indicators with consistent color coding (Green=Excellent, Blue=Good, Orange=Fair, Red=Poor)
  - Network detail modal with comprehensive technical information
  - Multi-AP network analysis with roaming detection

- 🗺️ **Advanced Coverage Mapping**
  - Interactive floor plan upload and visualization with support for PNG, JPEG, PDF, SVG, TIFF formats
  - Multiple coordinate tracking modes:
    - **Manual Entry** - Type coordinates directly
    - **Click to Select** - Point and click on map
    - **Live Mouse Tracking** - Real-time cursor following
    - **Grid Assistant** - Systematic measurement grid with customizable spacing
  - Full map transform support: zoom, rotate, pan with precise controls
  - Professional measurement point cards with signal quality indicators
  - Built-in recommendations system with best practices guide
  - **Complete state persistence** - save and load coverage map projects with exact zoom/rotation/pan state
  - Export coverage maps as high-quality PDFs with measurement data
  - Signal quality legend and coverage statistics
  - Roaming event detection and analysis

- 🚦 **Comprehensive Speed & Network Testing**
  - Visual download/upload speed tests with animated meters
  - Latency and packet loss analysis with real-time monitoring
  - Historical tracking of all test results with automatic logging
  - **🆕 "Run All Diagnostics"** - comprehensive automated testing suite with confirmation popup
  - **🆕 Full-screen diagnostic overlay** with animated progress indicator
  - Real-time progress indicators and detailed result breakdowns
  - Enhanced user feedback during test execution

- 📊 **Professional Export System**
  - Export all technical and user info, test results, and network scans
  - Multiple export formats (text reports, CSV data, PDF coverage maps)
  - Coverage map data export with complete measurement points and metadata
  - High-quality PDF generation with professional layouts
  - Customizable export templates
  - **🆕 Enhanced export workflow** - app stays open after successful exports
  - **🆕 Success feedback** with clear confirmation messages
  - Real-time signal monitoring data export

- 🎨 **Modern Professional UI**
  - Enhanced welcome screen with animated feature cards
  - Modern sidebar with hover effects and smooth animations
  - Dynamic Light/Dark mode with professional color schemes
  - Color-blind friendly icons and accessibility features
  - Extensive keyboard shortcuts and VoiceOver support
  - Adaptive layout for different screen sizes
  - Performance-optimized for large datasets
  - **🆕 Improved dashboard** with metric cards and quick actions

- 🧑‍💻 **Advanced Customization**
  - Hide or show any sidebar feature for deployments
  - Configuration file-based customization (no code changes needed)
  - Perfect for enterprise deployments and non-technical users
  - **🆕 Updated configuration keys** for all current features

- 🔧 **Advanced Technical Features**
  - Real-time WiFi monitoring and analysis
  - Advanced visualization with Charts framework
  - Comprehensive network diagnostics orchestration
  - Crash prevention and error handling
  - MainActor-optimized PDF generation
  - **🆕 Enhanced diagnostic flow** with better user feedback

- ❓ **Integrated Help & Documentation**
  - Comprehensive in-app help system
  - Step-by-step guides for all features
  - Coverage mapping best practices
  - Troubleshooting guides and technical explanations
  - **🆕 Real-time monitoring usage guide**

---

## Real-Time Signal Monitoring - Technical Details

### **Live Monitoring Capabilities**
The real-time signal monitoring system provides continuous WiFi analysis:

- **Update Frequency**: 1-second intervals for real-time feedback
- **Data Retention**: 300 data points (5 minutes of history)
- **Metrics Tracked**: RSSI, Noise Level, SNR, TX Rate, Signal Quality, SSID, BSSID, Channel, Band
- **Performance**: Background processing to avoid UI blocking

### **Signal Analysis Features**
- **Signal Quality Calculation**: Automatic quality percentage based on RSSI ranges
- **Stability Assessment**: Standard deviation analysis for connection stability
- **Trend Detection**: Analyzes recent signal changes (improving, stable, declining)
- **Connection Quality**: Categorizes stability from "Excellent" to "Very Poor"

### **Export Capabilities**
- **CSV Export**: Complete monitoring session data with timestamps
- **Data Fields**: All metrics with ISO8601 timestamps for analysis
- **Integration**: Works with external analysis tools and spreadsheet applications

---

## Enhanced Dashboard - Key Features

### **Real-Time Metrics**
- **Connection Status**: Current network connection with signal quality
- **Signal Strength**: Live RSSI values with quality indicators
- **Speed Test Results**: Latest download/upload speeds
- **Network Count**: Available networks from recent scans

### **Quick Actions**
- **Speed Test**: Direct access to speed testing
- **Network Scan**: Immediate WiFi network scanning
- **Ping Test**: Quick latency testing
- **Refresh Network**: Update all network information

### **Recent Activity**
- **Test History**: Latest diagnostic results with timestamps
- **Visual Indicators**: Color-coded status badges
- **Quick Access**: Direct links to detailed views

---

## Coverage Mapping - Advanced Features

### **Complete State Persistence** 
The coverage mapping system now includes **complete state persistence** when saving/loading projects:

- **Zoom level** - Exact scale factor preserved
- **Rotation angle** - Precise rotation state maintained  
- **Pan position** - Exact offset coordinates saved
- **Floor plan image** - High-quality image preservation
- **All measurement points** - Complete signal data and metadata

When you save a coverage map project as JSON and reload it later, everything returns to exactly how you left it.

### **Professional PDF Export** 
Generate high-quality PDF reports with:
- Floor plan with measurement points overlaid
- Signal quality statistics and analysis
- Comprehensive measurement data tables
- Professional formatting and layout

### **Grid Assistant** 
The Grid Assistant provides systematic measurement coverage:
- Customizable grid spacing (30px to 100px)
- Visual grid overlay on floor plans
- Ensures complete coverage analysis
- Perfect for professional site surveys

---

## Enhanced Diagnostic Flow

### **"Run All Diagnostics" Workflow**
The comprehensive diagnostic system includes:

1. **Confirmation Popup**: "Run All Diagnostics" alert with detailed description
2. **Start Analysis Button**: Initiates the full diagnostic suite
3. **Full-Screen Overlay**: Animated progress indicator covering entire app
4. **Concurrent Testing**: Speed, latency, and packet loss tests run simultaneously
5. **Export Prompt**: Automatic suggestion to export results when complete

### **Progress Visualization**
- **Animated Spinner**: Continuous rotation with app theme colors
- **Professional Layout**: Clear messaging and progress indication
- **Non-Blocking**: App remains responsive during testing
- **Status Updates**: Real-time feedback on test progress

---

## Recent Updates & Improvements

### **January 2025 Updates** 

#### **Real-Time Signal Monitoring**
- **Added:** Complete real-time WiFi monitoring with 1-second updates
- **Impact:** Professional-grade network monitoring capabilities

#### **Enhanced Dashboard**
- **Added:** Comprehensive dashboard with real-time metrics and quick actions
- **Impact:** Improved user experience with centralized system overview

#### **Improved Diagnostic Flow**
- **Restored:** "Run All Diagnostics" workflow with confirmation popup and progress overlay
- **Impact:** Better user feedback and professional diagnostic experience

#### **Enhanced Export System**
- **Fixed:** App now stays open after successful exports
- **Impact:** Improved workflow continuity and user experience

#### **JSON Export/Import State Persistence**
- **Fixed:** Coverage maps now remember zoom, rotation, and pan state when saved/loaded
- **Impact:** Perfect project restoration for professional workflows

#### **Performance Optimizations**
- **Fixed:** Large coverage map files now compile and render efficiently
- **Impact:** Improved app responsiveness with complex floor plans

#### **PDF Export Enhancement**
- **Fixed:** PDF exports now generate proper content instead of blank pages
- **Impact:** Professional reporting capabilities restored

#### **Signal Quality Color Consistency**
- **Fixed:** "Excellent" signals now consistently show green across all UI components
- **Impact:** Improved visual consistency and user experience

#### **Crash Prevention**
- **Fixed:** App no longer crashes when accessing roaming events with empty data
- **Impact:** Improved stability during coverage analysis

---

## Sidebar Customization (for Techs, Admins, Deployments)

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
    <key>HideDeviceInfo</key>
    <true/>
    <key>HideWifiScanner</key>
    <false/>
    <key>HideCoverageMapping</key>
    <false/>
    <key>HideSpeedTesting</key>
    <false/>
    <key>HideExportSystem</key>
    <false/>
    <key>HideCustomization</key>
    <true/>
    <key>HideTechnicalFeatures</key>
    <false/>
    <key>HideHelpAndDocumentation</key>
    <false/>
</dict>
</plist>