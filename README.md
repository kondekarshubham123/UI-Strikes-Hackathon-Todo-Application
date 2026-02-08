# 📝 UI Strikes Tambo Hackathon | Todo Application

<p align="center"><i>A fast and modern Todo app built with React, featuring task sharing via link, P2P Task Sync with WebRTC, theme customization, offline usage as a PWA, and caching for smooth performance.</i></p>

## [https://kondekarshubham123.github.io/UI-Strikes-Hackathon-Todo-Application/](https://kondekarshubham123.github.io/UI-Strikes-Hackathon-Todo-Application/)

<ul style="display: flex; flex-direction: column; gap:10px;">
  <li style="vertical-align: middle;">
    <img src="https://go-skill-icons.vercel.app/api/icons?i=react" alt="react" width="24" style="vertical-align: middle; margin-right: 4px;" /> React
  </li>
    <li style="vertical-align: middle;">
    <img src="https://go-skill-icons.vercel.app/api/icons?i=typescript" alt="typescript" width="20" style="vertical-align: middle;margin-right: 4px;" /> Typescript
  </li>
    <li style="vertical-align: middle;">
    <img src="https://go-skill-icons.vercel.app/api/icons?i=vite" alt="vite" width="24" style="vertical-align: middle;margin-right: 4px;" /> Vite
  </li>
  <li style="vertical-align: middle;">
    <img src="https://go-skill-icons.vercel.app/api/icons?i=vitest" alt="vitest" width="24" style="vertical-align: middle;margin-right: 4px;" /> Vitest
  </li>
  <li style="vertical-align: middle;">
    <img src="https://go-skill-icons.vercel.app/api/icons?i=emotion" alt="emotion" width="24" style="vertical-align: middle;margin-right: 4px;" /> Emotion
  </li>
    <li style="vertical-align: middle;">
    <img src="https://go-skill-icons.vercel.app/api/icons?i=mui" alt="mui" width="24" style="vertical-align: middle;margin-right: 4px;" /> Material UI (MUI)
  </li>
</ul>

## ⚡ Features

### 🔗 Share Tasks by Link or QR Code

Easily share your tasks with others using a link or QR code.

**[Example Link](https://kondekarshubham123.github.io/UI-Strikes-Hackathon-Todo-Application/share?task=N4IgJg9gdgpiBcAzAhgGwM4wDQgA4EspYwEAXAJwFdsQpkBbOeEAdRgCN19SYACAERgA3GKgi5GUUiBxgY6AMbl8uUvmgIQAYXIxkPXsl6pkUMIQDmvXMgt8A7twAWvAEp6FpAHQArdL0QIcl4FVHwYKS9eJ1JSXHR4AHpE+1SvAE8ISlJKdhgvBQh6FP0FJwB+IQBedgBZAGsoRABpAA0ASQAxAEEADgAyUiqAJgBmdH7kdgB9MtNYVCrEXRgtCDktBlwvIIsZEBh6CB98TQBGRABOMDOAWgvRxAVb4YAGV7B7xAAWdnZ9wpiciaADE7AAbMNvohEPswPomCA3sMAKy3V7fF6vAAqrzO8DOl3gr3BXleAHZRgAtOF6MBhWCaZFojEvUa4-FnXrE15k940nAKBEWILpBAAbVA+BIzFew0uwwU7GQaMQ4Jgw1u3zOCkx7BRyHJtwUKMuyFeyGQMAUiBgo32dEYmhYQXq+0Ox1OzAeGoBECBoKhvRgMJAAF8sFKZWdwb1yWdUdryd9waMyaMcI7EWtzFA9jgPSdzogDaqYK9YYL-UFQeCbsNQ2GALo4EzoUgAZWQIiZcpZmLeHPgb3go15oxR1PDQA&userName=Maciej)**


### 🤖 AI Emoji Suggestions

This feature uses Chrome’s experimental `window.LanguageModel` API powered by **Gemini Nano** — an on-device LLM.

⚠️ Requires **Chrome Canary 128+** with the **Gemini Nano model installed** - [Setup guide](https://docs.google.com/document/d/1VG8HIyz361zGduWgNG7R_R8Xkv0OOJ8b5C9QKeCjU0c/view?pli=1&tab=t.0#heading=h.witohboigk0o)

Code: [src/components/EmojiPicker.tsx](https://github.com/kondekarshubham123/UI-Strikes-Hackathon-Todo-Application/blob/main/src/components/EmojiPicker.tsx#L116)

### 🔄 P2P Task Sync with WebRTC

Securely sync all the data between devices using peer-to-peer WebRTC connections. Devices pair via QR code, and your data is transferred directly between them — only minimal server involvement for connection setup, with no data stored or processed in the cloud.

- Tasks and categories are auto-merged based on recent edits or deletions
- For settings and other data, you choose which device to sync from

### 🎨 Color Themes & Dark Mode

Choose from various color themes and toggle between light and dark modes to suit your preferences.

### 🗣️ Task Reading Aloud

Option to have tasks read aloud using the native `SpeechSynthesis` API, with a selection of voices to choose from.

### 📥 Import/Export Tasks

Users can import and export tasks to/from JSON files. This feature allows users to back up their tasks or transfer them to other devices easily. [Example Import File](https://github.com/kondekarshubham123/UI-Strikes-Hackathon-Todo-Application/blob/main/example-import.json)

### 📴 Progressive Web App (PWA)

This app is a Progressive Web App (PWA), which means it can be installed on your device, **used even when you're offline** and behave like a native app with shortcuts and app badges.


### 🔄 Update Prompt

The app features a custom update prompt that notifies users when a new version is available, allowing for easy refresh to access the latest improvements.


### 📱 Custom Splash Screens

The app automatically generates custom splash screens from a single HTML template for various iOS and iPadOS devices in both light and dark modes. These splash screens provide a smooth, native-like launch experience when the app is opened as a PWA.


To generate splash screens:

```bash
npm run generate-splash
```

Code: [scripts/splash-screens](https://github.com/kondekarshubham123/UI-Strikes-Hackathon-Todo-Application/blob/main/scripts/splash-screens)

## 👨‍💻 Installation

To install and run the project locally, follow these steps:

1. Clone the repository:

```bash
git clone https://github.com/kondekarshubham123/UI-Strikes-Hackathon-Todo-Application.git
```

2. Navigate to the project directory:

```bash
cd UI-Strikes-Hackathon-Todo-Application
```

3. Install the dependencies:

```bash
npm install
```

4. Start the development server:

```bash
npm run dev
```

The app will now be running at [http://localhost:5173/](http://localhost:5173/).

> [!TIP]
> For mobile device testing, use `npm run dev:host` to preview the app on your local network with HTTPS (required for camera features) and a QR code in the terminal for quick access. To enable PWA features in development, see [vite.config.ts](vite.config.ts).


## Credits

Made with ❤️ by [kondekarshubham123](https://github.com/kondekarshubham123), licensed under [MIT](https://github.com/kondekarshubham123/UI-Strikes-Hackathon-Todo-Application/blob/main/LICENSE).
