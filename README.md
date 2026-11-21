<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="images/vidona-logo-white.png">
    <img src="images/vidona-logo-black.png" alt="Vidona" width="360">
  </picture>
</p>

<p align="center"><b>Turn long videos into ready-to-post short clips, on your own Windows PC.</b></p>

Vidona takes a long video (a podcast, an interview, a stream) and helps you turn it into vertical clips for TikTok, YouTube Shorts and Instagram Reels. AI finds the moments worth clipping, you choose the ones you want, and Vidona frames, captions and edits them.

## Download

**[Download the latest version from the Releases page](https://github.com/sufyanahmadkamboh/vidona-release/releases/latest)**: the file is `Vidona-Setup-<version>.exe`.

This repository only holds the installer. The source code is private.

## What it does

1. **Import** a long video. Vidona transcribes it with Deepgram (fast, paid with your own key) or with Whisper on your PC (free).
2. **Find clips.** AI reads the transcript and suggests the best moments, with the reason for each one. The ones most likely to hook viewers and keep them watching come first as Top picks, and each clip starts on its first real line. You approve, trim and title them.
3. **Frame in 9:16.** Each clip is framed on your PC, following faces and whoever is speaking.
4. **Edit.** Captions in nine styles, silence removal, punch-in zooms, an opening title, music ducked under the voice, your watermark and credit line: all free and without AI. Or ask for an AI edit plan that adds graphics, titles, sound effects and stock B-roll, and change things in plain words.
5. **Export** finished clips with their caption files, covers and post text for TikTok, YouTube Shorts and Instagram Reels (title, caption and hashtags, written to each platform's rules), ready to post.

## Requirements

- Windows 10 or 11, 64-bit.
- About 600 MB of disk space for the app, plus room for your projects.
- Optional: your own API keys. Anthropic for AI clip finding, edit plans and post text, Deepgram for fast transcription, Pexels or Pixabay for stock B-roll. Every paid step has a free option that runs on your PC, and Vidona shows the cost before anything paid runs.

## Installing

1. Download `Vidona-Setup-<version>.exe` from [Releases](https://github.com/sufyanahmadkamboh/vidona-release/releases/latest) and run it.
2. By default it installs for your Windows user only (no administrator rights needed); the installer also offers to install it for everyone on the PC. It adds Start menu and desktop shortcuts.

This early version is signed with a test certificate, not a commercial one. Windows SmartScreen may therefore show "Windows protected your PC" or "Unknown publisher". If you trust this download, choose **More info** and then **Run anyway**. Each release lists the installer's SHA-256 checksum, so you can check the file you downloaded:

```powershell
Get-FileHash .\Vidona-Setup-0.3.0.exe -Algorithm SHA256
```

To update, download the newest installer and run it. Your projects and settings are kept.

## Privacy

- Your videos stay on your PC.
- If you choose Deepgram, the video's sound is sent to Deepgram to be transcribed. With Whisper on your PC, nothing leaves your computer.
- AI steps send text, only when you ask for them: the transcript for clip finding, and a clip's words for edit plans, post text and Ask AI, to the AI service you choose. Stock B-roll searches send a few keywords to Pexels or Pixabay.
- API keys are encrypted by Windows on your PC, never shown again and never written to logs.
- Crash records stay on your PC. Nothing is uploaded automatically.

---

Copyright © 2026 Sufyan Ahmad. All rights reserved.
