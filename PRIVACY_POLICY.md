# Privacy Policy for Instant Photo Viewer

**Last Updated:** November 2026

**Instant Photo Viewer** ("the Application") is developed by **MrKalita**. Your privacy and data sovereignty are fundamental principles of our software design. This Privacy Policy outlines our strict offline data handling practices.

---

### 1. 100% Offline Execution & Zero Data Collection
Instant Photo Viewer is an entirely local, offline native Windows desktop application:
- **No Analytics or Telemetry**: Instant Photo Viewer contains zero analytics SDKs, zero telemetry probes, zero tracking pixels, and zero background reporting services.
- **No Personal Information**: We do not collect, process, transmit, store, or monetize personal names, email addresses, IP addresses, location data, or device identifiers.
- **No Network Activity**: The Application contains zero networking libraries and makes zero outbound internet connections. It operates completely disconnected from the internet.

### 2. Local Image & File Processing
- **Explicit User Control**: The Application only accesses files that you explicitly choose to open (or neighboring image files within the same directory for gallery and slideshow navigation).
- **In-Memory Decoding**: All image processing, EXIF metadata extraction, color space conversion, and Direct3D 11 hardware rendering occur strictly within your system's local RAM and GPU video memory.
- **No Cloud Synchronization**: Your photos, images, EXIF metadata, and file paths never leave your device under any circumstances.

### 3. Local Preferences & Configuration
- Any user preferences (such as window state, slideshow interval, zoom behavior, and resident process toggles) are stored strictly on your local computer in `%LOCALAPPDATA%\InstantPhotoViewer\settings.json`.
- This data remains exclusively on your machine and is never shared, transmitted, or backed up to remote servers.

### 4. Windows Startup Task Transparency
- If enabled by the user, Instant Photo Viewer registers a standard Windows Startup Task (`windows.startupTask`) to keep a lightweight resident process in the system tray for sub-50ms instant warm launching.
- This background process runs 100% locally with zero network activity and consumes minimal idle memory (~1 MB).
- You can enable or disable this feature at any time through the in-app Settings dialog (`Ctrl+,`), system tray menu, Windows Settings (`Apps > Startup`), or Windows Task Manager.

### 5. Safe Operations
- File deletions performed within the app (`Delete` key) use the official Windows Shell `IFileOperation` API to send files to the Windows Recycle Bin, allowing full user recovery.

### 6. Contact & Support
For any questions or feedback regarding this Privacy Policy, please open an issue on the project's GitHub repository or reach out via the Microsoft Store:
- **GitHub**: https://github.com/Mrkalitaa/InstantPhotoViewer
- **Microsoft Store**: https://apps.microsoft.com/detail/9NV5167C5GGS
