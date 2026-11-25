---
title: QrTransfer
---

# QrTransfer

Send a file from your Mac to your iPhone with a stream of QR codes. Once both apps are installed, all you need for the transfer is your Mac’s display and your iPhone’s camera.

[Get the source and build instructions](https://github.com/QrTransfer/QrTransfer#build-from-source)

## What you’ll need

- **QrSender** on a Mac running macOS 13 or later.
- **QrReceiver** on an iPhone running iOS 16 or later. Build and install it from Xcode using the instructions above.

## Send a file

1. Open or drop a small file into QrSender and click **Play**.
2. Open QrReceiver, allow camera access, and point the iPhone at the Mac screen.
3. When the file is verified, choose where to save or open it in the iOS share sheet.

QrReceiver automatically detects the sender’s **Mono** and **Color ×3** modes. Color mode puts up to three QR payloads on screen at once. If scanning stalls, switch to **Mono**, lower the playback rate, or reduce the block size.

## How it works

The QRT2 protocol uses fountain coding so later QR codes can help recover missed data. The receiver verifies the finished file with SHA-256. Use matching QRT2 versions of both apps.

[Read the protocol details](https://github.com/QrTransfer/QrTransfer/blob/main/QrSender/README.md#protocol-v2-lt-fountain-code) · [Report an issue](https://github.com/QrTransfer/QrTransfer/issues)
