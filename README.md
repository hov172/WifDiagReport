# 📡 WiFi Diag Report

**Professional Wi-Fi diagnostics, network analysis, coverage mapping, and Help Desk reporting for macOS.**

WiFi Diag Report is a free macOS application designed for Wi-Fi and network diagnostics, system information retrieval, coverage analysis, and technical troubleshooting.

Built for **IT professionals, Help Desk teams, students, and power users**, the application can analyze a Mac's connectivity, scan surrounding wireless networks, monitor signal quality, test network performance, map Wi-Fi coverage, and generate detailed diagnostic reports.

> **System Requirement:** macOS 13.0 (Ventura) or newer.

---

## 🎯 Intended Use

WiFi Diag Report enables IT staff to perform Wi-Fi tests and export detailed reports that can help identify interference, weak coverage, performance problems, configuration issues, and other potential causes of connectivity problems.

### 🏫 Help Desk / Higher Education Workflow

In my current environment at a small college, we use a customized version of WiFi Diag Report designed specifically for student troubleshooting.

Advanced IT-level tools can be hidden while still allowing students or other end users to:

1. Run approved Wi-Fi and network diagnostics.
2. Collect device and connection information.
3. Generate a standardized diagnostic report.
4. Email the report to the Help Desk.

The report gives IT staff a useful technical baseline before dispatching a technician or an IT-managed computer to the reported location for comparison testing.

This helps determine whether a problem is related to:

* The student's device
* Wi-Fi signal strength
* Access point coverage
* Network performance
* Wireless interference
* Device hardware capabilities
* Configuration
* The surrounding RF environment

Feature visibility can be controlled through the application's `Configuration.plist`, allowing organizations to create simplified deployments without maintaining a separate application build.

---

# 🌐 Multi-Platform Wi-Fi Analyzer Project

WiFi Diag Report is part of a larger collection of Wi-Fi diagnostic tools I have developed for **PowerShell, Windows, macOS, and iOS/iPadOS**.

The goal is to provide similar Wi-Fi troubleshooting and reporting capabilities across platforms while taking advantage of the networking APIs available on each operating system.

| Platform            | Project                           | Access                                                                                                             |
| ------------------- | --------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| 🖥️ **PowerShell**  | PS Wi-Fi Analyzer                 | [GitHub](https://github.com/hov172/PS_WI-FI_Analyzer)                                                              |
| 🪟 **Windows**      | WinWiFiAnalyzer                   | [GitHub](https://github.com/hov172/WinWiFiAnalyzer)                                                                |
| 📱 **iOS / iPadOS** | Wi-Fi Analyzer Beta               | [Apple TestFlight](https://testflight.apple.com/join/hDPGsHzd)                                                     |
| 🍎 **macOS**        | Wi-Fi Analyzer — Windows-style UI | [Download DMG](https://github.com/hov172/WinWiFiAnalyzer/releases/download/Windows_Wifi_Report/Wi.Fi.Analyzer.dmg) |
| 🍎 **macOS**        | WiFi Diag Report                  | This Project                                                                                                       |

### 🖥️ PowerShell

**PS_WI-FI_Analyzer** provides Wi-Fi diagnostics and reporting directly through Windows PowerShell.

It is designed for administrators and technicians who want a lightweight script-based diagnostic tool without requiring a full graphical application.

**Repository:**
https://github.com/hov172/PS_WI-FI_Analyzer

### 🪟 Windows

**WinWiFiAnalyzer** provides a graphical Windows application for Wi-Fi diagnostics, network analysis, troubleshooting, and reporting.

**Repository:**
https://github.com/hov172/WinWiFiAnalyzer

### 📱 iOS / iPadOS

The iOS/iPadOS version is currently available for beta testing through Apple TestFlight.

**Join the Beta:**
https://testflight.apple.com/join/hDPGsHzd

Because Apple restricts access to certain low-level Wi-Fi information on iOS/iPadOS, some diagnostics available on Windows and macOS cannot be implemented identically on iPhone or iPad.

### 🍎 macOS — Windows Layout Version

A separate macOS Wi-Fi Analyzer is available that follows the layout and workflow of **WinWiFiAnalyzer**, providing a more consistent interface for users moving between Windows and macOS.

**Download DMG:**
https://github.com/hov172/WinWiFiAnalyzer/releases/download/Windows_Wifi_Report/Wi.Fi.Analyzer.dmg

---

# 🖼️ WiFi Diagnostics Report

<img width="1439" height="808" alt="WiFi Diag Report" src="https://github.com/user-attachments/assets/7fa21c04-c59a-4e64-8538-dda12e0f32d4" />

<img width="1437" height="810" alt="WiFi Diag Report" src="https://github.com/user-attachments/assets/34e9ed06-e46b-4eda-8e77-22bbf4ee7ae5" />

<img width="1440" height="809" alt="WiFi Diag Report" src="https://github.com/user-attachments/assets/ec024941-0983-4207-b595-0769c3a0751c" />

---

# 📊 Example Reports

## IT Administrator — Wi-Fi Coverage Map

An IT team member can survey an area with reported Wi-Fi problems and generate a coverage-map report containing collected measurements and visual coverage information.

[Example WiFi Coverage Map Report](https://github.com/user-attachments/files/21747000/Example.WiFi-Coverage-MapReport.pdf)

## Student / End-User Diagnostic Report

Students or other non-IT users can generate a simplified diagnostic report and send it directly to the Help Desk.

[![Download Example Report](https://img.shields.io/badge/Download-ExampleReportForIT.txt-brightgreen)](https://github.com/hov172/WifDiagReport/raw/main/ExampleReportForIT.txt)

---

# 🆕 What's New

## Version 4.4 Build 1.5 — Multi-AP Mapping

### 📡 Multi-AP Capture & Overlap Mapping

* **Multi-AP Capture** — Every measurement point can perform a background scan and store all visible APs, including:

  * SSID
  * BSSID
  * RSSI
  * Channel
  * Band

* **Heatmap Layers** — Switch between:

  * Connected network
  * Individual access points
  * AP overlap zones

* **Overlap Visualization**

  * 1 usable AP
  * 2 usable APs
  * 3+ usable APs
  * Uses a ≥ −70 dBm usable-signal threshold

* **Band Filtering** — Analyze AP overlap independently for:

  * 2.4 GHz
  * 5 GHz
  * 6 GHz

* **Sticky Point Selection** — Selected survey points remain highlighted across map views.

* **Layer-Aware Reports** — Coverage-map PDF and print reports follow the currently selected heatmap layer.

* **Full-Screen Quick Add** — Add measurement points directly from the full-screen map.

### 🏪 App Store & Sandbox Improvements

* Correct macOS App Sandbox entitlements
* Outgoing network access
* Location support
* User-selected file access
* Correct Info.plist processing
* Improved App Store validation compatibility
* Sandbox-safe scanner CSV exports
* Removed unnecessary ATS arbitrary-load exceptions

### 🛡️ Sandbox-Safe Network Testing

When ICMP testing is unavailable because of App Sandbox restrictions, WiFi Diag Report can fall back to **UDP DNS round-trip measurements**.

Tests clearly identify UDP-based measurements instead of presenting them as ICMP results.

If no valid measurement can be collected, the application reports:

**Test Failed**

rather than generating misleading packet-loss results.

---

# 🚀 Core Features

## 📡 Wi-Fi Scanner

Scan surrounding wireless networks and analyze:

* SSID
* BSSID
* RSSI
* Signal quality
* Channel
* Band
* Security
* Nearby networks
* Channel congestion
* Multi-AP environments
* Potential roaming conditions

Scan information can also be exported for additional analysis.

---

## 📊 Real-Time Wi-Fi Monitoring

Monitor the active Wi-Fi connection continuously.

Metrics include:

* RSSI
* Noise
* SNR
* TX rate
* Signal quality
* MCS Index
* Spatial Streams / NSS
* Channel width
* PHY mode

Measurements update approximately every **1 second**.

Up to **300 measurements / 5 minutes** of recent data can be retained for visualization.

Available views include:

* Last 1 minute
* Last 5 minutes
* All collected data

Monitoring sessions can be exported to CSV.

---

# 🗺️ Advanced Wi-Fi Coverage Mapping

Upload a floor plan and perform an interactive Wi-Fi site survey.

Supported floor-plan formats include:

* PNG
* JPEG
* PDF
* SVG
* TIFF

Measurement points can collect:

* RSSI
* Noise
* SNR
* Channel
* Band
* MCS Index
* Spatial Streams / NSS
* Channel width
* PHY mode
* Timestamp
* Location information
* Visible AP information

### Measurement Modes

Coverage points can be created using:

* Manual coordinates
* Click-to-select
* Live mouse tracking
* Grid Assistant

### Map Controls

Maps support:

* Zoom
* Pan
* Rotation
* Point selection
* Point renaming
* Point details
* AP information
* Measurement deletion
* Saved map state

Saved projects preserve map positioning and measurement information.

---

# 🔥 Signal Heatmaps

WiFi Diag Report can generate interpolated signal heatmaps from collected measurement points.

Heatmaps use measured RSSI information to visualize wireless coverage across a floor plan.

Available visualization layers include:

### Connected Network

Displays signal coverage for the currently connected network.

### Individual AP

Select a specific BSSID/AP and visualize its measured coverage.

### AP Overlap

Visualize areas where multiple usable APs overlap.

Band filtering allows overlap analysis to be restricted to:

* 2.4 GHz
* 5 GHz
* 6 GHz

This prevents multiple radios from the same multi-band deployment from artificially inflating AP overlap counts.

Heatmaps can also be included in exported coverage-map reports.

---

# 🌐 Real Network Performance Testing

WiFi Diag Report performs real network measurements rather than simulated results.

## Download / Upload Testing

HTTP throughput measurements can be performed using multiple concurrent network streams.

## Latency

Latency testing measures network round-trip performance and can report:

* Average latency
* Jitter
* Test method

## Packet Loss

Packet-loss testing evaluates whether expected responses are successfully received.

When sandbox restrictions prevent ICMP measurements, supported tests can use UDP-based network measurements instead.

Failed tests are reported as failures rather than generating fabricated results.

---

# 🧠 IT Analysis Engine

The IT Analysis Engine converts collected technical information into structured diagnostic findings.

It is designed specifically for:

* Help Desk technicians
* Desktop support
* Network administrators
* IT managers
* Higher-education IT environments

## Executive Summary

Provides:

* Overall network health assessment
* High-level findings
* Major problems
* Positive observations
* Risk assessment

## Signal Analysis

Evaluates:

* RSSI
* Signal quality
* SNR
* Signal stability
* Coverage
* Potential roaming readiness

## Performance Analysis

Evaluates:

* Download performance
* Upload performance
* Latency
* Jitter
* Packet loss
* Connection reliability

## Environment Analysis

Evaluates:

* Nearby networks
* Channel congestion
* Wireless interference
* Security
* Band utilization
* Optimization opportunities

## Hardware Analysis

Evaluates:

* Wi-Fi standard
* MCS capability
* Spatial streams
* Channel width
* Device limitations
* Hardware efficiency
* Potential upgrade opportunities

---

# 🚦 IT Recommendations

Diagnostic findings can generate prioritized recommendations.

### 🔴 Critical

Problems requiring immediate attention.

### 🟠 High

Important problems likely to have a significant effect on connectivity or performance.

### 🟡 Medium

Recommended optimizations that may improve reliability or performance.

### 🟢 Low

Optional improvements and best-practice recommendations.

Recommendations can include:

* Technical details
* Measurements
* Explanation
* Troubleshooting actions
* Suggested remediation

Categories include:

* Signal
* Security
* Performance
* Hardware
* Environment
* Configuration

---

# 📶 Advanced Wi-Fi Metrics

## MCS Index

**Modulation and Coding Scheme (MCS)** provides information about the modulation, coding rate, spatial streams, and potential data rate of a Wi-Fi connection.

Supported analysis includes Wi-Fi 4, Wi-Fi 5, and Wi-Fi 6 environments.

## Spatial Streams — NSS

The Number of Spatial Streams helps identify the MIMO capabilities being used by the connection.

More spatial streams can provide greater potential throughput when supported by both the client and access point.

## Channel Width

WiFi Diag Report can identify common channel widths including:

* 20 MHz
* 40 MHz
* 80 MHz
* 160 MHz

## PHY Mode

The application can identify supported/current Wi-Fi PHY information including:

* 802.11n / Wi-Fi 4
* 802.11ac / Wi-Fi 5
* 802.11ax / Wi-Fi 6

---

# 📄 Professional Reporting

WiFi Diag Report can export diagnostic information in multiple formats for different audiences.

Reports can include:

* Device information
* Network configuration
* Wi-Fi connection information
* Signal measurements
* Nearby network scans
* Speed-test results
* Latency
* Packet loss
* Advanced Wi-Fi metrics
* Coverage-map measurements
* Heatmaps
* IT Analysis findings
* Recommendations

### Report Types

**End-User / Student Report**

Designed to provide Help Desk technicians with the information needed to begin troubleshooting.

**IT Technical Report**

Provides detailed measurements and technical findings.

**Executive Summary**

Provides higher-level network-health information and major findings.

**Coverage Map Report**

Combines floor plans, survey points, signal information, statistics, and optional heatmaps.

---

# 🛠️ Run All Diagnostics

The automated diagnostic workflow can run multiple tests and collect information in a single operation.

The interface provides:

* Confirmation before starting
* Full-screen progress display
* Concurrent network testing
* Real-time progress
* Result summaries
* Export options after completion

---

# 🎛️ Deployment Customization

WiFi Diag Report can be customized for different types of users without creating separate builds.

The application reads:

`WifiDialogReport/Configuration.plist`

Feature visibility is controlled using `HideXXXX` configuration keys.

For example:

```xml
<key>HideAdvancedTools</key>
<true/>
```

A value of:

```xml
<true/>
```

hides the associated feature.

A value of:

```xml
<false/>
```

makes the feature available.

This allows organizations to create different experiences for:

* Students
* Faculty
* Staff
* Help Desk technicians
* Network administrators
* IT administrators

while maintaining the same application.

---

# ⚡ Quick Start

## Requirements

* macOS 13 Ventura or newer
* Wi-Fi enabled
* Location permission for Wi-Fi scanning
* Network access for performance testing
* Additional permissions where required by macOS

## Basic Workflow

1. Launch WiFi Diag Report.
2. Review the Dashboard.
3. Verify device and network information.
4. Scan surrounding Wi-Fi networks.
5. Start real-time signal monitoring.
6. Run network performance tests.
7. Run the automated diagnostic workflow.
8. Review IT Analysis findings.
9. Generate a diagnostic report.

---

# 🗺️ Coverage Survey Workflow

1. Open **Coverage Mapping**.
2. Import a floor plan.
3. Select a measurement method.
4. Move to the first physical survey location.
5. Add a measurement point.
6. Allow WiFi Diag Report to collect Wi-Fi/AP information.
7. Continue through the survey area.
8. Enable the signal heatmap.
9. Select the desired AP or overlap layer.
10. Review coverage and overlap.
11. Generate the coverage-map report.

---

# 🧰 Troubleshooting

## Wi-Fi Permissions

If Wi-Fi scanning does not work:

* Verify Wi-Fi is enabled.
* Verify Location Services are enabled.
* Grant requested permissions.
* Restart the application after changing permissions if necessary.

## Network Scanning

If surrounding networks are not detected:

* Verify Wi-Fi is active.
* Refresh the scan.
* Check macOS privacy permissions.
* Check for VPN or security restrictions.

## Coverage Mapping

If a floor plan cannot be loaded:

* Verify the file format.
* Check file permissions.
* Verify sufficient available disk space.

## Export Problems

If an export fails:

* Verify the destination is writable.
* Check available disk space.
* Select another destination.
* Try another supported export format.

## Network Tests

Some network tests may behave differently when the application is running inside the macOS App Sandbox.

When ICMP access is unavailable, supported diagnostics can automatically use an alternate UDP-based measurement.

The application identifies the measurement method in the results.

---

# 🏗️ Technical Details

WiFi Diag Report is built using native macOS technologies including:

* Swift
* SwiftUI
* CoreWLAN
* Apple networking frameworks
* Swift Charts
* macOS system information interfaces

The application uses background processing where appropriate to avoid blocking the user interface during network collection and diagnostic operations.

---

# 👨‍💻 Development

## Requirements

* macOS 13+
* Xcode
* Swift / SwiftUI development environment

## Setup

1. Clone the repository.
2. Open `Wifi Diagnostics Report.xcodeproj` in Xcode.
3. Configure signing if required.
4. Build and run.

---

# 🤝 Contributing

Contributions are welcome.

Areas of interest include:

* Wi-Fi analysis
* Coverage mapping
* Network diagnostics
* Additional reporting formats
* Performance improvements
* UI/UX improvements
* Accessibility
* Help Desk integration
* Cross-platform feature parity

Bug reports, feature requests, documentation improvements, and code contributions are welcome through GitHub.

---

# 🌐 Connect With Me

* [GitHub](https://github.com/hov172)
* [PowerShell Gallery](https://www.powershellgallery.com/profiles/hov172)
* 📨 Slack: **@Hov172**
* 🕹️ Discord: **Jay172_**
* [LinkedIn](https://www.linkedin.com/in/jesus-a-785bb616?trk=people-guest_people_search-card)
* [Twitter / X — @AyalaSolutions](https://twitter.com/AyalaSolutions)
* [Bluesky — @AyalaSolutions](https://bsky.app/profile/ayalasolutions.bsky.social)
* [Buy Me a Coffee](https://buymeacoffee.com/hov172)

For questions, issues, and feature requests, please use the project's GitHub Issues or Discussions.

---

# ⭐ Support the Project

If you find these tools useful, consider giving the repositories a ⭐ on GitHub.

It helps support continued development of the **PowerShell, Windows, macOS, and iOS/iPadOS Wi-Fi diagnostic tools**.
