## ⚙️ Bundled Dependencies

Meowsic includes two external binaries distributed in upstream releases. Both are bundled **unmodified**, and are provided under their own licenses:

| Component               | Purpose                | Source Archive                                               | License                                                    |
| ----------------------- | ---------------------- | ------------------------------------------------------------ | ---------------------------------------------------------- |
| `yt-dlp.exe` / `yt-dlp` | YouTube downloader     | Released from [yt-dlp / Unlicense]                           | **Unlicense** (public domain)                              |
| `ffmpeg.exe` / `ffmpeg` | FFmpeg with GPL codecs | Binaries from [BtbN/FFmpeg-Builds (win64/gpl / linux64/gpl)] | **GPL v2+/v3+** (due to enabled codecs) + MIT LGPL wrapper |

> **Note**: These tools are not maintained by Meowsic and may be replaced at runtime.

---

## 📄 Included License Files

In each release ZIP (`win64.zip`, `linux64.zip`), the following files are included at the top level:

```
yt-dlp(.exe)
ffmpeg(.exe)
LICENSE-yt-dlp          ← Unlicense text
LICENSE-ffmpeg-gpl      ← FFmpeg GPL license text
LICENSE-ffmpeg-builds   ← MIT license from BtbN/FFmpeg-Builds
FFmpeg-source-offer     ← Written offer to obtain the FFmpeg source code
```

- **The GPL license text** is extracted verbatim from the FFmpeg upstream’s `LICENSE.txt`.
- **`FFmpeg-source-offer`** is a written notice linking to the **exact release archive** and repo used, satisfying GPL §6/§4 for binary distribution without source.
- The **Unlicense** is public domain—exempts copyleft—but `LICENSE-yt-dlp` is included for transparency.
- The **MIT license** is included because BtbN’s build scripts and wrapper are MIT-licensed and upstream to the FFmpeg binary you redistribute.

---

## 🌐 Archived Source URLs

Sources for user verification (embedded in `FFmpeg-source-offer`):

- FFmpeg (GPL-enabled build):  
  `https://github.com/BtbN/FFmpeg-Builds/releases/latest`

- yt-dlp:  
  `https://github.com/yt-dlp/yt-dlp`

These URLs point to the **exact upstream versions** bundled in each Meowsic release.

---

## 🖥️ Supported Architectures

All builds currently provide **64-bit binaries** only:

- ✅ `win64` (Windows 64-bit)
- ✅ `linux64` (Linux x86_64)
- ❌ `winarm64` (Not yet supported)
- ❌ `linuxarm64` (Not yet supported)

---

## 📜 Legal Notes & Disclaimers

- **GPL Compliance**: Redistributing FFmpeg executables requires **both** the license text and a valid **source offer**—which are included as `LICENSE-ffmpeg-gpl` and `FFmpeg-source-offer` respectively.

- **Unlicense**: yt-dlp is in the public domain under the Unlicense; there are no copyleft restrictions, but attribution and transparency are preserved.

- **YouTube Terms of Service (TOS)**: Meowsic’s distribution of these tools **does not imply People-centric use is TOS-compliant**. Users must comply with [YouTube’s API and content TOS](https://developers.google.com/youtube/terms) if they use Meowsic to access or redistribute YouTube content.

- **User Responsibility**: By using Meowsic, you acknowledge you are responsible for any legal risks arising from how yt-dlp and ffmpeg are used—including copyright and streaming. Meowsic itself does not host or modify these tools.
