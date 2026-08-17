# Live Translation Overlay

A free, browser-based Japanese-to-English live subtitle overlay for presentations.
It uses Chrome speech recognition, Chrome's built-in Translator API, and Document
Picture-in-Picture to place an always-on-top subtitle window over Canva or
another presentation.

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

1. Click **Prepare translation** and wait until the Japanese-to-English model is ready.
2. Click **Open floating overlay**.
3. Drag the floating subtitle window to the bottom of the screen.
4. Click **Start listening** and allow microphone access.
5. Open Canva in another tab or window and start the presentation.
6. Speak Japanese in short sentences with natural pauses.

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
