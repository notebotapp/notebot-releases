<p align="center">
  <img src="https://notebotapp.com/assets/icon-512.png" width="112" alt="">
</p>

<h1 align="center">Notebot</h1>

<p align="center">
  Lecture slides, recordings and photos of the board —<br>
  turned into one study note you can actually use.
</p>

<p align="center">
  <a href="https://github.com/giobachour/notebot-releases/releases/latest"><img alt="Latest release" src="https://img.shields.io/github/v/release/giobachour/notebot-releases?label=latest&color=141414&labelColor=141414&style=flat-square"></a>
  <img alt="macOS 12 or newer" src="https://img.shields.io/badge/macOS-12%2B-141414?style=flat-square">
  <img alt="Windows 10 and 11" src="https://img.shields.io/badge/Windows-10%20%26%2011-141414?style=flat-square">
  <a href="https://notebotapp.com"><img alt="notebotapp.com" src="https://img.shields.io/badge/notebotapp.com-f6f1eb?style=flat-square&labelColor=f6f1eb&color=141414"></a>
</p>

<p align="center">
  <b><a href="https://github.com/giobachour/notebot-releases/releases/latest">Download the latest release →</a></b>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://notebotapp.com/assets/shots/home-dark-hero.webp">
    <img src="https://notebotapp.com/assets/shots/home-light-hero.webp" width="820" alt="Notebot's home screen: a greeting, course chips, recent notes as pastel cards, and the week's study time">
  </picture>
</p>

---

This repository holds the **installers**. Every download here is built and signed by the author; the app's source code is kept in a private repository.

Notebot is free while it is in beta.

## Download

| | Requirements | File |
|---|---|---|
| **macOS** | Apple silicon (M1 or later), macOS 12 or newer | `Notebot-x.y.z.dmg` — about 380 MB |
| **Windows** | Windows 10 or 11, 64-bit | `Notebot-Setup-x.y.z.exe` — about 245 MB |

Both files are on the **[latest release page](https://github.com/giobachour/notebot-releases/releases/latest)**. There is no Intel-Mac build.

### Installing on macOS

1. Open the `.dmg` and drag **Notebot** into **Applications**.
2. The first launch shows *“Notebot cannot be opened because Apple cannot check it for malicious software.”* That is macOS noticing an app that was not bought from the App Store, not a problem with the download.
3. Close the message, open **System Settings → Privacy & Security**, scroll down and press **Open Anyway**. Confirm once.

This is needed only for the first install. Updates from inside the app never ask again.

### Installing on Windows

1. Run the `Notebot-Setup` file. It installs for your user only, so Windows never asks for an administrator password.
2. Windows may show *“Windows protected your PC.”* That is SmartScreen noticing an installer without a company certificate. Press **More info**, then **Run anyway**.
3. Notebot lands in your Start menu, with an optional desktop shortcut.

To remove it later: **Settings → Apps → Notebot → Uninstall**. Your notes folder is never touched.

## First run

Notebot asks four things, once:

- **Sign in with Google.** Notebot is in beta with a small group, so signing in is how we know who is testing it. See [what is recorded](https://notebotapp.com/privacy).
- **Your name**, for the app to greet you by.
- **A folder for your notes.** Any folder. One inside iCloud Drive or OneDrive puts your notes on your phone too.
- **A Gemini key**, free from Google AI Studio. The setup has a button that opens the page, and tests the key for you before continuing.

There is also an optional download of the transcription model (about 150 MB), used when you add a lecture recording. You can skip it; it downloads the first time you need it.

A welcome note opens on the first launch and explains the rest inside the app.

## What it does

<table>
<tr>
<td width="50%">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://notebotapp.com/assets/shots/note-dark.webp">
  <img src="https://notebotapp.com/assets/shots/note-light.webp" alt="A generated study note with headings, callouts and maths">
</picture>
</td>
<td width="50%"><img src="https://notebotapp.com/assets/shots/drill-card.webp" alt="A drill card with a question and a hidden answer"></td>
</tr>
</table>

- **Drop a lecture in, get one note.** Slides as PDF or PowerPoint, an audio recording, photos of the whiteboard, scans of handwritten pages, your own typed notes — any mix, for one lecture. Notebot writes a single explained note, not a transcript.
- **Read and study it in the app.** Rendered Markdown with maths and diagrams, a live outline, full-text search across the vault, an exam lens, and drill cards built from the note's own questions.
- **Recordings stay on your computer.** They are transcribed locally before anything is sent to Google.
- **Your notes are plain Markdown files** in the folder you chose. Obsidian and any other Markdown app read the same folder.

More, with pictures, at **[notebotapp.com](https://notebotapp.com)**.

## Updates

Notebot checks this page for a newer version about once a day. When there is one, a line appears at the top of the window: **What's new** shows the release notes, **Update** installs it and reopens the app.

Every release since 1.0.7 ships a `.sig` file next to the installer — an Ed25519 signature over the exact file. Notebot verifies it before installing anything, and refuses a download that does not match. That is why in-app updates are the safest way to upgrade.

## Your notes and your key

- Notes, recordings and figures are **never uploaded** to us. They live in your folder.
- Your Gemini key stays on your computer and is used only to talk to Google's API.
- The beta sign-in records your name, email address, which version you run and the day you last opened it. Nothing else. The [privacy page](https://notebotapp.com/privacy) is the full list, and says how to have it deleted.

## Something wrong?

[Open an issue](https://github.com/giobachour/notebot-releases/issues) with what you were doing and, if a run failed, the text under **Show details** in the panel. If you are in the beta group, a message works too.

<p align="center">
  <sub>Made by Giorgio Bachour, a student who needed it.</sub>
</p>
