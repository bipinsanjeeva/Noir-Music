<div align="center">
  <img src="assets/banner.png" alt="Noir Music Logo"/>

  <p><b>A modern Android music app with ad-free streaming, synced lyrics, offline playback, and an intuitive user experience.</b></p>
</div>

---

## Overview

Noir Music is an independent fork of the Echo Music open-source project, with a customized identity and user interface.

Noir Music delivers a seamless, premium listening experience by leveraging YouTube Music's vast library — without the ads. It adds powerful extras including offline downloads, real-time synchronized lyrics, and environment-aware music recognition.

> [!IMPORTANT]
> **In-app OTA updates have been permanently removed.** Please update manually via the website. Noir Music is completely free and ad-free; the few ads shown during a manual download help support the ongoing development of this project. Please do not open issues requesting to bring this back. Thank you for your support!

---

## Table of Contents

- [Overview](#overview)
- [Screenshots](#screenshots)
- [Features](#features)
- [Installation & Setup](#installation--setup)
- [Support the Project](#support-the-project)
- [Contributors](#contributors)
- [Special Thanks](#special-thanks)
- [Legal Disclaimer & Terms of Use](#legal-disclaimer--terms-of-use)

---

## Screenshots

<div align="left">
  <table style="margin: 0 auto; border-collapse: collapse;">
    <tr>
      <td align="center" style="padding: 15px; border: none;">
        <b>Home Screen</b><br><br>
        <img src="Screenshots/Home.png" alt="Home Screen" width="220" style="border-radius: 12px; box-shadow: 0 8px 16px rgba(0,0,0,0.2);"/>
      </td>
      <td align="center" style="padding: 15px; border: none;">
        <b>Material Player</b><br><br>
        <img src="Screenshots/Material%20you%20music%20page.png" alt="Material Player" width="220" style="border-radius: 12px; box-shadow: 0 8px 16px rgba(0,0,0,0.2);"/>
      </td>
      <td align="center" style="padding: 15px; border: none;">
        <b>Apple Style Player</b><br><br>
        <img src="Screenshots/Apple%20inspired%20music%20page.png" alt="Apple Style Player" width="220" style="border-radius: 12px; box-shadow: 0 8px 16px rgba(0,0,0,0.2);"/>
      </td>
    </tr>
    <tr>
      <td align="center" style="padding: 15px; border: none;">
        <b>Synchronized Lyrics</b><br><br>
        <img src="Screenshots/lyrics.png" alt="Synchronized Lyrics" width="220" style="border-radius: 12px; box-shadow: 0 8px 16px rgba(0,0,0,0.2);"/>
      </td>
      <td align="center" style="padding: 15px; border: none;">
        <b>Search & Explore</b><br><br>
        <img src="Screenshots/search%20page.png" alt="Search & Explore" width="220" style="border-radius: 12px; box-shadow: 0 8px 16px rgba(0,0,0,0.2);"/>
      </td>
      <td align="center" style="padding: 15px; border: none;">
        <b>Music Library</b><br><br>
        <img src="Screenshots/library.png" alt="Music Library" width="220" style="border-radius: 12px; box-shadow: 0 8px 16px rgba(0,0,0,0.2);"/>
      </td>
    </tr>
  </table>
</div>

---

## Features

### What's New

> - **Data Saver Mode (Beta)** — Automatically reduces data usage during playback for limited connections.
> - **Settings Search Index** — Quickly find and navigate to any settings option instantly.
> - **Redesigned UI** — Cleaner, faster, and more intuitive interface from the ground up.
> - **Import & Sync from Spotify** — Bring your playlists over with ease and keep them up-to-date with one-tap Fast Sync.
> - **Listen Together** — Sync music in real time, similar to Spotify Jam.
> - **Podcast Support** — Listen to podcasts alongside your music library.
> - **Local Media Support** — Play music files stored directly on your device.
> - **Dynamic Island Support** — Enhanced playback notifications on supported Android devices.

<br>

<details>
<summary><b>Streaming & Playback</b></summary>
<br>

- **Ad-Free** — Stream without any interruptions.
- **Data Saver Mode** — Reduce data consumption when streaming on cellular networks.
- **Seamless Playback** — Switch effortlessly between audio-only and video modes.
- **Background Playback** — Listen while using other apps or with the screen off.
- **Offline Mode** — Download tracks, albums, and playlists via a dedicated download manager.
- **Crossfade** — Smooth transitions between tracks.
- **Canvas Animations** — Visual animations while playing music.

</details>

<details>
<summary><b>Discovery & Echo Find</b></summary>
<br>

- **Echo Find** — Identify songs playing around you using advanced audio recognition.
- **Echo Brain** — An intelligent, on-device engine that analyzes your listening momentum and auto-injects perfectly aligned tracks into your queue. Read more in the [Echo Brain Documentation](ECHO_BRAIN_DOCS.md).
- **Smart Recommendations** — Personalized suggestions based on your listening history.
- **Comprehensive Browsing** — Explore Charts, Podcasts, Moods, and Genres.

</details>

<details>
<summary><b>Lyrics</b></summary>
<br>

- **Multiple Lyric Animations** — Choose from various lyric display styles.
- **Word-by-Word Lyrics** — Precise per-word synchronization.
- **Lyrics+</b> — New lyrics provider for improved accuracy and coverage.
- **AI Translation** — Built-in Google Translate integration for lyrics in any language.

</details>

<details>
<summary><b>Integrations</b></summary>
<br>

- **Music Sharing via Odesli** — Share songs as Song.link for cross-platform listening.
- **Set as Ringtone** — Directly set any song as your device ringtone.

</details>

<details>
<summary><b>Smart Playback</b></summary>
<br>

- **Pause on Mute** — Auto-pause when your device is muted.
- **Resume on Bluetooth** — Playback resumes when headphones or earbuds reconnect.

</details>

<details>
<summary><b>Customization</b></summary>
<br>

- **UI Density Scale** — Adjust interface spacing to your preference.
- **High Refresh Rate Support** — Smoother UI and animations on supported displays.
- **Fluid UI & Animations** — Material 3 Emphasized easing and GPU-accelerated lyrics for a silky smooth, lag-free experience.
- **Hide Player Thumbnail** — Keep the player minimal without album art.
- **Crop Album Art** — Adjust album art display to fit your style.
- **Hide Video Songs** — Filter out video content from your feed.
- **Hide YouTube Shorts** — Keep Shorts out of your music browsing.

</details>

---

## Installation & Setup

### Android Installation

Download the latest pre-compiled APK from the [Noir Music Releases Page](https://github.com/bipinsanjeeva/Echo-Music/releases).

<details>
<summary><b>Building from Source</b></summary>
<br>

1. **Clone the Repository**

   ```bash
   git clone https://github.com/bipinsanjeeva/Echo-Music.git
   cd Echo-Music

2. Configure Android SDK
   Create a local.properties file:
   echo "sdk.dir=/path/to/your/android/sdk" > local.properties

   (For detailed paths on Windows/macOS/Linux, refer to [SETUP.md](SETUP.md))
3. Firebase Configuration (Optional)
   Firebase configuration is optional depending on the build configuration. See [SETUP.md](SETUP.md) for configuration instructions.
4. Build the Application
   Noir Music has two build variants: FOSS and GMS.
    - To build the FOSS Universal Debug variant:
      ./gradlew assembleUniversalFossDebug
    - To build the GMS Universal Debug variant:
      ./gradlew assembleUniversalGmsDebug
      (For optimized ARM64 builds, release builds, or other options, refer to [SETUP.md](SETUP.md))
</details>

Support the Project
If Noir Music has been useful to you, consider supporting its development.
<div align="left">
  <table style="margin: 0 auto; border-collapse: collapse; border: none;">
    <tr>
      <td align="center" style="padding: 15px; border: none;">
        <a href="https://buymeacoffee.com/bipinsanjeeva" style="text-decoration:none;">
          <img src="assets/bmac.png" alt="Buy Me A Coffee Logo" width="140" style="border-radius: 12px; box-shadow: 0 8px 16px rgba(0,0,0,0.2);"/>
        </a>
      </td>

  <td align="center" style="padding: 15px; border: none;">
    <a href="upi://pay?pa=here.bipins@oksbi&pn=Noir%20Music&cu=INR" style="text-decoration:none;">
      <img src="assets/UPI.png" alt="UPI Logo" width="140" style="border-radius: 12px; box-shadow: 0 8px 16px rgba(0,0,0,0.2);"/>
    </a>
  </td>
</tr>

  </table>
</div>

Contributors
Noir Music is an independent fork of the Echo Music open-source project.
The original project and its contributors remain credited through the project's source history and attribution. This fork does not claim ownership of the original contributors' work.
Special Thanks
Noir Music stands on the shoulders of several excellent open-source projects. Sincere thanks to:
Project	Description
Metrolist & Vivi Music	Foundational inspiration and architecture reference
ArchiveTune	Material You UI inspiration
Better Lyrics	Lyrics enhancement and synchronization
SimpMusic	Lyrics implementation reference
Music Recognizer	Audio recognition
BravePipe	Decryption handling and backup playback engine


Legal Disclaimer & Terms of Use
1. Open-Source Project
   Noir Music is an open-source fork of the Echo Music project and is distributed under the GPL-3.0 license.
   This project is provided for educational and personal use. Please review the applicable licenses and terms of the services accessed through the application.
2. Third-Party Content
   Noir Music is a third-party client that accesses publicly available content and services provided by third parties, including YouTube and YouTube Music.
   Noir Music is not affiliated with, endorsed by, or sponsored by YouTube, Google, or the original Echo Music developers.
3. Support Content Creators
   We respect the work of artists, musicians, and content creators.
   Users are encouraged to support creators through official platforms and services.
4. No Hosting of Copyrighted Material
   Noir Music does not host or upload audio, video, or other copyrighted media on its own servers.
   Content accessed through the application remains the property of its respective copyright owners.
5. User Responsibility
   The software is provided "AS IS", without warranty of any kind.
   Users are responsible for ensuring that their use of the application complies with applicable laws and the Terms of Service of the platforms they access.
   For concerns regarding the Noir Music project or its code, contact:
   bipinhere.work@gmail.com