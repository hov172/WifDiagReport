# File Reference Guide: Wifi Diagnostics Report App

> **Platform Note:**  
> This project is **macOS ONLY**. Any iOS/`UIKit` files or references are obsolete—do not add, reference, or support iOS/Universal targets. The current codebase is built for macOS 13+ with SwiftUI.

This document serves as a lookup reference for developers and contributors, providing a high-level overview of which file is responsible for which part of the app. Use this to quickly determine where to make changes for new features, UI tweaks, bug fixes, or support tasks.

**Project Status:** Cleaned up July 2025 - Reduced from 70+ files to 31 essential Swift files

---

## Main Entry & Navigation

- **DeviceInfoUniversalAppApp.swift**  
  Main app lifecycle entry; sets up root views and environment objects.

- **ContentView.swift**  
  Split navigation UI; main hub for sidebar and all primary screen switching.  
  **Contains Modern UI Components:**  
  - `ModernSidebarView` - Enhanced sidebar with modern styling and animations
  - `ModernNavigationItem` - Individual navigation items with hover/selection states
  - `ModernSectionHeader` - Styled section headers with custom typography
  - `EnhancedActionButton` - Primary/secondary action buttons with press animations
  - `EnhancedWelcomeView` - Animated welcome screen with feature highlights
  - `EnhancedFeatureCard` - Individual feature cards with hover effects
  - `NavigationSelection` enum - Navigation state management
  - `runAllDiagnosticsAndPromptExport()` - Comprehensive diagnostics orchestration
  **Imports:** All main view controllers and manages app-wide navigation state.
  **Wiring new main features always starts here!**

- **SidebarConfig.swift**  
  Controls visibility/enablement of items in the sidebar, based on configuration.  
  **Used by:** `ContentView.swift` (determines if menu items are shown/hidden)

---

## Device & Network Info Screens

- **Views/DeviceInfoDetailView.swift**  
  Shows summary and advanced details about the device hardware/OS.  
  **Imports:** `DeviceInfoManager.swift`, `SharedComponents.swift`  
  **Linked from:** `ContentView.swift` (case `.deviceInfo` in sidebar switch)

- **Views/NetworkInfoDetailView.swift**  
  Shows network status (IP, WiFi, DNS, signal, etc).  
  **Imports:** `DeviceInfoManager.swift`, `SharedComponents.swift`  
  **Linked from:** `ContentView.swift` (case `.networkInfo`)

---

## WiFi Analysis

- **WiFiScannerManager.swift**  
  Logic for scanning all available WiFi networks; provides model for scan results and security checks.  
  **Used by:** `WiFiScannerView.swift`, `DeviceInfoManager.swift` (for wifi scan functionality)

- **WiFiScannerView.swift**  
  User interface for viewing scan results, scanning, and exporting as CSV.  
  **Imports:** `WiFiScannerManager.swift`, `NetworkDetailView.swift`, `DeviceInfoManager.swift`  
  **Linked from:** `ContentView.swift` (case `.wifiScanner`)

- **NetworkDetailView.swift**  
  Modal that shows all technical info for a specific WiFi network in the list.  
  **Imports:** `WiFiScannerManager.swift`, `Charts`  
  **Presented from:** `WiFiScannerView.swift`

---

## Speed, Latency, and Packet Loss Testing

- **Views/SpeedTestView.swift**  
  UI for running and showing speed/latency/packet loss tests.  
  **Imports:** `DeviceInfoManager.swift`, `Views/SpeedMeterView.swift`, `Views/NetworkMetricRow.swift`
  **Linked from:** `ContentView.swift` (case `.speedTest`)

- **Views/SpeedMeterView.swift**  
  Visual circular meter for speed test. Used in `SpeedTestView`.

- **Views/NetworkMetricRow.swift**  
  Row for displaying and running individual latency/packet loss tests.

---

## WiFi Coverage Mapping

### Main Coverage Map View
- **CoverageMapView.swift**  
  Main coverage mapping interface; lets user upload a floorplan, plot signal readings, visualize WiFi coverage, and export results.  
  **Imports:** `DeviceInfoManager.swift`, `CoverageMapViewComponents/*`  
  **Linked from:** `ContentView.swift` (case `.coverageMap`)

### Coverage Map Supporting Components
- **CoverageMapViewComponents/CoverageMapViewSupportingViews.swift**  
  Collection of reusable UI components for the coverage mapping feature:
  - `StatCard` - Statistics display cards with icons and colors
  - `PlaceholderView` - Empty state view when no floor map is loaded
  - `TextFieldView` - Custom styled text input fields
  - `InstructionStepView` - Numbered instruction steps
  - `MeasurementPointCardView` - Individual measurement point display cards
  - `RecommendationsView` - Full-screen coverage mapping guide modal
  - `RecommendationSection` - Organized sections within recommendations
  **Used by:** `CoverageMapView.swift`

- **CoverageMapViewComponents/CoveragePointView.swift**  
  Individual coverage point visualization and interaction component.

- **CoverageMapViewComponents/FloorPlanPicker.swift**  
  File picker and floor plan upload interface.

- **CoverageMapViewComponents/FullScreenMapView.swift**  
  Full-screen coverage map display with advanced interactions.

- **CoverageMapViewComponents/GridOverlay.swift**  
  Grid overlay system for systematic measurement point placement.

### Coverage Map Data Models
- **Models/CoordinateTrackingMode.swift**  
  Enum defining coordinate input methods: `manual`, `click`, `realtime`, `grid`.  
  **Used by:** Coverage mapping components for user interaction modes.

- **Models/CoverageMapData.swift**  
  Codable struct for saving/loading complete coverage map state.  
  **Features:** NSImage to Data conversion, point collection, map size preservation.  
  **Used by:** Coverage mapping for data persistence.

---

## Network Test History

- **Views/NetworkHistoryView.swift**  
  Shows a historical log of tests/results, with stats recorded for each test run.  
  **Imports:** `DeviceInfoManager.swift`  
  **Linked from:** `ContentView.swift` (case `.networkHistory`)  
  **Behavior:** *Every time a speed, latency, or packet loss test finishes, its result (with timestamp, SSID, download/upload speeds, and latency) is automatically added to the in-memory history, visible in this view.*

---

## Export & Reports

- **ExportView.swift**  
  UI for exporting all diagnostics/tests to a text file (with optional user info).  
  **Imports:** `DeviceInfoManager.swift`, `AppKit`, `UniformTypeIdentifiers`  
  **Linked from:** `ContentView.swift` (case `.exportInfo`)

---

## Help & Documentation

- **HelpView.swift**  
  Built-in help, guides, explanations for all features & workflows.  
  **Linked from:** `ContentView.swift` (case `.help`)

---

## Visualization & Analysis

- **WiFiVisualization.swift**  
  Provides reusable graphs, channel analysis, legends for WiFi metrics.  
  **Imports:** `DeviceInfoManager.swift`, `WiFiScannerManager.swift`
  **Used in:** Analysis/coverage or advanced screens

- **WiFiTriangulationManager.swift**  
  Advanced WiFi positioning and triangulation logic.  
  **Used by:** Coverage mapping and location-based analysis features.

---

## Shared, Utility, & Styling

- **SharedComponents.swift**  
  Common views (e.g. `InfoRow`) and color/style extensions for card/layout.  
  **Imported by:** Almost all SwiftUI screens and rows.

- **CustomUIComponents.swift**  
  Additional custom UI components and view modifiers.  
  **Contains:** Specialized components for advanced UI interactions.

- **CoordinateTrackingComponents.swift**  
  Components related to coordinate tracking and user input handling.  
  **Used by:** Coverage mapping and location-based features.

---

## Model & Logic Backbone

- **DeviceInfoManager.swift**  
  Core ObservableObject for device/network info, test orchestration, results tracking, data exporting.  
  **Injected as**: `@EnvironmentObject` at top app level (see `DeviceInfoUniversalAppApp.swift`).  
  **Accessed via**: `@EnvironmentObject` or `@ObservedObject` in almost all main screens and detail pages.  
  **Network test results in `networkHistory` are automatically updated after every speed, latency, or packet loss test completes.**

- **LocationManager.swift**  
  Handles device location services and GPS-related functionality.  
  **Used by:** Coverage mapping and location-aware features.

---

## Project Configuration & Settings

- **Configuration.plist**  
  App configuration settings and feature toggles.  
  **Used by:** Various components for runtime configuration.

- **WifiDialogReport.entitlements**  
  macOS app entitlements and permissions.  
  **Required for:** Network access, file system access, and other system features.

- **Info.plist**  
  Standard iOS/macOS app information property list.  
  **Contains:** App metadata, version info, and system requirements.

---

## Legacy & Backup Files

- **Files like `Untitled.swift`, `UIDevice+ModelName.swift`**  
  Legacy iOS-specific or unused files. Safe to delete unless referenced in import statements.

---

## Folder & File Organization Policy

- **`/Views/`** - User-facing screens and major view components
- **`/CoverageMapViewComponents/`** - Supporting components for coverage mapping feature
- **`/Models/`** - Data models and enums
- **Root level** - Managers, shared utilities, main views, and app lifecycle files
- **Remove/ignore any `.swift` files containing iOS/`UIKit` code** or legacy stubs not referenced in navigation or imports.

---

## Previews and Test Views

- Files with `#if DEBUG ..._Previews` are for Xcode previews and safe to edit. Does not affect production.

---

## State & Data Flow

- Uses `@EnvironmentObject` for "global" shared state (e.g. `DeviceInfoManager`, `SidebarConfig`).
- All primary screens access these models automatically as environment objects.  
- When adding a new shared state, inject it in `DeviceInfoUniversalAppApp.swift` and access it with `@EnvironmentObject` in your views.

---

## Comprehensive Quick Reference Chart

| Feature/Screen                   | Main File(s) to Edit                                           | Supporting Components | Linked/Used In                | Appears In Sidebar         |
|----------------------------------|---------------------------------------------------------------|----------------------|-------------------------------|----------------------------|
| Device Info (Overview)           | Views/DeviceInfoDetailView.swift                              | SharedComponents.swift | ContentView.swift             | Yes                        |
| Network Status                   | Views/NetworkInfoDetailView.swift                             | SharedComponents.swift | ContentView.swift             | Yes (toggleable via config)|
| WiFi Scanning & List             | WiFiScannerManager.swift, WiFiScannerView.swift                | WiFiVisualization.swift | ContentView.swift             | Yes                        |
| Specific Network Details         | NetworkDetailView.swift                                       | Charts framework | WiFiScannerView.swift (modal) | No (modal only)            |
| Speed/Latency/Packet Test        | Views/SpeedTestView.swift, Views/SpeedMeterView.swift, Views/NetworkMetricRow.swift | DeviceInfoManager.swift | ContentView.swift | Yes |
| WiFi Coverage Mapping            | CoverageMapView.swift                                         | CoverageMapViewComponents/*, Models/* | ContentView.swift             | Yes                        |
| Coverage Map Components          | CoverageMapViewComponents/CoverageMapViewSupportingViews.swift | StatCard, PlaceholderView, etc. | CoverageMapView.swift | N/A (internal components) |
| Coverage Map Data Models         | Models/CoordinateTrackingMode.swift, Models/CoverageMapData.swift | Foundation | Coverage mapping components | N/A (data layer) |
| Test History (Past Results)      | Views/NetworkHistoryView.swift                                      | DeviceInfoManager.swift | ContentView.swift             | Yes (auto-records each test run) |
| Export Results                   | ExportView.swift                                              | AppKit, UniformTypeIdentifiers | ContentView.swift             | Yes                        |
| Help & Documentation             | HelpView.swift                                                | N/A | ContentView.swift             | Yes                        |
| Visualization/Charts             | WiFiVisualization.swift                                       | Charts framework | Advanced/coverage screens     | No (shared logic/UI)       |
| Coordinate Tracking              | CoordinateTrackingComponents.swift                            | Models/CoordinateTrackingMode.swift | Coverage mapping | No (utility layer) |
| Styling/Reusable Components      | SharedComponents.swift, CustomUIComponents.swift                                        | SwiftUI extensions | Almost everywhere             | N/A                        |
| Data Models & Logic              | DeviceInfoManager.swift, WiFiScannerManager.swift, LocationManager.swift              | Foundation, Core Location | Everywhere (`@EnvironmentObject`, `@ObservedObject`)  | N/A                        |

---

## How to Add a Sidebar Feature — Step By Step

**Checklist for a new user-visible page:**

1. **Create a new file in `/Views/` (e.g. `Views/MyFeatureView.swift`).**
2. **Add a case to** the `NavigationSelection` enum in `ContentView.swift`:
```swift
enum NavigationSelection {
    // Add your new feature here
    case myFeature
}