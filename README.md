# CineVity — Modern Asztali Videólejátszó & Médiaszerver Központ / Modern Desktop Video Player & Media Hub

[🇭🇺 Magyar](#-magyar) | [🇬🇧 English](#-english) | [📝 Újdonságok / What's New](WHATS_NEW.md)

---

## 🇭🇺 Magyar

A **CineVity** egy modern, gyors és letisztult asztali videólejátszó Windowsra, amely natív `libmpv` GPU-lejátszást, gyárilag beépített **NomosUni 2× AI felskálázást**, beépített **CineVity Médiaszervert**, egykattintásos **Android TV / Samsung Tizen TV** app telepítést, kétirányú TV-szinkront, telefonos Wi-Fi távirányítót, lebegő minilejátszót, DVD-polcos TMDB médiakönyvtárat és intelligens feliratkezelést kínál egyetlen telepítőben.

### Letöltés és telepítés (Minden az egyben / Out-of-the-Box)

1. Nyisd meg a **[Legfrissebb kiadások (Releases)](https://github.com/kuriouss33/cinevity-releases/releases/latest)** oldalt.
2. Töltsd le a `CineVity_1.5.0_x64-setup.exe` (vagy a legújabb `CineVity_..._x64-setup.exe`) telepítőt.
3. Futtasd a telepítőt, majd indítsd el a **CineVity** alkalmazást.

> **Gyárilag előkészített csomag (Out-of-the-Box):** A Windows telepítő alapból tartalmaz minden szükséges futtatókörnyezetet — a `libmpv` motort, a teljes **AI felskálázó futtatókörnyezetet** (`VapourSynth R73` + beágyazott Python 3.12 + `VSORT DirectML` + `2xNomosUni_compact_otf_medium.onnx`), a hordozható **CineVity Médiaszervert** (`mediaserver.exe`, `ffmpeg.exe`, `ffprobe.exe` és TV/Web klienst), valamint a csomagolt TV-telepítőket (`CineVity-AndroidTV.apk` + ADB és aláírt `CineVity.wgt` + SDB). Külön letöltés vagy kézi konfiguráció nem szükséges.
>
> **Automatikus és megbízható frissítések:** Indításkor a CineVity automatikusan ellenőrzi a digitálisan aláírt (Minisign) frissítéseket, a telepítő pedig frissítés/eltávolítás előtt leállítja a háttérben futó segédfolyamatokat (`mediaserver.exe`, `adb.exe`, `sdb.exe`), így a frissítés mindig zökkenőmentes. A verziótörténet a [WHATS_NEW.md](WHATS_NEW.md) fájlban érhető el.

---

### Főbb funkciók

- **GPU-gyorsított lejátszás (`libmpv`):** Hardveres dekódolás és `gpu-next` (`d3d11`) megjelenítés széles videó- és hangformátum-támogatással, automatikus HDR tónustérképezéssel.
- **Beépített NomosUni 2× AI felskálázás & Képarányok:**
  - **NomosUni 2× AI felskálázás** (`VapourSynth R73` + beágyazott Python 3.12 + `VSORT DirectML` + ONNX modell) azonnal aktiválható külső letöltés nélkül ≤ 720p videókhoz, automatikus felbontás-kikerüléssel 720p felett.
  - Képarány-módok ultraszéles monitorokhoz és TV-khez, beleértve a **Képernyőkitöltés (Fit to Screen)** módot.
- **Stúdió hangrendszer:**
  - 5 sávos **Equalizer** valós idejű spektrum-analizátorral és előre beállított profilokkal
  - **3D Térhang (Spatial Audio)** és **Vokál-elnémítás**
  - **Éjszakai mód (Night Mode / DRC):** Tisztább párbeszédek halkabb hangerő mellett is
  - **S/PDIF AC3 5.1 passthrough** házimozi erősítőkhöz
- **Beépített CineVity Médiaszerver & LAN Web/TV Streaming:**
  - Egy kattintással indítható helyi médiaszerver hardveres `FFmpeg`/`FFprobe` HLS átkódolással és 4K HDR DirectStream móddal.
  - Natívan használható **Samsung Tizen TV-n**, **Android TV-n**, **iPad / Safari** eszközökön és **asztali böngészőkben** (Firefox, Brave, Chrome).
- **Egykattintásos TV App Telepítő:**
  - Beépített **TV App Telepítő** a Médiaszerver központban: automatikus LAN TV felderítés és vezeték nélküli telepítés a csomagolt `CineVity-AndroidTV.apk` (+ `adb.exe`) és aláírt `CineVity.wgt` (+ `sdb.exe`) csomagokkal, lépésről lépésre útmutatóval.
- **Kétirányú Desktop ↔ TV szinkron & Cast-to-TV:**
  - Valós idejű eszközfigyelés és azonnali küldés TV-re vagy asztali böngészőbe a kiválasztott hangsáv, feliratsáv és pontos lejátszási pozíció megőrzésével.
- **Telefonos távirányító (Wi-Fi & QR-kód):**
  - Irányítsd a lejátszót okostelefonod böngészőjéből külön mobilapp telepítése nélkül a generált QR-kóddal vagy helyi URL-lel (lejátszás, tekerés, hangerő, sávváltás, feliratok).
- **Lebegő minilejátszó (PiP / Mindig felül):**
  - Szabadon húzható kompakt lejátszóablak `S` / `M` / `L` méret-előbeállításokkal, 4 sarokba igazítással (`↖` `↗` `↙` `↘`), **Mindig felül** rögzítéssel és gyors billentyűkkel (`P` / `Esc`).
- **Médiakönyvtár, DVD-polc & Okos PC keresés:**
  - Filmek, Sorozatok és Egyéb videók rendszerezése 3D DVD-polcon húzható, mentett arányú elválasztóval, kétoszlopos részletezővel és jobb alsó `HU / EN` leírásváltóval.
  - **Folytatás és Következő sáv (Continue Watching & Up Next)**, továbbá TV Direct Play kompatibilitás-ellenőrzés és hang-optimalizálás.
  - **Okos PC keresés (Smart Scan PC):** Egygombos meghajtó-szkennelés előnézeti és **Bizalmi áttekintő (Confidence Review)** modállal, valamint angol-első TMDB keresés automatikus magyar felülírással.
- **Okos feliratkezelés:**
  - Beépített és helyi `.srt` / `.vtt` feliratok automatikus felismerése, ms/s csúszás-szinkronizálás.
  - Testreszabható felirat-megjelenés (`XS`–`XL` méret, szín, körvonal, áttetsző sötét háttérdoboz).
  - Online **OpenSubtitles.com** keresés, egykattintásos letöltés, saját fiókos bejelentkezés és automatikus letöltés.
- **Pontos vezérlés, Pillanatképek, 30 lépéses Bemutató & Névjegy:**
  - Forgatható **Jog tárcsa** (Képkocka / `0.1s` / `1.0s`), finom tekerés egérgörgővel, `0.25x–3.0x` sebesség, ismétlés és azonnali nagy felbontású pillanatképek a `Képek\CineVity` (`Pictures\CineVity`) mappába.
  - Beépített **30 lépéses kétnyelvű interaktív bemutató (HU/EN)** (`?` gomb) és dedikált **Névjegy** oldal kézi frissítés-ellenőrzéssel.

---

### Gyors használati útmutató

- **Videó megnyitása:** Kattints a fájl megnyitása gombra, húzd rá a videót, vagy nyiss meg bármilyen videófájlt társítással a CineVity-vel.
- **AI felskálázás bekapcsolása:** Használd az oldalsáv **AI Felskálázás** kapcsolóját ≤ 720p tartalmak valós idejű 2× javításához — a telepítő minden szükséges összetevőt alapból tartalmaz.
- **Könyvtár & Okos PC keresés:** Nyisd meg a **Kollekció** nézetet, adj hozzá mappákat vagy futtasd az **Okos PC keresést** a Filmek / Sorozatok / Egyéb videók automatikus TMDB párosításához.
- **Médiaszerver & TV telepítés:** Nyisd meg a **Médiaszerver** központot a szerver indításához, a TV alkalmazások (Android TV / Samsung Tizen) vezeték nélküli telepítéséhez és a **TV-re küldéshez**.
- **Telefonos távirányító & Minilejátszó:** A felső/alsó vezérlősávon egy kattintással generálhatsz QR-kódot a telefonos távirányítóhoz, vagy válthatsz lebegő minilejátszóra (`P`).
- **Feliratok & Hang:** A felirat panelen válassz helyi/beágyazott sávot, állítsd a megjelenést vagy lépj be az OpenSubtitles-fiókodba; a hangpanelen érd el az Equalizert, a 3D Térhangot és az Éjszakai módot (`N`).
- **Bemutató & Névjegy:** Kattints a `?` (**Bemutató**) gombra a 30 lépéses interaktív túrához, vagy nyisd meg a **Névjegy** oldalt a kézi frissítés-ellenőrzéshez.

### Billentyűparancsok

| Billentyű | Művelet |
| --- | --- |
| `Space` | Lejátszás / Szünet |
| `F` | Teljes képernyő ki/be |
| `P` | Lebegő minilejátszó (PiP / Mindig felül) |
| `Esc` | Kilépés a teljes képernyőből / minilejátszóból |
| `M` | Némítás ki/be |
| `↑` / `↓` | Hangerő +5% / -5% |
| `←` / `→` | Tekerés -5 mp / +5 mp |
| `Shift` + `←` / `→` | Előző / Következő videó |
| `[` / `]` | Sebesség -0.25x / +0.25x |
| `Backspace` | Sebesség visszaállítása (1.0x) |
| `A` | Képarány váltása |
| `N` | Éjszakai mód (DRC) ki/be |
| `S` | Képernyőkép készítése |
| `I` | Film / Sorozat részletek |
| `Z` / `X` | Felirat szinkron -0.1 mp / +0.1 mp |
| `Alt` + `Z` / `X` | Felirat szinkron -1.0 mp / +1.0 mp |
| `J` / `K` | Hang szinkron -0.1 mp / +0.1 mp |

---

## 🇬🇧 English

**CineVity** is a modern, fast, and clean desktop video player for Windows combining native `libmpv` GPU playback, out-of-the-box **NomosUni 2× AI Upscaling**, a built-in **CineVity Media Server**, one-click **Android TV / Samsung Tizen TV** app installation, two-way TV sync, a browser-based Wi-Fi Phone Remote, a Floating Mini-Player, a TMDB DVD bookshelf library, and smart subtitle management in a single all-in-one installer.

### Download & Installation (Out of the Box)

1. Visit the **[Latest Releases](https://github.com/kuriouss33/cinevity-releases/releases/latest)** page.
2. Download the `CineVity_1.5.0_x64-setup.exe` (or the latest `CineVity_..._x64-setup.exe`) installer.
3. Run the installer and launch **CineVity**.

> **All Dependencies Bundled Out of the Box:** The Windows installer pre-bundles every runtime dependency—`libmpv`, the full **AI Upscaling runtime** (`VapourSynth R73` + embedded Python 3.12 + `VSORT DirectML` + `2xNomosUni_compact_otf_medium.onnx`), the portable **CineVity Media Server** (`mediaserver.exe`, `ffmpeg.exe`, `ffprobe.exe`, and the TV/Web client), plus the **TV App Installers** (`CineVity-AndroidTV.apk` + ADB and signed `CineVity.wgt` + SDB). No manual setup or extra downloads are required.
>
> **Automatic & Reliable Updates:** On startup, CineVity checks for Minisign-verified updates and prompts to download, install, and relaunch automatically. Before upgrading or uninstalling, the NSIS hooks terminate background helper processes (`mediaserver.exe`, `adb.exe`, `sdb.exe`) to ensure clean file replacement. See [WHATS_NEW.md](WHATS_NEW.md) for full release notes.

---

### Key Features

- **Smooth GPU Playback (`libmpv`):** Hardware-accelerated `gpu-next` (`d3d11`) video rendering with broad codec support and automatic HDR tone-mapping.
- **Bundled NomosUni 2× AI Upscaling & Aspect Ratios:**
  - **NomosUni 2× AI Upscaling** (`VapourSynth R73` + embedded Python 3.12 + `VSORT DirectML` + ONNX model) works immediately out of the box for ≤ 720p videos, automatically bypassing higher-resolution sources.
  - Smart aspect ratio presets for widescreen and ultrawide displays, including **Fit to Screen**.
- **Studio Audio Suite:**
  - 5-band **Equalizer** with live spectrum analyzer and presets
  - **3D Spatial Audio** and **Vocal Mute**
  - **Night Mode (DRC):** Clearer dialogue at lower volumes
  - **S/PDIF AC3 5.1 passthrough** for home theater receivers
- **Integrated CineVity Media Server & LAN Web/TV Streaming:**
  - Launch the local media server in one click with hardware `FFmpeg`/`FFprobe` HLS transcoding and 4K HDR DirectStream support.
  - Streams to **Samsung Tizen TV**, **Android TV**, **iPad / Safari**, and **desktop browsers** (Firefox, Brave, Chrome).
- **One-Click TV App Installer:**
  - Built-in **TV App Installer** tab in the Media Server Hub featuring automatic LAN TV discovery, bundled `CineVity-AndroidTV.apk` (+ `adb.exe`) and signed `CineVity.wgt` (+ `sdb.exe`), and guided wireless installation.
- **Two-Way Desktop ↔ TV Sync & Cast-to-TV:**
  - Live device monitoring and instant casting to TVs or web browsers while preserving audio track, subtitle track, and resume position.
- **Phone as a Remote (Wi-Fi & QR Code):**
  - Control playback, seeking, volume, tracks, and subtitles from any phone browser on the same Wi-Fi network via QR code or copyable URL—no mobile app required.
- **Floating Mini-Player (PiP / Always on Top):**
  - Draggable compact floating window with `S` / `M` / `L` size presets, 4-corner snapping (`↖` `↗` `↙` `↘`), Always-on-Top pinning, and quick controls (`P` / `Esc`).
- **Media Library, DVD Bookshelf & Smart PC Scan:**
  - Organize Movies, TV Series, and Other Videos on a DVD bookshelf with a draggable saved split-pane divider, two-column details panel, and bottom-right `HU / EN` overview toggle.
  - **Continue Watching & Up Next** hub, TV Direct Play compatibility diagnostics, and TV audio optimization.
  - **Smart PC Scan:** One-button drive scanning with intelligent categorization and a **Confidence Review Modal**, powered by English-first TMDB matching with automatic Hungarian metadata overlay.
- **Smart Subtitles:**
  - Embedded track selection and automatic local `.srt` / `.vtt` discovery with millisecond/second sync controls.
  - Customizable subtitle styling (`XS`–`XL` size, color, outline, translucent dark background box).
  - Online **OpenSubtitles.com** search, one-click download, personal account login, and auto-download.
- **Precision Controls, Screenshots, 30-Step Interactive Tour & About Page:**
  - Rotary **Jog Wheel** (Frame / `0.1s` / `1.0s`), fine mouse wheel seeking, `0.25x–3.0x` playback speed, loop controls, and high-resolution screenshots saved to `Pictures\CineVity`.
  - Built-in **30-step bilingual interactive tour (HU/EN)** (`?` button) and dedicated **About** page (author: Dózsa Tamás) with manual update checking.

---

### Quick User Guide

- **Playing a Video:** Click the open file button, drag-and-drop a video, or open any media file directly with CineVity.
- **AI Upscaling:** Toggle **AI Upscaling** in the sidebar to enhance ≤ 720p videos in real time—all runtime components are already pre-bundled.
- **Library & Smart PC Scan:** Switch to **Collection** to add media folders or run **Smart Scan PC** for automated TMDB matching across Movies, TV Series, and Other Videos.
- **Media Server & TV Setup:** Open the **Media Server Hub** to start streaming over LAN, install the bundled Android TV (`.apk`) or Samsung Tizen (`.wgt`) client wirelessly, or cast directly to a connected device.
- **Phone Remote & Mini-Player:** Click the Phone Remote button to scan the QR code from your phone, or press `P` to switch into the Floating Mini-Player.
- **Subtitles & Audio:** Open the Subtitles drawer for embedded/local tracks, visual styling, sync offsets, or OpenSubtitles.com search & login; open the Audio drawer for the 5-band Equalizer, Spatial Audio, and Night Mode (`N`).
- **Tour & About:** Click `?` (**Tour**) anytime for the 30-step walkthrough, or visit **About** to review shortcuts and check for updates.

### Keyboard Shortcuts

| Key | Action |
| --- | --- |
| `Space` | Play / Pause |
| `F` | Toggle Fullscreen |
| `P` | Toggle Floating Mini-Player (PiP / Always on Top) |
| `Esc` | Exit Fullscreen / Mini-Player |
| `M` | Toggle Mute |
| `↑` / `↓` | Volume +5% / -5% |
| `←` / `→` | Seek -5s / +5s |
| `Shift` + `←` / `→` | Previous / Next track |
| `[` / `]` | Speed -0.25x / +0.25x |
| `Backspace` | Reset speed (1.0x) |
| `A` | Toggle Aspect Ratio |
| `N` | Toggle Night Mode (DRC) |
| `S` | Take Screenshot |
| `I` | Movie / TV Show details |
| `Z` / `X` | Subtitle delay -0.1s / +0.1s |
| `Alt` + `Z` / `X` | Subtitle delay -1.0s / +1.0s |
| `J` / `K` | Audio delay -0.1s / +0.1s |

---

## 🛠️ Technical Overview (For Developers)

### Core Architecture & Stack
- **Desktop Frontend:** React 19, TypeScript, Vite 8, Lucide React
- **Desktop Backend:** Rust (Edition 2024), Tauri v2
- **Media Playback Engine:** `libmpv` (`libmpv-2.dll` / `libmpv2` crate) with native Windows `HWND` embedding and `gpu-next` (`d3d11`) rendering
- **AI Upscaling Pipeline (Bundled):** Portable `VapourSynth R73` + embedded Python 3.12 (`PYTHONDONTWRITEBYTECODE=1`) + `VSORT` (`DirectML.dll` + `onnxruntime.dll`) + `2xNomosUni_compact_otf_medium.onnx`
- **Integrated Media Server (Bundled):** Rust Axum/Tokio HTTP & WebSocket server (`mediaserver.exe`), hardware-accelerated `FFmpeg` / `FFprobe` HLS transcoder + DirectStream, and a Chromium M63-compatible TV/Web client
- **TV Client Installers (Bundled):** Native Kotlin/ExoPlayer Android TV app (`CineVity-AndroidTV.apk` + `adb.exe`) and Samsung Tizen TV package (`CineVity.wgt` + `sdb.exe`)
- **Database:** Embedded SQLite via `rusqlite` (`bundled` feature)
- **Automation:** PowerShell release pipeline (`scripts/release.ps1`)

### Tauri v2 Plugins & Capabilities
- `tauri-plugin-dialog` — Native file/folder pickers and update confirmation dialogs
- `tauri-plugin-window-state` — Window size and position persistence (with safe `960×580` minimum floor and Mini-Player restoration)
- `tauri-plugin-updater` — Signed update checks, downloads, and installation
- `tauri-plugin-process` — Application relaunch after updates

### External Integrations
- **TMDB API:** Movie/TV metadata, artwork, and episode details (English-first lookup with Hungarian overlay)
- **OpenSubtitles.com REST API:** Subtitle search, download, and personal account authentication

### Build, Signing & Release Pipeline
- **Bundler:** Tauri Windows x64 NSIS target (`tauri.conf.json` + `tauri.windows.conf.json` + `nsis/hooks.nsh`) producing an all-in-one `CineVity_<version>_x64-setup.exe`
- **Security:** Minisign cryptographic signing (`TAURI_SIGNING_PRIVATE_KEY` / `-KeyPassword` / `-PromptPassword`) generating `.sig` updater artifacts
- **Distribution:** `scripts/release.ps1` syncs versions across `package.json`, `src-tauri/Cargo.toml`, and `src-tauri/tauri.conf.json`, builds & signs the installer, generates `latest.json`, and publishes the release to [`kuriouss33/cinevity-releases`](https://github.com/kuriouss33/cinevity-releases) via GitHub CLI (`gh`).
