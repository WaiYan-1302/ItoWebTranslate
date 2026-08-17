# Live Translation Overlay

A free, browser-based Japanese-and-English live subtitle overlay for presentations.
It uses Chrome speech recognition, Chrome's built-in Translator API, and Document
Picture-in-Picture to place an always-on-top subtitle window over Canva or
another presentation.

## Features

- Japanese → English translation
- English → Japanese translation
- Adjustable black-window opacity
- Adjustable font size, family, and color
- Adjustable overlay-window width and height
- Default appearance: white font on a black window

## Requirements

- Current **desktop Google Chrome** on Windows, macOS, or Linux
- Internet connection for speech recognition and the first language-pack download
- Microphone permission
- HTTPS hosting, such as GitHub Pages

Android Chrome is not supported by Chrome's built-in Translator API.

## Publish on GitHub Pages

1. Create a new **public** GitHub repository.
2. Upload `index.html` and this `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Choose the `main` branch and `/ (root)`, then save.
6. Wait a few minutes and open the published GitHub Pages URL in desktop Chrome.

No build command, dependency installation, API key, or server is required.

## Use

1. Select **Japanese → English** or **English → Japanese**.
2. Adjust opacity, font, font color, font size, and requested window size.
3. Click **Prepare translation** and wait until the selected model is ready.
4. Click **Open floating overlay**.
5. Drag the floating subtitle window to the bottom of the screen.
6. Click **Start listening** and allow microphone access.
7. Open Canva in another tab or window and start the presentation.
8. Speak the selected source language in short sentences with natural pauses.

Appearance settings update the open overlay immediately. After entering a new
width or height, click **Apply size**. Chrome may limit extremely large or small
Picture-in-Picture window sizes.

Keep the control page open. Closing it also closes the floating overlay.

## Processing and privacy

- Japanese-to-English translation runs locally through Chrome's downloaded
  Translator language pack.
- Chrome speech recognition may send microphone audio to an online recognition
  service.
- GitHub Pages only hosts the static website files.

## Troubleshooting

### Translator or overlay says unavailable

Update desktop Google Chrome at `chrome://settings/help`, restart Chrome, and
open the hosted HTTPS page again.

### Microphone denied

Click the site-information icon beside the address bar, allow **Microphone**,
reload, and repeat the three setup steps.

### Overlay closes

The control page must remain open. Open Canva in a separate tab or window.

### Captions are delayed

Pause briefly after each sentence. Final translation begins when speech
recognition marks a phrase as complete.
