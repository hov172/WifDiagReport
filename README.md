# Wifi Diagnostics Report

<img width="1677" height="1025" alt="main" src="https://github.com/user-attachments/assets/4b0a9eb4-ea3f-4f7f-86e8-c4addf526ccb" />

<img width="1677" height="1018" alt="Scanning" src="https://github.com/user-attachments/assets/edd07ba4-cc55-4d22-8000-108b56ca9422" />

## Overview

**Wifi Diagnostics Report** is a professional-grade, free macOS app for WiFi/network diagnostics, system info, and technical troubleshooting.

Built for IT professionals, support staff, students, and power users, it empowers anyone to analyze their Mac's connectivity, scan WiFi, map coverage, check speeds, and export rich diagnostics with ease.

> **Note:** This app requires macOS 13.0 (Ventura) or newer.

---

## What's New

### Version 4.0 Build 1.2 - Performance Optimizations & Stability Improvements

#### **🚀 Real-Time Monitoring Performance Fixes (NEW)**
- **🆕 Fixed SwiftUI State Management** - Eliminated "Modifying state during view update" errors that caused undefined behavior
- **🆕 Optimized Chart Rendering** - Resolved filtering issues that prevented signal data from displaying in real-time charts
- **🆕 Enhanced Data Flow** - Streamlined filtering logic with proper computed property implementation for smooth UI updates
- **🆕 Improved User Interface Stability** - Fixed invalid SF Symbols and UI rendering issues for better visual consistency
- **🆕 Enhanced Debug Logging** - Comprehensive diagnostic output for troubleshooting real-time monitoring performance

#### **📊 Enhanced Real-Time Signal Monitoring**
- **🆕 Smooth Chart Updates** - Fixed filtering algorithms to ensure all collected data points display correctly in charts
- **🆕 Proper Time Range Filtering** - "Last 1 minute", "Last 5 minutes", and "All data" options now work reliably
- **🆕 Performance Optimization** - Reduced computational overhead with intelligent caching and debouncing
- **🆕 Reliable Data Collection** - Enhanced timestamp handling ensures accurate time-based filtering
- **🆕 Visual Consistency** - Fixed chart rendering issues with proper RSSI value display and color coding

#### **🔧 Technical Architecture Improvements**
- **🆕 SwiftUI Best Practices** - Eliminated state modifications during view updates following Apple's guidelines
- **🆕 Memory Optimization** - Improved data management for long-running monitoring sessions
- **🆕 Error Prevention** - Enhanced error handling and crash prevention in real-time monitoring
- **🆕 System Integration** - Better CoreWLAN framework integration with robust fallback mechanisms
- **🆕 UI/UX Polish** - Fixed visual inconsistencies and improved user feedback systems

### Version 4.0 Build 1.0 - Advanced WiFi Analytics & Enhanced Data Collection

#### **🚀 Enhanced WiFi Data Collection**
- **🆕 MCS Index Tracking** - Modulation and Coding Scheme analysis for precise data rate understanding
- **🆕 Spatial Streams (NSS) Detection** - Number of spatial streams monitoring for MIMO performance analysis
- **🆕 Channel Width Monitoring** - 20MHz, 40MHz, 80MHz, 160MHz channel width detection
- **🆕 PHY Mode Analysis** - 802.11n/ac/ax (Wi-Fi 4/5/6) protocol detection and reporting
- **🆕 Advanced System Profiler Integration** - Deep system-level WiFi metrics parsing for comprehensive analysis

#### **📊 Enhanced Coverage Mapping**
- **🆕 Extended Measurement Data** - Coverage points now capture MCS Index, Spatial Streams, Channel Width, and PHY Mode
- **🆕 Advanced Point Information** - Comprehensive technical data display in coverage point cards and popups
- **🆕 Enhanced CSV Export** - Updated data export includes all new MCS/NSS/PHY fields for professional analysis
- **🆕 Professional WiFi Planning** - Enterprise-grade data collection suitable for RF planning and optimization

#### **🎛️ Enhanced Dashboard Experience**
- **🆕 Advanced WiFi Metrics Card** - Dedicated section showing MCS Index, Spatial Streams, Channel Width, PHY Mode, TX Rate, RSSI, Noise, and SNR
- **🆕 Intelligent MCS Descriptions** - User-friendly explanations of Modulation and Coding Scheme values
- **🆕 NSS Stream Analysis** - Clear spatial stream information with performance implications
- **🆕 Real-Time Advanced Metrics** - Live monitoring of all enhanced WiFi parameters

#### **🔧 Technical Enhancements**
- **🆕 Hardened Runtime Support** - Enhanced security and compatibility for macOS deployment
- **🆕 System Profiler Parser** - Advanced parsing of macOS system_profiler WiFi data for detailed network information
- **🆕 Robust Error Handling** - Improved fallback mechanisms for MCS/NSS data when unavailable
- **🆕 Performance Optimization** - Enhanced data collection efficiency with minimal system impact

### Complete State Persistence
- **Coverage maps now remember zoom, rotation, and pan state** when saved/loaded
- Perfect project restoration for professional workflows

### Enhanced User Interface
- **Fixed right-click context menu** in coverage mapping - "View Details" now properly shows point information instead of attempting deletion
- **Improved context menu organization** with proper action routing for "View Details", "Copy AP Info", and "Delete Point"
- Enhanced point information display with comprehensive signal data, timestamps, and coordinates

### Professional PDF Export
- High-quality PDF generation with measurement data and floor plans
- Professional layouts with statistics and analysis

### Performance Optimizations
- Improved app responsiveness with complex floor plans and large datasets
- Enhanced compilation times and stability
- **🆕 Real-time monitoring performance improvements** with optimized data filtering and chart rendering

### Visual Consistency
- Signal quality colors now consistent across all UI components
- Green=Excellent, Blue=Good, Orange=Fair, Red=Poor
- **🆕 Fixed UI elements** with proper SF Symbol usage and visual polish

### Enhanced Stability
- Crash prevention and error handling improvements
- Better handling of edge cases and empty data
- **Fixed context menu callback routing** for proper user interaction
- **🆕 SwiftUI stability improvements** with proper state management and view lifecycle handling

### Real-Time Signal Monitoring
- **Live WiFi signal monitoring** with 1-second interval updates
- **🆕 Reliable real-time charts** showing signal strength, noise levels, and SNR with proper data display
- **🆕 Enhanced time range filtering** with "Last 1 minute", "Last 5 minutes", and "All data" options working correctly
- Signal stability analysis with trend detection
- Export capability for long-term monitoring data
- **🆕 Performance optimized** with reduced computational overhead and smooth UI updates

### Improved Diagnostic Flow
- **Restored "Run All Diagnostics" workflow** with confirmation popup
- Full-screen diagnostic overlay with animated progress indicator
- Better user feedback during test execution
- Enhanced export process that keeps app open after file saves

### Enhanced Dashboard
- **Comprehensive dashboard view** with real-time network metrics
- Quick action cards for common diagnostic tasks
- Recent activity tracking and system overview
- Improved metric visualization and status indicators

### **📊 Enhanced Data Collection**
- **🆕 Comprehensive WiFi metrics collection** for coverage mapping including RSSI, noise levels, and SNR
- **🆕 Advanced signal quality analysis** with noise floor measurements and signal-to-noise ratios
- **🆕 Professional measurement data** suitable for enterprise WiFi planning and troubleshooting

### **🔧 Enhanced User Interface**
- **🆕 Fixed right-click context menu** in coverage mapping - "View Details" now properly shows point information instead of attempting deletion
- **🆕 Improved context menu organization** with proper action routing for "View Details", "Copy AP Info", and "Delete Point"
- **🆕 Enhanced point information display** with comprehensive signal data including SNR and noise levels, timestamps, and coordinates

---

## Features

- Real-Time Device & Network Info
  - Models, OS version (shown with marketing name & build), CPU/RAM, active interface, MAC/IP/DNS, WiFi details (SSID, channel, band, security)
  - **🆕 Advanced WiFi Metrics** - MCS Index, Spatial Streams (NSS), Channel Width, PHY Mode (802.11n/ac/ax)
  - Real-time network monitoring with automatic refresh capabilities
  - Enhanced dashboard with quick stats and system overview

- WiFi Scanner
  - Instantly see all nearby SSIDs, signal quality, channels, security protocols, and export full scans to CSV/text
  - Advanced channel analysis and interference detection
  - Consistent visual signal strength indicators with professional color coding
  - Network detail modal with comprehensive technical information
  - Multi-AP network analysis with roaming detection

- Real-Time Signal Monitoring 
  - **🆕 Stable and reliable WiFi signal monitoring** with continuous 1-second updates and proper data display
  - **🆕 High-performance real-time charts** showing RSSI, noise levels, and signal-to-noise ratio with optimized rendering
  - **🆕 Enhanced Chart Display** - Smooth line graphs with proper scaling and reliable time-based filtering
  - **🆕 Robust time range controls** - "Last 1 minute", "Last 5 minutes", and "All data" filtering working correctly
  - Signal stability analysis with connection quality assessment
  - Trend detection (improving, stable, declining) over time
  - Export monitoring data to CSV for detailed analysis
  - Up to 5 minutes of historical data retention (300 data points)
  - **🆕 Performance optimized** with intelligent caching and reduced computational overhead

- Advanced Coverage Mapping 
  - Interactive floor plan upload and visualization with support for PNG, JPEG, PDF, SVG, TIFF formats
  - **🆕 Enhanced measurement data collection** - Each coverage point now records comprehensive WiFi metrics:
    - RSSI (Received Signal Strength Indicator)
    - Noise Level - Environmental noise measurement
    - SNR (Signal-to-Noise Ratio) - Signal quality indicator
    - **🆕 MCS Index** - Modulation and Coding Scheme for data rate analysis
    - **🆕 Spatial Streams (NSS)** - MIMO stream count for throughput optimization
    - **🆕 Channel Width** - 20MHz, 40MHz, 80MHz, 160MHz bandwidth detection
    - **🆕 PHY Mode** - 802.11n/ac/ax (Wi-Fi 4/5/6) protocol identification
    - Channel and Band information
    - Timestamp and Location data
  - Multiple coordinate tracking modes:
    - Manual Entry - Type coordinates directly
    - Click to Select - Point and click on map
    - Live Mouse Tracking - Real-time cursor following
    - Grid Assistant - Systematic measurement grid with customizable spacing
  - Full map transform support: zoom, rotate, pan with precise controls
  - Professional measurement point cards with signal quality indicators
  - **🆕 Enhanced context menu** - Right-click coverage points for "View Details" (comprehensive point information including MCS, NSS, and PHY data), "Copy AP Info" (clipboard export), and "Delete Point" (confirmation dialog)
  - Built-in recommendations system with best practices guide
  - Complete state persistence - save and load coverage map projects with exact zoom/rotation/pan state
  - **🆕 Professional PDF export** with enhanced measurement data including MCS/NSS analysis and statistics
  - Signal quality legend and coverage statistics
  - Roaming event detection and analysis

- Comprehensive Speed & Network Testing
  - Visual download/upload speed tests with animated meters
  - Latency and packet loss analysis with real-time monitoring
  - Historical tracking of all test results with automatic logging
  - Restored "Run All Diagnostics" - comprehensive automated testing suite with confirmation popup
  - Full-screen diagnostic overlay with animated progress indicator
  - Real-time progress indicators and detailed result breakdowns

- Professional Export System
  - Export all technical and user info, test results, and network scans
  - Multiple export formats (text reports, CSV data, high-quality PDF coverage maps)
  - **🆕 Enhanced coverage map data export** with complete MCS/NSS measurement points and transform state
  - MainActor-optimized PDF generation for reliable exports
  - Enhanced export workflow - app stays open after successful exports
  - Customizable export templates with user and location information
  - Real-time signal monitoring data export with advanced WiFi metrics

- Modern Professional UI
  - **🆕 Enhanced dashboard** with Advanced WiFi Metrics card showing MCS descriptions and NSS analysis
  - Enhanced welcome screen with animated feature cards
  - Modern sidebar with hover effects and smooth animations
  - Dynamic Light/Dark mode with professional color schemes
  - Consistent color-blind friendly icons and accessibility features
  - **🆕 Improved visual consistency** with proper SF Symbol usage and UI polish
  - Extensive keyboard shortcuts and VoiceOver support
  - Adaptive layout for different screen sizes
  - Performance-optimized for large datasets and complex interactions
  - Improved dashboard with metric cards and quick actions

- Advanced Customization
  - Hide or show any sidebar feature for deployments
  - Configuration file-based customization (no code changes needed)
  - Perfect for enterprise deployments and non-technical users
  - Updated configuration keys for all current features

- Advanced Technical Features
  - **🆕 Enhanced WiFi Analysis** - Deep system profiler integration for MCS/NSS detection
  - **🆕 Optimized real-time monitoring** with proper SwiftUI state management and performance improvements
  - Advanced visualization with Charts framework and reliable data filtering
  - Comprehensive network diagnostics orchestration
  - Enhanced crash prevention and error handling
  - Professional-grade measurement accuracy
  - Improved diagnostic flow with better user feedback

- Integrated Help & Documentation
  - Comprehensive in-app help system
  - Step-by-step guides for all features
  - Coverage mapping best practices
  - Troubleshooting guides and technical explanations
  - **🆕 MCS/NSS technical documentation** and WiFi standard explanations
  - Real-time monitoring usage guide
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

## Quick Start

### Installation Requirements
- macOS 13.0 (Ventura) or newer
- Admin privileges for some network diagnostics

### Basic Usage
1. Launch the app - Modern welcome screen guides you through features
2. **🆕 Enhanced Dashboard** - View comprehensive system overview with real-time metrics including Advanced WiFi Metrics (MCS Index, Spatial Streams, Channel Width, PHY Mode)
3. Device Info - View comprehensive system information (integrated into dashboard)
4. WiFi Scanner - Scan and analyze nearby networks
5. **🆕 Real-Time Monitor** - Monitor WiFi signal quality in real-time with stable, high-performance chart visualization
6. **🆕 Enhanced Coverage Mapping** - Upload floor plans and create professional signal maps with MCS/NSS data collection
7. Speed Testing - Run comprehensive network performance tests
8. **🆕 Enhanced Export** - Generate professional reports with advanced WiFi analytics

### Coverage Mapping Workflow 
1. Upload Floor Plan - Drag & drop or select PNG, JPEG, PDF, SVG, TIFF files
2. Choose Tracking Mode - Manual, click, live, or Grid Assistant (recommended)
3. **🆕 Enhanced Measurements** - Click locations to record comprehensive WiFi data including MCS Index, Spatial Streams, Channel Width, and PHY Mode
4. Transform & Analyze - Zoom, rotate, pan for perfect alignment
5. **🆕 Advanced Export** - Save as JSON project (with complete state) or generate PDF report with MCS/NSS analysis

### Real-Time Signal Monitoring Workflow 
1. Navigate to Real-time Monitor - Select from sidebar
2. Start Monitoring - Click "Start Monitoring" button
3. **🆕 Reliable Visualization** - Watch real-time charts with stable data display, smooth line graphs, and proper time-based filtering
4. **🆕 Time Range Controls** - Switch between "Last 1 minute", "Last 5 minutes", and "All data" views for different analysis perspectives
5. Analyze Trends - Monitor signal stability, variation, and connection quality
6. **🆕 Advanced Export** - Save monitoring session data as CSV with MCS/NSS metrics for analysis

### Advanced WiFi Analysis (New in v4.0)
1. **MCS Index Monitoring** - Track Modulation and Coding Scheme for data rate optimization
2. **Spatial Streams Analysis** - Monitor MIMO stream count for throughput analysis
3. **Channel Width Detection** - Identify 20MHz, 40MHz, 80MHz, 160MHz configurations
4. **PHY Mode Identification** - Detect Wi-Fi 4/5/6 (802.11n/ac/ax) protocols
5. **Professional Data Export** - All advanced metrics included in coverage mapping and monitoring exports

---

## Troubleshooting

### Real-Time Monitoring Issues (Fixed in Build 1.2)

#### **Chart Not Displaying Data** 
- **Issue**: Signal data was being collected but charts showed "No signal data to display"
- **Cause**: SwiftUI state management issues and filtering problems
- **Fix**: Optimized data filtering logic and eliminated state modifications during view updates

#### **"Modifying state during view update" Errors** 
- **Issue**: Console warnings about undefined behavior
- **Cause**: State variables being modified inside computed properties during view rendering
- **Fix**: Redesigned filtering architecture with proper computed properties

#### **Time Range Filtering Not Working** 
- **Issue**: "Last 1 minute" and "Last 5 minutes" showed no data despite data collection
- **Cause**: Timestamp comparison and filtering logic issues
- **Fix**: Enhanced timestamp handling and proper time-based filtering implementation

#### **Performance Issues** 
- **Issue**: Excessive filtering calls and UI lag during monitoring
- **Cause**: Redundant data processing and inefficient state management
- **Fix**: Intelligent caching, debouncing, and optimized data flow

### General Troubleshooting

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

## Sidebar Customization (for Techs, Admins, Deployments)

Wifi Diagnostics Report makes it easy for technical users to toggle feature visibility for non-technical end-users—without code changes or custom builds.

### How It Works

The app loads a bundled configuration file:  
WifiDialogReport/Configuration.plist

This file uses keys of the form HideXXXX for each feature or tool in the sidebar.

- Set the value to <true/> to hide a sidebar section or tool
- Set the value to <false/> to show that section/tool

#### Example: Configuration.plist
```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
    <key>HideDashboard</key>
    <false/>
    <key>HideNetworkScanner</key>
    <false/>
    <key>HideSpeedTest</key>
    <false/>
    <key>HideCoverageMap</key>
    <false/>
    <key>HideNetworkHistory</key>
    <false/>
    <key>HideReal-timeMonitor</key>
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
| HideDashboard |  Hide dashboard overview | false |
| HideNetworkScanner | Hide WiFi scanner tool | false |
| HideSpeedTest | Hide speed testing tool | false |
| HideCoverageMap | Hide coverage mapping tool | false |
| HideNetworkHistory | Hide network test history | false |
| HideReal-timeMonitor |  Hide real-time signal monitoring | false |
| HideHelp | Hide help documentation | false |
| HideExport | Hide export functionality | false |
| HideRunAll | Hide "Run All Tests" button | false |
| HideDebugExport | Hide debug export option | true |

### Updated Configuration
The configuration system has been updated to match all current sidebar sections and features. Make sure to use the exact key names shown above (including spaces) for proper functionality.

---

## Technical Details

### Real-Time Signal Monitoring
- Update Frequency: 1-second intervals
- Data Retention: 300 data points (5 minutes)
- Metrics Tracked: RSSI, Noise Level, SNR, TX Rate, Signal Quality, MCS Index, Spatial Streams (NSS), Channel Width, PHY Mode
- Export Format: CSV with timestamps and all measured parameters
- Performance: Background processing to avoid UI blocking

### Enhanced Diagnostic Flow
- Confirmation Popup: Shows before running comprehensive diagnostics
- Progress Overlay: Full-screen animated indicator during test execution
- Concurrent Testing: Speed, latency, and packet loss tests run simultaneously
- Export Integration: Automatic prompt to export results after completion

### Improved Export System
- App Persistence: Application remains open after successful exports
- Success Feedback: Clear confirmation messages with file information
- Error Handling: Detailed error messages for troubleshooting
- Multiple Formats: Text reports, CSV data, and PDF coverage maps

### Real-Time Signal Monitoring 
- **🆕 Enhanced Chart Display** - Smooth line graphs with proper scaling and time-based filtering
- Update Frequency: 1-second intervals
- Data Retention: 300 data points (5 minutes)
- Metrics Tracked: RSSI, Noise Level, SNR, TX Rate, Signal Quality, MCS Index, Spatial Streams (NSS), Channel Width, PHY Mode
- Export Format: CSV with timestamps and all measured parameters
- Performance: Background processing to avoid UI blocking

---

## Contributing

We welcome contributions! Whether you're fixing bugs, adding features, or improving documentation, your help makes this tool better for everyone.

### Development Setup
1. Clone the repository
2. Open Wifi Diagnostics Report.xcodeproj in Xcode
3. Build and run (requires macOS 13.0+)

### Feature Areas
- Real-time monitoring enhancements
- Additional export formats
- Advanced network analysis
- UI/UX improvements
- Performance optimizations

---

## Acknowledgments

Built with for the macOS community, IT professionals, and anyone who needs reliable network diagnostics.

Special thanks to:
- The macOS developer community
- CoreWLAN framework contributors
- SwiftUI Charts framework
- All users providing feedback and suggestions
- For their contributions and support, making Wifi Diagnostics Report version 4.0 a better and more powerful tool for advanced WiFi analytics and network troubleshooting.
