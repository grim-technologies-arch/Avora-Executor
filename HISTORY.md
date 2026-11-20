# Avora — Development History & File Provenance Log

**Project:** Avora (`Avora` C++ Execution Core & `AvoraUI` Desktop Application)  
**Copyright:** © 2026 Avora. All rights reserved.  
**Generated:** 2026-11-20 18:39:30 (+08:00)  
**Workspace Root:** `d:\Avora Invite only`

---

## 1. Chronological Development Timeline

### Phase 0 — Avora C++ Core & Runtime (`2026-09-13` – `2026-11-19`)
| Date / Time | Milestone | Key Artifacts |
|---|---|---|
| `2026-09-13 09:10` | Initial Visual Studio user project setup | `Avora\Nam.vcxproj.user` |
| `2026-09-19 14:59` | Core headers (`globals.h`, `roblox.h`) | `Avora\globals.h`, `Avora\roblox.h` |
| `2026-10-06 23:47` | Project configuration update | `Avora\Avora.vcxproj.user` |
| `2026-11-14 13:15` – `17:22` | Execution scheduler, HTTP GC/resume fixes, crash handler, Myriad API/callback/GC, and C-closure regression testing | `Avora\.maintenance\build-*.log`, `crash-fix-report.md`, `execution-fix-report.md`, `cclosure-regression-*.log` |
| `2026-11-17` – `2026-11-18` | Integration logs (`ghp.log`, `hoho.log`) | `Avora\.maintenance\ghp.log`, `Avora\.maintenance\hoho.log` |
| `2026-11-19 21:01` – `21:23` | Solution consolidation, `CrashHandler.hpp`, and `entry.cpp` updates | `Avora\Avora.sln`, `Avora\Avora.vcxproj`, `Avora\CrashHandler.hpp`, `Avora\entry.cpp` |

### Phase 1 — AvoraUI Foundation, Auth & Packaging (`2026-11-20 11:21` – `11:51`)
| Time (`2026-11-20`) | Milestone | Key Files |
|---|---|---|
| `11:21:14` – `11:21:43` | Electron 45 app shell, sandboxed preload, invite-only auth client, login/register UI, branding assets (`logo.png`, `icon.ico`) | `AvoraUI\package.json`, `electron\main.cjs`, `electron\preload.cjs`, `electron\auth.cjs`, `src\index.html`, `src\styles.css`, `src\app.js`, `tests\auth.test.cjs` |
| `11:22:15` – `11:25:16` | Automated UI, native IPC, and packaged `.exe` verification harnesses + first portable build | `scripts\verify-ui.cjs`, `scripts\verify-native.cjs`, `scripts\verify-packaged.cjs`, `release\Avora-1.0.0-Windows.exe` |
| `11:37:08` – `11:37:55` | Text-selection repaint stability fix & verification | `scripts\verify-selection.cjs`, `artifacts\selection-before.png`, `artifacts\selection-fixed.png` |
| `11:49:08` – `11:51:53` | Demo session persistence (`session-store.cjs`) and Dashboard / Home workspace (`dashboard.js`, `dashboard.css`, activity heatmap, updates, featured cards) | `electron\session-store.cjs`, `src\dashboard.js`, `src\dashboard.css`, `tests\session-store.test.cjs`, `scripts\verify-demo.cjs` |

### Phase 2 — Editor Workspace & Script Hub (`2026-11-20 15:00` – `15:41`)
| Time (`2026-11-20`) | Milestone | Key Files |
|---|---|---|
| `15:00:15` – `15:06:18` | Editor workspace, file tree, tabs, console pane, native open/save dialogs (`editor-files.cjs`), and editor verification | `src\editor.css`, `src\editor\workspace.js`, `electron\editor-files.cjs`, `src\vendor\editor.js`, `scripts\verify-editor.cjs`, `tests\editor-files.test.cjs` |
| `15:30:34` – `15:36:15` | Custom accessible animated select menus (`select.js`/`select.css`), Script Hub 2-column grid, 6 game thumbnails, filters, favorites/recent | `src\ui\select.js`, `src\ui\select.css`, `src\script-hub.js`, `src\script-hub.css`, `src\assets\hub\*.png`, `scripts\verify-hub.cjs` |
| `15:41:05` | Sleek custom scrollbars | `src\ui\scrollbars.css` |

### Phase 3 — Acrylic Glass & 120 FPS Backdrop Engine (`2026-11-20 15:50` – `17:12`)
| Time (`2026-11-20`) | Milestone | Key Files |
|---|---|---|
| `15:50:50` – `16:04:37` | Acrylic glass CSS/JS layer and DWM blur integration | `src\ui\glass.css`, `src\ui\glass.js`, `electron\desktop-blur.cjs`, `scripts\preview-glass.cjs` |
| `16:52:09` – `17:12:49` | Live Z-order behind-window Win32 capture, 120 FPS `worker_threads` geometry tracker (`backdrop-worker.cjs`), and O(1) separable Gaussian blur on `#desktop-backdrop` | `electron\backdrop-worker.cjs`, `electron\desktop-blur.cjs`, `electron\main.cjs`, `src\ui\glass.js`, `src\ui\glass.css` |

### Phase 4 — Polish, ScriptBlox Live Feed, Xmind Font & Monaco Luau (`2026-11-20 17:38` – `18:36`)
| Time (`2026-11-20`) | Milestone | Key Files |
|---|---|---|
| `17:38` – `17:46` | Script Hub & Workspace tree sliding pill animations, footer removal, square Play button, frosted acrylic dropdowns, filled verified badge, spaced floating scrollbars, square heatmap cells | `src\script-hub.css`, `src\editor.css`, `src\dashboard.css`, `src\ui\scrollbars.css`, `src\ui\glass.css` |
| `17:47` – `18:20` | Live ScriptBlox API (`electron\scriptblox.cjs`) for Home Featured Scripts, paginated endless Script Hub, and live search; zero-flash startup pre-warm; console collapse animation & filter spacing; icon-only bell + centered profile modal; bundled Google Fonts `Xmind` | `electron\scriptblox.cjs`, `src\assets\fonts\xmind-*.woff2`, `src\styles.css`, `src\dashboard.js`, `src\script-hub.js` |
| `18:25` – `18:36` | Upgraded to **Monaco Editor** with smooth caret/scroll animations, transparent glass theme, and Luau/Roblox/UNC autofill (`luau-monaco.js`); inline double-click file rename with locked extensions; final unpacked & portable builds | `src\editor\luau-monaco.js`, `src\editor\workspace.js`, `src\vendor\editor.worker.js`, `src\vendor\editor.css`, `release\win-unpacked\Avora.exe`, `release\Avora-1.0.0-Windows.exe` |

---

## 2. AvoraUI File Creation & Modification Inventory

| File | Created | Last Modified | Size (bytes) |
|---|---|---|---|
| `AvoraUI\package.json` | `2026-11-20 11:21:14` | `2026-11-20 18:29:11` | 2,525 |
| `AvoraUI\.gitignore` | `2026-11-20 11:21:14` | `2026-11-20 11:21:14` | 40 |
| `AvoraUI\avora.config.json` | `2026-11-20 11:21:14` | `2026-11-20 11:21:14` | 53 |
| `AvoraUI\README.md` | `2026-11-20 11:21:14` | `2026-11-20 15:55:27` | 5,114 |
| `AvoraUI\electron\auth.cjs` | `2026-11-20 11:21:14` | `2026-11-20 11:49:08` | 5,320 |
| `AvoraUI\electron\main.cjs` | `2026-11-20 11:21:14` | `2026-11-20 18:19:08` | 7,902 |
| `AvoraUI\electron\preload.cjs` | `2026-11-20 11:21:14` | `2026-11-20 18:16:41` | 1,281 |
| `AvoraUI\electron\session-store.cjs` | `2026-11-20 11:49:08` | `2026-11-20 11:49:08` | 815 |
| `AvoraUI\electron\editor-files.cjs` | `2026-11-20 15:02:49` | `2026-11-20 15:02:49` | 3,363 |
| `AvoraUI\electron\desktop-blur.cjs` | `2026-11-20 16:04:37` | `2026-11-20 17:12:49` | 4,420 |
| `AvoraUI\electron\backdrop-worker.cjs` | `2026-11-20 17:05:07` | `2026-11-20 17:07:24` | 11,519 |
| `AvoraUI\electron\scriptblox.cjs` | `2026-11-20 17:47:14` | `2026-11-20 18:19:08` | 6,280 |
| `AvoraUI\src\index.html` | `2026-11-20 11:21:14` | `2026-11-20 18:29:12` | 30,118 |
| `AvoraUI\src\styles.css` | `2026-11-20 11:21:14` | `2026-11-20 18:11:03` | 8,181 |
| `AvoraUI\src\app.js` | `2026-11-20 11:21:14` | `2026-11-20 11:51:12` | 6,163 |
| `AvoraUI\src\dashboard.css` | `2026-11-20 11:51:12` | `2026-11-20 18:10:47` | 17,415 |
| `AvoraUI\src\dashboard.js` | `2026-11-20 11:51:12` | `2026-11-20 18:19:08` | 11,717 |
| `AvoraUI\src\editor.css` | `2026-11-20 15:00:15` | `2026-11-20 18:34:02` | 12,358 |
| `AvoraUI\src\editor\workspace.js` | `2026-11-20 15:01:55` | `2026-11-20 18:36:28` | 21,466 |
| `AvoraUI\src\editor\luau-monaco.js` | `2026-11-20 18:25:11` | `2026-11-20 18:25:11` | 17,410 |
| `AvoraUI\src\script-hub.js` | `2026-11-20 15:34:09` | `2026-11-20 18:19:08` | 14,763 |
| `AvoraUI\src\script-hub.css` | `2026-11-20 15:34:09` | `2026-11-20 18:10:47` | 10,175 |
| `AvoraUI\src\ui\select.js` | `2026-11-20 15:30:34` | `2026-11-20 15:41:05` | 7,374 |
| `AvoraUI\src\ui\select.css` | `2026-11-20 15:30:34` | `2026-11-20 18:19:08` | 2,618 |
| `AvoraUI\src\ui\scrollbars.css` | `2026-11-20 15:41:05` | `2026-11-20 17:55:12` | 924 |
| `AvoraUI\src\ui\glass.css` | `2026-11-20 15:50:50` | `2026-11-20 18:10:47` | 7,733 |
| `AvoraUI\src\ui\glass.js` | `2026-11-20 15:50:50` | `2026-11-20 17:12:49` | 5,269 |
| `AvoraUI\src\assets\logo.png` | `2026-11-20 11:21:28` | `2026-11-20 11:21:28` | 90,670 |
| `AvoraUI\build\icon.ico` | `2026-11-20 11:21:28` | `2026-11-20 11:21:28` | 47,610 |
| `AvoraUI\src\assets\fonts\xmind-latin.woff2` | `2026-11-20 18:10:07` | `2026-11-20 18:10:08` | 27,196 |
| `AvoraUI\src\assets\fonts\xmind-latin-ext.woff2` | `2026-11-20 18:10:08` | `2026-11-20 18:10:08` | 15,600 |
| `AvoraUI\src\vendor\editor.js` | `2026-11-20 15:02:50` | `2026-11-20 18:34:17` | 4,621,882 |
| `AvoraUI\src\vendor\editor.css` | `2026-11-20 18:25:36` | `2026-11-20 18:34:17` | 379,672 |
| `AvoraUI\src\vendor\editor.worker.js` | `2026-11-20 18:25:36` | `2026-11-20 18:25:36` | 307,264 |
| `AvoraUI\tests\auth.test.cjs` | `2026-11-20 11:21:14` | `2026-11-20 11:51:51` | 4,722 |
| `AvoraUI\tests\session-store.test.cjs` | `2026-11-20 11:51:51` | `2026-11-20 11:51:51` | 1,154 |
| `AvoraUI\tests\editor-files.test.cjs` | `2026-11-20 15:06:18` | `2026-11-20 15:06:18` | 2,560 |
| `AvoraUI\scripts\verify-ui.cjs` | `2026-11-20 11:22:15` | `2026-11-20 11:37:33` | 4,751 |
| `AvoraUI\scripts\verify-native.cjs` | `2026-11-20 11:24:39` | `2026-11-20 11:30:47` | 1,074 |
| `AvoraUI\scripts\verify-packaged.cjs` | `2026-11-20 11:25:16` | `2026-11-20 11:31:02` | 2,295 |
| `AvoraUI\scripts\verify-selection.cjs` | `2026-11-20 11:37:08` | `2026-11-20 16:56:27` | 2,920 |
| `AvoraUI\scripts\verify-demo.cjs` | `2026-11-20 11:51:51` | `2026-11-20 14:51:29` | 7,732 |
| `AvoraUI\scripts\verify-editor.cjs` | `2026-11-20 15:03:51` | `2026-11-20 18:29:11` | 8,316 |
| `AvoraUI\scripts\verify-hub.cjs` | `2026-11-20 15:35:45` | `2026-11-20 15:41:05` | 8,616 |
| `AvoraUI\scripts\preview-glass.cjs` | `2026-11-20 15:50:50` | `2026-11-20 17:12:49` | 4,485 |
| `AvoraUI\release\win-unpacked\Avora.exe` | `2026-11-20 18:34:29` | `2026-11-20 18:34:32` | 249,989,120 |
| `AvoraUI\release\Avora-1.0.0-Windows.exe` | `2026-11-20 11:24:37` | `2026-11-20 18:36:51` | 112,197,542 |
