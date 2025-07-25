# Wifi Diagnostics Report

<img width="1023" alt="WifiApp" src="https://github.com/user-attachments/assets/3103d218-9c7b-4279-8b23-cdb0a489afcf" />

## Overview

**Wifi Diagnostics Report** is a professional-grade, free macOS app for WiFi/network diagnostics, system info, and technical troubleshooting.

Built for IT professionals, support staff, students, and power users, it empowers anyone to analyze their Mac's connectivity, scan WiFi, map coverage, check speeds, and export rich diagnostics with ease.

> **Note:** This app requires macOS 13.0 (Ventura) or newer.

---

## What's New - Version 4.0 Build 1.2

### **🚀 Real-Time Monitoring Performance Fixes (Latest)**
- **🆕 Fixed SwiftUI State Management** - Eliminated "Modifying state during view update" errors that caused undefined behavior
- **🆕 Optimized Chart Rendering** - Resolved filtering issues that prevented signal data from displaying in real-time charts
- **🆕 Enhanced Data Flow** - Streamlined filtering logic with proper computed property implementation for smooth UI updates
- **🆕 Improved User Interface Stability** - Fixed invalid SF Symbols and UI rendering issues for better visual consistency
- **🆕 Enhanced Debug Logging** - Comprehensive diagnostic output for troubleshooting real-time monitoring performance

### **📊 Enhanced Real-Time Signal Monitoring**
- **🆕 Smooth Chart Updates** - Fixed filtering algorithms to ensure all collected data points display correctly in charts
- **🆕 Proper Time Range Filtering** - "Last 1 minute", "Last 5 minutes", and "All data" options now work reliably
- **🆕 Performance Optimization** - Reduced computational overhead with intelligent caching and debouncing
- **🆕 Reliable Data Collection** - Enhanced timestamp handling ensures accurate time-based filtering
- **🆕 Visual Consistency** - Fixed chart rendering issues with proper RSSI value display and color coding

### **🔧 Technical Architecture Improvements**
- **🆕 SwiftUI Best Practices** - Eliminated state modifications during view updates following Apple's guidelines
- **🆕 Memory Optimization** - Improved data management for long-running monitoring sessions
- **🆕 Error Prevention** - Enhanced error handling and crash prevention in real-time monitoring
- **🆕 System Integration** - Better CoreWLAN framework integration with robust fallback mechanisms
- **🆕 UI/UX Polish** - Fixed visual inconsistencies and improved user feedback systems

### **📱 Enhanced WiFi Data Collection (Version 4.0)**
- **🆕 MCS Index Tracking** - Modulation and Coding Scheme analysis for precise data rate understanding
- **🆕 Spatial Streams (NSS) Detection** - Number of spatial streams monitoring for MIMO performance analysis
- **🆕 Channel Width Monitoring** - 20MHz, 40MHz, 80MHz, 160MHz channel width detection
- **🆕 PHY Mode Analysis** - 802.11n/ac/ax (Wi-Fi 4/5/6) protocol detection and reporting
- **🆕 Advanced System Profiler Integration** - Deep system-level WiFi metrics parsing for comprehensive analysis

---

## Features

- **Enhanced Dashboard** 
  - **🆕 Advanced WiFi Metrics Card** - Dedicated section showing MCS Index, Spatial Streams, Channel Width, PHY Mode, TX Rate, RSSI, Noise, and SNR
  - **Comprehensive system overview** with real-time network metrics
  - Quick action cards for common diagnostic tasks (Speed Test, Network Scan, Ping Test)
  - Recent activity tracking with historical test results
  - Connection status indicators with signal quality badges
  - Improved metric visualization and status indicators

- **Real-Time Device & Network Info**
  - Models, OS version (shown with marketing name & build), CPU/RAM, active interface, MAC/IP/DNS, WiFi details (SSID, channel, band, security)
  - **🆕 Advanced WiFi Metrics** - MCS Index, Spatial Streams (NSS), Channel Width, PHY Mode (802.11n/ac/ax)
  - Real-time network status monitoring with automatic refresh
  - Comprehensive system information collection
  - **Enhanced dashboard integration** with quick stats and system overview

- **Real-Time Signal Monitoring (Enhanced Build 1.2)** 
  - **🆕 Stable and reliable WiFi signal monitoring** with continuous 1-second updates and proper data display
  - **🆕 High-performance real-time charts** showing RSSI, noise levels, and signal-to-noise ratio with optimized rendering
  - **🆕 Enhanced Chart Display** - Smooth line graphs with proper scaling and reliable time-based filtering
  - **🆕 Robust time range controls** - "Last 1 minute", "Last 5 minutes", and "All data" filtering working correctly
  - Signal stability analysis with connection quality assessment
  - Trend detection (improving, stable, declining) over time
  - Export monitoring data to CSV for detailed analysis
  - Up to 5 minutes of historical data retention (300 data points)
  - Current signal status cards with real-time metrics
  - Signal variation analysis with stability ratings
  - **🆕 Performance optimized** with intelligent caching and reduced computational overhead

- **WiFi Scanner**
  - Instantly see all nearby SSIDs, signal quality, channels, security protocols, and export full scans to CSV/text
  - Advanced channel analysis and interference detection
  - Visual signal strength indicators with consistent color coding (Green=Excellent, Blue=Good, Orange=Fair, Red=Poor)
  - Network detail modal with comprehensive technical information
  - Multi-AP network analysis with roaming detection

- **Advanced Coverage Mapping**
  - Interactive floor plan upload and visualization with support for PNG, JPEG, PDF, SVG, TIFF formats
  - **🆕 Enhanced measurement data collection** - Each coverage point now records comprehensive WiFi metrics:
    - **RSSI** (Received Signal Strength Indicator) in dBm
    - **Noise Level** - Environmental noise measurement in dBm
    - **SNR** (Signal-to-Noise Ratio) in dB - Critical for signal quality assessment
    - **🆕 MCS Index** - Modulation and Coding Scheme for data rate analysis
    - **🆕 Spatial Streams (NSS)** - MIMO stream count for throughput optimization
    - **🆕 Channel Width** - 20MHz, 40MHz, 80MHz, 160MHz bandwidth detection
    - **🆕 PHY Mode** - 802.11n/ac/ax (Wi-Fi 4/5/6) protocol identification
    - **Channel and Band** information (2.4GHz, 5GHz, 6GHz)
    - **SSID and BSSID** for AP identification
    - **Timestamp** for temporal analysis
    - **Coordinates** for precise location tracking
  - Multiple coordinate tracking modes:
    - **Manual Entry** - Type coordinates directly
    - **Click to Select** - Point and click on map
    - **Live Mouse Tracking** - Real-time cursor following
    - **Grid Assistant** - Systematic measurement grid with customizable spacing
  - Full map transform support: zoom, rotate, pan with precise controls
  - Professional measurement point cards with signal quality indicators
  - **Enhanced context menu system** - Right-click coverage points for comprehensive options:
    - **"View Details"** - Shows detailed point information alert with complete signal data (RSSI, noise, SNR, MCS, NSS, PHY data), timestamps, and coordinates
    - **"Copy AP Info"** - Copies complete point information to clipboard including all metrics
    - **"Delete Point"** - Shows confirmation dialog for point removal
  - Built-in recommendations system with best practices guide
  - **Complete state persistence** - save and load coverage map projects with exact zoom/rotation/pan state
  - **🆕 Professional PDF export** with enhanced measurement data including MCS/NSS analysis and statistics
  - Signal quality legend and coverage statistics
  - Roaming event detection and analysis

- **Comprehensive Speed & Network Testing**
  - Visual download/upload speed tests with animated meters
  - Latency and packet loss analysis with real-time monitoring
  - Historical tracking of all test results with automatic logging
  - **"Run All Diagnostics"** - comprehensive automated testing suite with confirmation popup
  - **Full-screen diagnostic overlay** with animated progress indicator
  - Real-time progress indicators and detailed result breakdowns
  - Enhanced user feedback during test execution

- **Professional Export System**
  - Export all technical and user info, test results, and network scans
  - Multiple export formats (text reports, CSV data, PDF coverage maps)
  - **🆕 Enhanced coverage map data export** with complete MCS/NSS measurement points and transform state
  - High-quality PDF generation with professional layouts
  - Customizable export templates
  - **Enhanced export workflow** - app stays open after successful exports
  - **Success feedback** with clear confirmation messages
  - Real-time signal monitoring data export with advanced WiFi metrics

- **Modern Professional UI**
  - Enhanced welcome screen with animated feature cards
  - Modern sidebar with hover effects and smooth animations
  - Dynamic Light/Dark mode with professional color schemes
  - Color-blind friendly icons and accessibility features
  - **🆕 Improved visual consistency** with proper SF Symbol usage and UI polish
  - Extensive keyboard shortcuts and VoiceOver support
  - Adaptive layout for different screen sizes
  - Performance-optimized for large datasets
  - **Improved dashboard** with metric cards and quick actions

- **Advanced Customization**
  - Hide or show any sidebar feature for deployments
  - Configuration file-based customization (no code changes needed)
  - Perfect for enterprise deployments and non-technical users
  - **Updated configuration keys** for all current features

- **Advanced Technical Features**
  - **🆕 Enhanced WiFi Analysis** - Deep system profiler integration for MCS/NSS detection
  - **🆕 Optimized real-time monitoring** with proper SwiftUI state management and performance improvements
  - Advanced visualization with Charts framework and reliable data filtering
  - Comprehensive network diagnostics orchestration
  - Enhanced crash prevention and error handling
  - Professional-grade measurement accuracy
  - **Enhanced diagnostic flow** with better user feedback

- **Integrated Help & Documentation**
  - Comprehensive in-app help system
  - Step-by-step guides for all features
  - Coverage mapping best practices
  - Troubleshooting guides and technical explanations
  - **🆕 MCS/NSS technical documentation** and WiFi standard explanations
  - **Real-time monitoring usage guide**
  - **🆕 Performance troubleshooting** section for real-time monitoring issues

---

## Advanced WiFi Metrics Guide (New in v4.0)

### Understanding MCS Index
**Modulation and Coding Scheme (MCS)** determines the data rate and signal quality of your WiFi connection:

- **802.11n (Wi-Fi 4)**: MCS 0-31
  - MCS 0-7: 1 spatial stream
  - MCS 8-15: 2 spatial streams  
  - MCS 16-23: 3 spatial streams
  - MCS 24-31: 4 spatial streams

- **802.11ac (Wi-Fi 5)**: MCS 0-9 per spatial stream
  - Higher MCS = better signal quality and data rates
  - Requires good signal strength and low interference

- **802.11ax (Wi-Fi 6)**: MCS 0-11 per spatial stream
  - Most advanced with highest efficiency
  - Supports more devices and better performance

### Spatial Streams (NSS)
**Number of Spatial Streams** indicates MIMO capability:
- **1 Stream**: Basic connection, lower throughput
- **2 Streams**: Standard for most devices, good performance
- **3-4 Streams**: High-performance devices, maximum throughput
- **8+ Streams**: Enterprise/high-end equipment

### Channel Width Impact
**Bandwidth allocation affects performance**:
- **20MHz**: Basic, congested areas, longer range
- **40MHz**: Standard, good balance of speed and range
- **80MHz**: High speed, shorter range, less congested
- **160MHz**: Maximum speed, latest devices only

### PHY Mode Evolution
- **802.11n (Wi-Fi 4)**: Up to 600 Mbps, 2.4/5 GHz
- **802.11ac (Wi-Fi 5)**: Up to 6.9 Gbps, 5 GHz only
- **802.11ax (Wi-Fi 6)**: Up to 9.6 Gbps, 2.4/5/6 GHz, improved efficiency

### Professional Analysis Tips
1. **Monitor MCS Index**: Higher values indicate better signal quality
2. **Check Spatial Streams**: More streams = potential for higher throughput
3. **Optimize Channel Width**: Balance between speed and coverage
4. **Upgrade PHY Mode**: Newer standards provide better performance and efficiency
5. **Use Coverage Mapping**: Visualize how these metrics vary across your space

---

## Real-Time Signal Monitoring - Technical Details (Enhanced Build 1.2)

### **Live Monitoring Capabilities**
The real-time signal monitoring system provides continuous WiFi analysis with enhanced performance:

- **🆕 Optimized Performance**: Intelligent data filtering with proper computed properties and no state modifications during view updates
- **🆕 Reliable Chart Rendering**: Fixed SwiftUI architecture issues for consistent data display
- **🆕 Enhanced Time Filtering**: Proper timestamp handling for "Last 1 minute", "Last 5 minutes", and "All data" views
- **Update Frequency**: 1-second intervals for real-time feedback
- **Data Retention**: 300 data points (5 minutes of history)
- **Metrics Tracked**: RSSI, Noise Level, SNR, TX Rate, Signal Quality, MCS Index, Spatial Streams (NSS), Channel Width, PHY Mode, SSID, BSSID, Channel, Band
- **Performance**: Background processing to avoid UI blocking with optimized data management

### **Signal Analysis Features**
- **Signal Quality Calculation**: Automatic quality percentage based on RSSI ranges
- **Stability Assessment**: Standard deviation analysis for connection stability
- **Trend Detection**: Analyzes recent signal changes (improving, stable, declining)
- **Connection Quality**: Categorizes stability from "Excellent" to "Very Poor"
- **🆕 Advanced Metrics Integration**: Displays MCS Index, Spatial Streams, Channel Width, and PHY Mode in real-time

### **Export Capabilities**
- **CSV Export**: Complete monitoring session data with timestamps
- **🆕 Enhanced Data Fields**: All metrics including MCS/NSS data with ISO8601 timestamps for analysis
- **Integration**: Works with external analysis tools and spreadsheet applications

### **Performance Optimizations (Build 1.2)**
- **🆕 SwiftUI State Management**: Eliminated state modifications during view updates
- **🆕 Intelligent Caching**: Reduced computational overhead with smart data filtering
- **🆕 Memory Efficiency**: Improved data management for long-running sessions
- **🆕 Error Prevention**: Enhanced crash prevention and robust fallback mechanisms

---

## Enhanced Dashboard - Key Features

### **Real-Time Metrics**
- **🆕 Advanced WiFi Metrics Display**: MCS Index, Spatial Streams, Channel Width, PHY Mode with intelligent descriptions
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
The coverage mapping system includes **complete state persistence** when saving/loading projects:

- **Zoom level** - Exact scale factor preserved
- **Rotation angle** - Precise rotation state maintained  
- **Pan position** - Exact offset coordinates saved
- **Floor plan image** - High-quality image preservation
- **All measurement points** - Complete signal data and metadata including MCS/NSS metrics

When you save a coverage map project as JSON and reload it later, everything returns to exactly how you left it.

### **Professional PDF Export** 
Generate high-quality PDF reports with:
- Floor plan with measurement points overlaid
- **🆕 Enhanced measurement data** including MCS/NSS analysis and statistics
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

## Troubleshooting Guide (Updated Build 1.2)

### **Real-Time Monitoring Issues (Fixed in Build 1.2)**

#### **Chart Not Displaying Data** ✅ RESOLVED
- **Issue**: Signal data was being collected but charts showed "No signal data to display"
- **Cause**: SwiftUI state management issues and filtering problems
- **Fix**: Optimized data filtering logic and eliminated state modifications during view updates

#### **"Modifying state during view update" Errors** ✅ RESOLVED  
- **Issue**: Console warnings about undefined behavior
- **Cause**: State variables being modified inside computed properties during view rendering
- **Fix**: Redesigned filtering architecture with proper computed properties

#### **Time Range Filtering Not Working** ✅ RESOLVED
- **Issue**: "Last 1 minute" and "Last 5 minutes" showed no data despite data collection
- **Cause**: Timestamp comparison and filtering logic issues
- **Fix**: Enhanced timestamp handling and proper time-based filtering implementation

#### **Performance Issues** ✅ RESOLVED
- **Issue**: Excessive filtering calls and UI lag during monitoring
- **Cause**: Redundant data processing and inefficient state management
- **Fix**: Intelligent caching, debouncing, and optimized data flow

### **General Troubleshooting**

#### **WiFi Permissions**
- Ensure Location Services are enabled for WiFi scanning
- Grant necessary permissions when prompted
- Restart the app if permissions were recently changed

#### **Network Scanning Issues**
- Check that WiFi is enabled and connected
- Try refreshing the network scan
- Ensure no VPN or network restrictions are blocking scans

#### **Coverage Mapping Problems**
- Verify uploaded images are in supported formats (PNG, JPEG, PDF, SVG, TIFF)
- Check file permissions for uploaded floor plans
- Ensure sufficient disk space for project saves

#### **Export Problems**
- Verify write permissions to selected export location
- Check available disk space
- Try alternative export formats if one fails

#### **Performance Optimization**
- Close unnecessary apps during intensive monitoring sessions
- Reduce chart update frequency for older Macs if needed
- Use "Last 1 minute" view for real-time monitoring on lower-spec machines

---

## Recent Updates & Improvements

### **Version 4.0 Build 1.2 - Performance & Stability**

#### **Real-Time Monitoring Performance Fixes**
- **🆕 Fixed SwiftUI State Management** - Eliminated "Modifying state during view update" errors
- **🆕 Optimized Chart Rendering** - Resolved filtering issues preventing signal data display
- **🆕 Enhanced Data Flow** - Streamlined filtering logic with proper computed properties
- **🆕 Improved UI Stability** - Fixed invalid SF Symbols and rendering issues
- **🆕 Enhanced Debug Logging** - Comprehensive diagnostic output for troubleshooting

#### **Technical Architecture Improvements**
- **🆕 SwiftUI Best Practices** - Proper state management following Apple's guidelines
- **🆕 Memory Optimization** - Improved data management for long sessions
- **🆕 Error Prevention** - Enhanced crash prevention and error handling
- **🆕 System Integration** - Better CoreWLAN framework integration
- **🆕 UI/UX Polish** - Fixed visual inconsistencies and improved feedback

### **Version 4.0 Build 1.0 - Advanced WiFi Analytics**

#### **Enhanced WiFi Data Collection**
- **🆕 MCS Index Tracking** - Modulation and Coding Scheme analysis
- **🆕 Spatial Streams (NSS) Detection** - MIMO performance monitoring
- **🆕 Channel Width Monitoring** - 20MHz, 40MHz, 80MHz, 160MHz detection
- **🆕 PHY Mode Analysis** - 802.11n/ac/ax protocol identification
- **🆕 System Profiler Integration** - Deep system-level WiFi metrics

#### **Enhanced Coverage Mapping**
- **🆕 Extended Measurement Data** - MCS Index, Spatial Streams, Channel Width, PHY Mode
- **🆕 Advanced Point Information** - Comprehensive technical data display
- **🆕 Enhanced CSV Export** - Complete MCS/NSS/PHY field export
- **🆕 Professional WiFi Planning** - Enterprise-grade data collection

#### **Enhanced Dashboard Experience**
- **🆕 Advanced WiFi Metrics Card** - MCS descriptions and NSS analysis
- **🆕 Intelligent MCS Descriptions** - User-friendly explanations
- **🆕 NSS Stream Analysis** - Performance implications display
- **🆕 Real-Time Advanced Metrics** - Live monitoring of enhanced parameters

#### **Enhanced User Interface**
- **Fixed:** Right-click context menu in coverage mapping now properly shows "View Details" with comprehensive point information
- **Impact:** Improved user experience with correct context menu functionality

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

#### **Context Menu Functionality**
- **Fixed:** Coverage point right-click "View Details" now shows point information instead of attempting deletion
- **Impact:** Proper user interaction and context menu functionality

#### **Crash Prevention**
- **Fixed:** App no longer crashes when accessing roaming events with empty data
- **Impact:** Improved stability during coverage analysis

#### **Enhanced Data Collection**
- **Added:** Comprehensive WiFi metrics collection for coverage mapping including RSSI, noise levels, and SNR
- **Impact:** Professional-grade measurement data suitable for enterprise WiFi planning and analysis

#### **Advanced Signal Quality Analysis**
- **Added:** Noise floor measurements and signal-to-noise ratio calculations for each coverage point
- **Impact:** More accurate signal quality assessment and troubleshooting capabilities

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
