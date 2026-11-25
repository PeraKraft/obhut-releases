# Obhut - Secure Notepad

### Your thoughts, encrypted.

Obhut is a privacy-focused desktop notes app for ideas, personal writing, and technical notes. Organize your documents into encrypted vaults, write with live Markdown styling or rich-text formatting, and create password-protected copies for sharing.

Your notes stay on your machine. No account, subscription, or internet connection is required for everyday use.

## Features

- Encrypted vaults with folders and multiple document tabs
- AES-256-GCM encryption and Argon2id password-based key derivation
- Live Markdown styling, code blocks, and interactive checklists
- Rich-text formatting and encrypted autosave
- PIN-based inactivity locking
- Separately password-protected exports for sharing

## Download

| Platform | Download | Verification |
|---|---|---|
| macOS — Apple Silicon | [Download Obhut 0.1.0](macos/Obhut-0.1.0-macos-arm64.zip) | [SHA-256 checksum](macos/Obhut-0.1.0-macos-arm64.zip.sha256) |

Intel Mac, Windows, and Linux builds are not currently provided.

## Install on macOS

1. Download and extract the ZIP.
2. Drag **Obhut.app** into **Applications**.
3. Open Obhut and follow the setup instructions.

**Test-release notice:** This build is ad-hoc signed, not Apple Developer ID signed or notarized. macOS may block its first launch. If you trust the download, use the per-app **Open Anyway** option under **System Settings → Privacy & Security**. Do not disable Gatekeeper globally.

### Verify the download

Download both files into the same folder, then run:

    shasum -a 256 -c Obhut-0.1.0-macos-arm64.zip.sha256

The result should report `OK`. This checks that the ZIP matches the published checksum; it does not establish Apple publisher trust.

## Before storing important notes

Obhut is under active development. Test with disposable notes first and keep independent backups of your entire vault folder. Forgotten encryption passwords cannot be recovered.

Encryption protects stored notes, but cannot guarantee protection against malware controlling your device. Clipboard history and operating-system memory handling also have limitations.