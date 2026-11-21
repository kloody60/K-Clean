# K-Clean

أداة تنظيف وتحليل للويندوز، بواجهة داكنة حديثة (عربي وإنجليزي).
**A modern Windows cleaner, disk analyzer and RAM optimizer** (Arabic / English UI, dark / light / system theme).

## Download / التحميل

Go to the **[Releases](../../releases/latest)** page and download `K-Clean-Setup.exe`.
Verify the file with the SHA-256 listed in the release notes if you want.

## Features / المميزات

**Cleaning / التنظيف**
- Basic cleaning (temp files, Windows Update cache, thumbnails, browser caches, GPU shader cache, crash reports, Recycle Bin, Steam cache on all drives).
- Deep cleaning (full Disk Cleanup, DISM component cleanup, Windows logs, Delivery Optimization, leftovers on every drive, RAM).
- Advanced options with a confirmation prompt (Event Logs, restore points, developer caches).
- Scan-only mode, and a Stop button while cleaning.

**Disk analyzer / تحليل المساحة**
- Fast scan of any drive or folder (about 7 seconds for a 300 GB system drive).
- Folder tree sorted by size with % bars, allocated size, file counts, last modified.
- Right-click menu: open, show in Explorer, copy path/name, copy, cut, rename, new folder, refresh, properties, the full Windows menu, delete (Recycle Bin or permanent).
- Search, largest 300 files, hide empty folders, export to CSV.

**Memory / الذاكرة**
- Live RAM gauge with details (in use, available, cached, standby, modified, free).
- One-click optimize: free working sets, clear standby list, defrag RAM.
- Auto optimize (low memory / every N minutes / only when CPU is idle), tray icon with live usage, hotkey, run at startup.

## Notes / ملاحظات

- Needs **administrator** permission (to clean system folders and optimize memory).
- The installer is **not code-signed**, so Windows SmartScreen may show a warning: choose *More info → Run anyway*.
- Default install path: `C:\Program Files (x86)\K-Clean`. You can change it in the installer.
- Uninstall from *Settings → Apps*.
- Cleaning deletes files. Review the selected options before you press *Start cleaning*; the "advanced" ones cannot be undone.

## Silent install

```
K-Clean-Setup.exe /S "/D=C:\Program Files (x86)\K-Clean" /LANG=en
K-Clean-Setup.exe /uninstall /S
```
