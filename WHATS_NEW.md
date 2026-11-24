# CineVity — Újdonságok / What's New

[🇭🇺 Magyar](#-magyar) | [🇬🇧 English](#-english)

---

## 🇭🇺 Magyar

Ez a dokumentum összefoglalja a **CineVity** egyes kiadásainak új funkcióit és fejlesztéseit.

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
