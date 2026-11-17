CineVity — Modern Desktop Video Player

A modern, high-performance desktop video player built with Tauri v2, React, TypeScript, and libmpv.

Features
Native GPU Video Engine: Hardware-accelerated playback powered by libmpv with support for a wide range of video/audio codecs and containers.
AI & Shader Upscaling: Real-time upscaling shaders (FSRCNNX, Lanczos Sharp, Cinema Smooth) and aspect ratio controls.
Studio Audio Suite:
5-band parametric equalizer with presets
Spatial audio & vocal isolation/muting
Night Mode / DRC (Dynamic Range Compression) for clear dialogue at low volume
S/PDIF AC3 passthrough
Precision Playback Controls: Frame-by-frame jog wheel scrubbing, fine mouse wheel seeking, playback speed, and A-B/looping controls.
Smart Subtitles:
Embedded subtitle track picker
Automatic local subtitle discovery
Online OpenSubtitles.com search, download, BYO account login, and auto-download
Media Library & Collections:
Local SQLite-backed library for Movies and TV Series
Automatic metadata, posters, and episode details via TMDB
Playback progress tracking and resume support
High-Res Screenshots: Instant frame capture saved to Pictures/CineVity.
Auto-Updater: Checks for new releases on startup and prompts with a native dialog to download, install, and relaunch.
Tech Stack
Frontend: React 19, TypeScript, Vite, Lucide Icons
Backend: Rust, Tauri v2 (tauri-plugin-dialog, tauri-plugin-window-state, tauri-plugin-updater, tauri-plugin-process)
Media & Storage: libmpv2, rusqlite (bundled SQLite)
User Guide
Opening & Playing Media
Click Open File (or drag/open a file via the OS) to start playback immediately.
Add folders or media items to your Library / Collections to browse Movies and TV Shows with TMDB metadata, season/episode lists, and resume progress.
Video & Audio Controls
Upscaling: Switch between off, FSRCNNX, Lanczos Sharp, and Cinema Smooth shaders in the player controls.
Audio: Open the Equalizer panel to adjust the 5-band EQ, choose presets, or toggle Night Mode, Spatial Audio, Vocal Mute, and S/PDIF AC3.
Screenshots: Use the camera button to capture the current frame to Pictures/CineVity.
Subtitles & OpenSubtitles.com
Local & Embedded: Embedded tracks and matching local .srt/.vtt files are detected automatically.
Online Search: Open the Subtitles panel to search OpenSubtitles.com. You can optionally sign in with your own OpenSubtitles account (Fiók) to use your personal download quota and enable automatic subtitle downloads.
Automatic Updates
When online, CineVity checks for updates shortly after startup.
If a newer version is available, a native dialog displays the version and release notes. Click Frissítés to download, install, and relaunch automatically, or Később to skip.
