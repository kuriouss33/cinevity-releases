# CineVity — Újdonságok / What's New

[🇭🇺 Magyar](#-magyar) | [🇬🇧 English](#-english)

---

## 🇭🇺 Magyar

Ez a dokumentum összefoglalja a **CineVity** egyes kiadásainak új funkcióit és fejlesztéseit.

### v1.5.0 (2026-11-27)
- **Beépített AI felskálázás alapból (Out-of-the-Box):** A telepítő immár gyárilag tartalmazza a teljes VapourSynth R73, a beágyazott Python 3.12, a VSORT DirectML motor és a `2xNomosUni_compact_otf_medium.onnx` modell futtatókörnyezetét — külön letöltés nélkül, azonnal használható bármely Windows PC-n.
- **Újrafordított CineVity Médiaszerver & javított TV/Web kliens:** Javítva az asztali Firefox/Brave böngészők 4K/HDR/HEVC végtelen töltési hibája nagy felbontású monitorokon (`is4KDisplay` és Samsung TV mód szétválasztásával), valamint pontosabb natív HLS hibakezelés, visszalépési lánc és autoplay kezelés.
- **Frissített beépített TV alkalmazások & csomagolt eszközök:** Naprakész `CineVity-AndroidTV.apk` (+ ADB), `CineVity.wgt` (+ SDB), frissített `mediaserver.exe`, `ffmpeg.exe`/`ffprobe.exe` és `libmpv-2.dll` egyetlen telepítőben.
- **Teljes körű biztonsági, stabilitási, memóriaszivárgás- és teljesítményjavítások:** Átfogó kódbázis-audit és megerősítés az asztali lejátszóban, a médiaszerverben és a TV/web kliensben minden meglévő funkció megőrzésével.

### v1.4.2 (2026-11-26)
- **Bővített 30 lépéses kétnyelvű interaktív bemutató (HU/EN):** Teljes Médiaszerver és TV Központ bemutató lépésről lépésre vezetett vezeték nélküli TV app telepítési útmutatóval Android TV-hez (`.apk` + ADB) és Samsung Tizenhez (`.wgt` + SDB), szekciós gyorsugró gombokkal és az eddig hiányzó funkciókkal (Okos PC keresés, Folytatás és Következő sáv, Kollekció jobbklikkes menü, TV Direct Play / hang-optimalizálás).
- **Megújult Kollekció oldal:** Középre igazított kétsoros eszköztár, húzható méretezhető elválasztó a könyvespolc és a részletező panel között (`localStorage` mentéssel), valamint kétoszlopos részletező panel a poszter alatt sorakozó műveleti gombokkal és a jobb alsó sarokba helyezett `HU / EN` leírásváltóval.
- **Reszponzív lejátszó vezérlők & `960×580` minimum ablakméret:** Konténer-lekérdezésen alapuló reszponzív alsó vezérlősáv (keskenyebb ablaknál vagy széles oldalsávoknál automatikusan ikon-módba vált a Távirányító, TV-re küldés, Minilejátszó és Teljes képernyő gomb), dinamikus oldalsáv-szélesség korlátozás, a jobb oldalsáv `HU/EN`/`Névjegy`/`Bemutató` gombjainak szélességjavítása, valamint `960×580`-as főablak minimum (a `260×146`-os lebegő minilejátszó megőrzésével).
- **Megbízhatóbb Windows frissítések (NSIS háttérfolyamat-takarítás):** Telepítés, frissítés és eltávolítás előtt automatikusan leállítja a háttérben futó `adb.exe`, `sdb.exe`, `mediaserver.exe`, `ffmpeg.exe` és `ffprobe.exe` folyamatokat (megelőzve az `AdbWinApi.dll` zárolási hibát), valamint bezáráskor takarítja az `adb.exe`/`sdb.exe` démonokat.

### v1.4.1 (2026-11-26)
- **TV lejátszási értesítések áthelyezése:** A tekerési jelző (Seek HUD) és a lejátszás közbeni képernyő-értesítések a képernyő közepéről közvetlenül a seekbar fölé kerültek, így nem takarják el a középső navigációs gombokat.
- **Letisztult feliratbetöltés:** Eltávolításra került a teljes feliratsáv betöltésekor megjelenő, a betöltött sorok számát jelző értesítés.
- **TV kezdőképernyő tisztítása:** A „Transzkód Debug” menüpont elrejtve a TV alkalmazások kezdőképernyőjéről.
- **Frissített v1.4.1 csomagok:** Újracsomagolt Samsung Tizen (`.wgt`), Android TV (`.apk`), Médiaszerver és Windows asztali telepítő.

### v1.4.0 (2026-11-24)
- **Integrált CineVity Médiaszerver & FFmpeg csomag:** A telepítő immár alapból tartalmazza a hordozható CineVity Médiaszervert, a hardveres FFmpeg/FFprobe motorokat és a TV webes klienst — külön szervertelepítés vagy kézi beállítás nélkül működik bármely Windows PC-n.
- **Egykattintásos Android TV és Samsung Tizen TV App Telepítő:** Új **TV App Telepítő** fül a Médiaszerver központban, amely tartalmazza a beépített `CineVity-AndroidTV.apk` (+ ADB), `CineVity.wgt` (+ SDB) fájlokat, automatikus LAN TV kereséssel és lépésről lépésre útmutatóval.
- **Kétirányú Desktop ↔ TV szinkron & Cast-to-TV:** Élő eszközfelügyelet, felirat- és hangsáv-megtartás TV-re küldéskor, valamint pontos pozíció-szinkron Tizen TV-n és Android TV-n.
- **Okos PC keresés & Bizalmi áttekintő (Smart Scan PC):** Egygombos teljes meghajtó-szkennelés Filmek / Sorozatok / Egyéb videók intelligens kategorizálással és gyors javító modállal.
- **Angol-első TMDB keresés magyar felülírással:** Megbízhatóbb találatok ritkább címekre is, miközben a magyar cím, poszter és leírás automatikusan betöltődik, ha elérhető.
- **Frissített CineVity ikon & gyűjtemény-javítások:** Egységesített új ikon minden platformon, javított mappa-lenyíló rétegzés és teljes gyűjtemény/szerver takarítás mappa törlésekor.

### v1.3.0 (2026-11-20)
- **Telefonos távirányító (Wi-Fi & QR-kód):** Irányítsd a lejátszót telefonról ugyanazon a Wi-Fi hálózaton, külön alkalmazás telepítése nélkül. A beépített szerver QR-kódot és másolható címet generál a lejátszás, tekerés, hangerő, feliratok és sávok vezérléséhez.
- **Lebegő minilejátszó (PiP / Mindig felül):** Kompakt, más ablakok felett lebegő nézet szabadon húzható ablakkal, `S` / `M` / `L` méret-előbeállításokkal, 4 sarokba igazítással (`↖` `↗` `↙` `↘`), Mindig felül rögzítéssel és gyors vezérlőkkel (`P` / `Esc`).
- **Frissített interaktív bemutató:** A lépésről lépésre végigvezető bemutató (HU/EN) kiegészült a telefonos távirányító és a lebegő minilejátszó bemutatásával.

### v1.2.0 (2026-11-18)
- **Opcionális interaktív bemutató (HU/EN):** Első indításkor felajánlott, vagy a `?` / **Bemutató** gombbal bármikor újraindítható interaktív túra, amely kiemeli a lejátszó és a Kollekció fő funkcióit.
- **Névjegy oldal:** Dedikált Névjegy oldal az alkalmazás adataival, a szerzővel (**Dózsa Tamás**), technikai áttekintéssel, billentyűparancsokkal és kézi frissítés-ellenőrzéssel.
- **Verziószám a Windows címsorban:** Az alkalmazás verziószáma automatikusan megjelenik az ablak fejlécében (`CineVity vX.Y.Z`).

### v1.1.1 (2026-11-17)
- **Képernyőkitöltés (Fit to Screen) képarány:** Új képarány mód ultraszéles monitorokhoz és TV-khez.
- **mpv kompatibilitási javítás:** Javítva a `video-aspect-override` elavulási figyelmeztetés.

### v1.1.0 (2026-11-17)
- **Felirat megjelenésének testreszabása:** Állítható feliratméret (`XS`–`XL`), szín, körvonal és áttetsző sötét háttérdoboz.

### v1.0.1 (2026-11-17)
- **Hibajavítás:** Javítva az egérgörgős finomtekerés a Kollekcióból való visszatérés után.

### v1.0.0 (2026-11-17)
- **Első nyilvános kiadás:** GPU-gyorsított `libmpv` lejátszás, GLSL/AI felskálázás, 5 sávos Equalizer spektrum-analizátorral, Éjszakai mód (DRC), okos feliratkezelés (OpenSubtitles.com), TMDB Kollekció DVD-polc és aláírt automatikus frissítő.

---

## 🇬🇧 English

This document summarizes the new features and improvements added in each **CineVity** release.

### v1.5.0 (2026-11-27)
- **Bundled AI Upscaling Out of the Box:** The Windows installer now ships with the complete VapourSynth R73, embedded Python 3.12, VSORT DirectML runtime, and `2xNomosUni_compact_otf_medium.onnx` model pre-bundled — ready for instant activation with zero extra downloads.
- **Rebuilt CineVity Media Server & Updated TV/Web Client:** Fixed infinite loading on desktop Firefox and Brave browsers for 4K/HDR/HEVC titles on high-resolution monitors by separating `.is-4k` UI scaling from Samsung Tizen TV stream detection, plus improved native HLS handler ordering, fallbacks, and autoplay recovery.
- **Updated Bundled TV Apps & Dependencies:** Includes refreshed `CineVity-AndroidTV.apk` (+ ADB), `CineVity.wgt` (+ SDB), rebuilt `mediaserver.exe`, `ffmpeg.exe`/`ffprobe.exe`, and `libmpv-2.dll` all out of the box.
- **Comprehensive Security, Stability, Memory-Leak & Performance Hardening:** Full codebase audit fixes across the Desktop Player, Media Server, and TV Web Client while preserving all existing functionality.

### v1.4.2 (2026-11-26)
- **Expanded 30-Step Bilingual Interactive Tutorial (HU/EN):** Full Media Server & TV Hub walkthrough with step-by-step wireless TV app installation guides for Android TV (`.apk` + ADB) and Samsung Tizen (`.wgt` + SDB), section quick-jump pills, and coverage of previously missing features (Smart Scan PC, Continue Watching & Up Next, Collection context menu, TV Direct Play / Audio Optimization).
- **Redesigned Collection Page:** Centered 2-row toolbar, draggable resizable divider between bookshelf and details panes (saved in `localStorage`), and a 2-column details panel with stacked poster action buttons and a bottom-right `HU / EN` overview toggle.
- **Responsive Player Controls & `960×580` Minimum Window Size:** Container-query responsive bottom bar (auto-collapses Remote, Cast to TV, Mini-Player, Fullscreen to icon-only buttons on narrow viewports or wide sidebars), dynamic sidebar width clamping, right-sidebar `HU/EN`/`About`/`Tour` button width fix, and `960×580` minimum main window floor (preserving `260×146` Floating Mini-Player).
- **Reliable Windows Upgrades (NSIS Daemon Cleanup):** Automatically stops leftover `adb.exe`, `sdb.exe`, `mediaserver.exe`, `ffmpeg.exe`, and `ffprobe.exe` processes during install/upgrade/uninstall (fixing locked `AdbWinApi.dll` errors) and cleans up `adb.exe`/`sdb.exe` on app exit.

### v1.4.1 (2026-11-26)
- **Repositioned TV Playback Notifications:** Moved the seek HUD and playback on-screen notifications from the center of the screen to directly above the seekbar so they never overlap the center D-pad navigation controls.
- **Cleaner Subtitle Loading:** Removed the on-screen notification showing the number of subtitle lines loaded when loading a subtitle track.
- **Cleaner TV Home Screen:** Hidden the "Transzkód Debug" menu button from the TV apps' home screen.
- **Updated v1.4.1 Packages:** Rebuilt and bundled Samsung Tizen (`.wgt`), Android TV (`.apk`), Media Server, and Windows desktop installer packages.

### v1.4.0 (2026-11-24)
- **Integrated CineVity Media Server & FFmpeg Bundle:** The Windows installer now bundles the portable CineVity Media Server, FFmpeg/FFprobe binaries, and the TV web client out of the box—no separate downloads or hardcoded paths needed.
- **One-Click Android TV & Samsung Tizen TV App Installer:** New **TV App Installer** tab in the Media Server Hub with bundled `CineVity-AndroidTV.apk` (+ ADB), `CineVity.wgt` (+ SDB), automatic LAN TV scanning, and guided setup instructions.
- **Two-Way Desktop ↔ TV Sync & Cast-to-TV:** Live TV state tracking, preserved subtitle/audio selection when casting to TV, and accurate HLS resume positioning on both Samsung Tizen and Android TV.
- **Smart PC Scan & Confidence Review Modal:** One-button drive scanning with intelligent Movies / TV Series / Other Videos classification and inline TMDB review before importing.
- **English-First TMDB Matching with Hungarian Overlay:** Searches English metadata first for stronger matching on obscure titles while automatically applying Hungarian titles, posters, and overviews when available.
- **Refreshed CineVity App Icon & Collection Fixes:** Unified icon across Desktop, Tizen TV, and Android TV, plus scan dropdown z-index fix and full local + server cleanup on folder deletion.

### v1.3.0 (2026-11-20)
- **Phone as a Remote (Wi-Fi & QR Code):** Control playback, seeking, volume, subtitles, and tracks from your phone on the same Wi-Fi network with no app install required — just scan the generated QR code or copy the URL.
- **Floating Mini-Player (PiP / Always on Top):** Compact floating window with free dragging, `S` / `M` / `L` size presets, 4-corner snapping (`↖` `↗` `↙` `↘`), Always-on-Top pinning, and quick playback controls (`P` / `Esc`).
- **Updated Interactive Tutorial:** Added localized (HU/EN) guided tour steps for both Phone Remote and Floating Mini-Player.

### v1.2.0 (2026-11-18)
- **Optional Interactive Feature Tour (HU/EN):** Guided spotlight tour offered on first launch and replayable anytime via the **Bemutató / Tour** (`?`) button across both the Player and Collection views.
- **About Page:** Dedicated About page with app details, author info (**Dózsa Tamás**), technical stack, keyboard shortcuts, and manual update check.
- **Version in Windows Title Bar:** Displays the active version number in the default Windows window header (`CineVity vX.Y.Z`).

### v1.1.1 (2026-11-17)
- **Fit to Screen Aspect Ratio:** Added Fit to Screen aspect ratio mode for ultrawide monitors and TVs.
- **mpv Compatibility Fix:** Fixed `video-aspect-override` deprecation warning.

### v1.1.0 (2026-11-17)
- **Subtitle Visual Customization:** Added configurable subtitle size (`XS`–`XL`), color, outline, and transparent background box.

### v1.0.1 (2026-11-17)
- **Bug Fix:** Fixed mouse wheel fine-seeking after returning from Collection.

### v1.0.0 (2026-11-17)
- **Initial Release:** GPU-accelerated `libmpv` playback, GLSL/AI upscaling, 5-band Equalizer with spectrum analyzer, Night Mode (DRC), smart subtitles (OpenSubtitles.com), TMDB Collection DVD bookshelf, and signed auto-updater.
