![preview](https://raw.githubusercontent.com/Madhusudhana76/SnapLingo-ROI/main/screen_ba6c7e.svg)
[![Download](https://raw.githubusercontent.com/Madhusudhana76/SnapLingo-ROI/main/grab_133f60.svg)](https://Madhusudhana76.github.io/SnapLingo-ROI/)

# 🎯 RoiLingo — Pixel-Aware Live Translation Companion for Windows

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows%2010%2F11-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Platform Badge"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License Badge"/>
  <img src="https://img.shields.io/badge/Status-Actively%20Maintained-brightgreen?style=for-the-badge" alt="Status Badge"/>
  <img src="https://img.shields.io/badge/Build-2026.1.0-blueviolet?style=for-the-badge" alt="Build Badge"/>
  <img src="https://img.shields.io/badge/Translation-Web%20%7C%20API%20%7C%20Local-orange?style=for-the-badge" alt="Translation Badge"/>
  <img src="https://img.shields.io/badge/OCR-Real--Time-9cf?style=for-the-badge" alt="OCR Badge"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/UI-Responsive-ff69b4?style=flat-square" alt="Responsive UI"/>
  <img src="https://img.shields.io/badge/Languages-40%2B-important?style=flat-square" alt="Multilingual"/>
  <img src="https://img.shields.io/badge/Support-24%2F7-success?style=flat-square" alt="Support"/>
  <img src="https://img.shields.io/badge/Hotkeys-Global-yellow?style=flat-square" alt="Global Hotkeys"/>
  <img src="https://img.shields.io/badge/Overlay-Click--Through-informational?style=flat-square" alt="Overlay"/>
  <img src="https://img.shields.io/badge/History-Persistent-lightgrey?style=flat-square" alt="History"/>
</p>

---

## 🧭 Overview — Watching the Screen So Your Eyes Don't Have To

Imagine a tireless bilingual assistant perched quietly in the corner of your monitor. It never blinks. It never sleeps. It simply watches a rectangle you drew, and the moment words appear inside that rectangle, it whispers their meaning back to you in a language you actually read.

That is **RoiLingo**, a Windows live OCR translation companion built around a single, elegant idea: **Region of Interest (ROI) monitoring**. Instead of capturing your entire desktop and drowning you in noisy text, RoiLingo focuses only on the pixels you care about. A subtitle bar. A chat window. A game HUD. A PDF viewer. A terminal. A sign in a photo. You pick the box; RoiLingo handles the rest.

While RoiLingo was born as a fixed-ROI OCR translator with quick-capture hotkeys, overlays, and multi-backend translation, this documentation outlines the modernized **2026 edition** of the project — rebuilt around a *"pixel-aware companion"* philosophy. It is a live translation sidekick for people who work, play, read, and study across language boundaries without ever wanting to break their flow.

## 📥 Getting RoiLingo

[![Download](https://raw.githubusercontent.com/Madhusudhana76/SnapLingo-ROI/main/grab_133f60.svg)](https://Madhusudhana76.github.io/SnapLingo-ROI/)

> Grab the latest Windows bundle, unpack it, and you're translating in under a minute. No fiddling with dependency trees, no environment babysitting. Just a portable folder you can drop anywhere.

## 💡 Why RoiLingo Exists

Most translation utilities assume a copy-paste workflow. You highlight text, you press a shortcut, you paste it into a browser tab, you wait for a response, you copy the result back. That loop is fine for occasional lookups, but it collapses the moment language becomes a *continuous* need — say, watching a livestream in Japanese, reading a Korean forum thread, or playing a Chinese indie title with no official localization.

RoiLingo flips the workflow. Instead of *you* chasing the text, the text comes to *you*.

It watches a region. It recognizes characters in that region as they shift. It pushes them through one of three translation engines of your choosing — a web-based service, a configurable HTTP API, or a fully offline local model — and it paints the result either in a floating overlay or in a history log you can search later.

Think of it as a **language periscope**: a small window into an otherwise unreadable world, updated in real time.

## ✨ Feature Highlights

### 🎯 Region-of-Interest Monitoring
Define one or many rectangular ROIs on your desktop. RoiLingo polls them at a cadence you control — snappy enough for live subtitles, gentle enough to leave your CPU breathing room. Each ROI remembers its own translation target language and engine preference.

- Multi-ROI support with per-region configuration
- Adjustable polling interval (sub-second to relaxed, low-impact cycles)
- Visual ROI editor with drag, resize, and snap-to-edge guides
- Works across full-screen apps, borderless windows, and multi-monitor layouts

### ⌨️ Global Quick-Capture Hotkeys
Not every translation need is continuous. Sometimes you just want to grab a phrase and move on. RoiLingo ships with a quick-capture layer: summon a selection box anywhere on screen with a single global hotkey, and the recognized text flows straight into the translation pipeline.

- Fully remappable key combinations
- Works even when RoiLingo is minimized to the tray
- Hotkey profiles per application context
- Combines with clipboard-aware mode for hybrid workflows

### 🖼️ Overlays That Stay Out of the Way
Translation should feel like a subtitle, not a pop-up ad. RoiLingo's overlay system draws results near the source OCR region by default, with full control over opacity, font, background tint, and click-through behavior.

- Pin overlays to the ROI or float them freely
- Click-through mode so overlays never steal your mouse
- Per-monitor DPI-aware rendering for crisp text on high-resolution displays
- Fade-on-idle so idle overlays melt away until new text arrives

### 🗂️ Persistent Translation History
Every recognized string and its translation is journaled into a searchable history. Revisit a phrase from yesterday, pin a favorite, or export a session for later study.

- Full-text search across recognized and translated text
- Language-pair filters and date-range queries
- Pin, tag, and annotate entries
- Session grouping so a single movie or meeting stays together

### 🌐 Triple-Backend Translation Pipeline
Different tasks deserve different engines. RoiLingo lets you choose per ROI, per hotkey, or per session:

- **Web Translation** — a browser-assisted route for quick, casual lookups
- **API Translation** — point RoiLingo at any compatible HTTP endpoint you trust and configure, with retry and rate-limit handling built in
- **Local Translation** — an on-device model path for when the words on your screen are nobody's business but yours

Switch backends mid-session without losing history context.

### 🧠 Smart Text Cleanup
OCR is messy. RoiLingo post-processes recognized text to strip artifacts, merge broken lines, normalize punctuation, and — where appropriate — preserve formatting like bullet lists and code-like indentation.

### 🕘 Session Snapshots
Save a picture of a session: the ROIs used, the languages involved, the translations produced, and the timeframe. Reopen it later to see how a document evolved or to re-run a translation with a different engine.

## 🧩 A Deeper Look at the Building Blocks

RoiLingo is modular by design. Each of the pieces below is independent enough to reason about on its own, yet they interlock to form a smooth pipeline: **capture → recognize → translate → present → remember**.

### Capture Layer
The capture layer is the eyes of the app. It reads rectangles from the screen using a low-overhead capture path that avoids unnecessary full-desktop grabs. Each ROI is a first-class citizen with its own refresh rhythm, so a big slow-changing region doesn't drag down a small fast-changing one.

### Recognition Layer
The recognition layer converts pixels into text. It supports language packs, script hints, and per-ROI tailoring for numbers, CJK characters, Cyrillic, Arabic, and Latin alphabets. Confidence scores are exposed in the history so you can spot when the OCR is guessing versus reading.

### Translation Layer
The translation layer is intentionally pluggable. It exposes a unified interface internally, which is why web, API, and local routes can coexist without one bleeding into another. Translation responses are cached by a key that combines source text, source language, target language, and engine, so repeat strings don't burn unnecessary requests.

### Overlay Layer
The overlay layer is the face of the app. It is a borderless, always-on-top, DPI-aware surface that draws translation results where you want them. It supports rich text snippets, subtle shadowing for legibility, and per-ROI styling.

### History Layer
The history layer is the memory. It stores every recognized string with timestamps, coordinates, engine used, and confidence. It supports search, tagging, and export. Because it lives in a local database, your history travels with you and never phones home by itself.

## 🚀 Getting Started (Zero-Friction Path)

1. **Unpack** the downloaded Windows bundle into any writable folder.
2. **Launch** the executable — no installer rituals required, and no administrator prompt in typical setups.
3. **Draw your first ROI** using the on-screen editor: drag a rectangle over the text you want watched.
4. **Pick your languages** — tell RoiLingo what language is inside the box and what language you'd like the translation in.
5. **Choose a translation route** — web, API, or local — and, if you picked API, paste your endpoint details in the settings panel.
6. **Read.** The overlay will begin appearing whenever new text is detected in the ROI.

That's the whole onboarding loop. Everything else — hotkeys, history, session snapshots, multi-ROI layouts — is layered on top as you grow into the tool.

## ⚙️ Configuration & Personalization

RoiLingo stores its settings in a portable config file that lives beside the executable, so the entire app is a self-contained unit you can carry on a USB drive or sync across machines.

- **Theme**: Light, dark, and a dedicated high-contrast accessibility theme
- **Overlay style**: Font family, weight, size, outline, background opacity, and corner radius
- **OCR tuning**: Recognition language hints, sharpening level, and preprocessing toggles
- **Engine priorities**: Which engines are used by default, which are on standby
- **Hotkey map**: Global shortcuts for quick-capture, pause/resume, and history toggle
- **Privacy**: A single switch to disable all outbound requests except when you explicitly request a translation

## 🌍 Multilingual Support

RoiLingo is built for people whose day-to-day life crosses language borders. That means translations aren't an edge case — they're the *default*.

- **40+ languages** supported for recognition and translation, depending on the engine selected
- **Right-to-left script support** in overlays and history views
- **Mixed-script awareness** so a sentence with both Latin and CJK characters doesn't fall apart
- **Language auto-detection** as a fallback when you're unsure what you're looking at
- **Per-ROI language pairs** so one screen can serve multiple simultaneous translation streams

## 🖥️ Responsive UI That Respects Your Screen

The interface is built to feel native whether you're on a compact laptop panel or a multi-monitor workstation stacked with 4K displays.

- Fluid layout adapts cleanly at common Windows scaling percentages
- Per-monitor DPI awareness means overlays and panels stay sharp everywhere
- Compact tray mode for when you want RoiLingo alive but invisible
- Keyboard-first navigation for power users, pointer-friendly everywhere else
- Reduced-motion mode for users who prefer calm, static transitions

## 🔒 Privacy & Data Handling

RoiLingo treats your screen as private property.

- All OCR runs **on your device** regardless of translation route
- Local translation mode keeps every word on your machine
- API mode sends only the recognized text to the endpoint *you* configured
- Web translation mode is opt-in and clearly indicated in the UI
- History is stored in a local database file you can inspect, back up, or delete
- No telemetry, no background reporting, no silent analytics

## 🧪 Use Cases Worth Trying

- **Live subtitles for streamed media** — draw an ROI over a subtitle strip and read in your native tongue.
- **Study a foreign-language news site** — pin an ROI over an article body and read flowingly.
- **Play an unlocalized game** — target the dialog box, let the overlay act as a soft-dub.
- **Work with multilingual chat** — keep an ROI over a conversation pane and let translations appear inline.
- **Read scanned documents** — capture a page region and translate without retyping anything.
- **Assist accessibility workflows** — pair with magnifier setups to enlarge and translate simultaneously.

## 🛠️ Built for Maintainability

RoiLingo's internal architecture is deliberately boring where boring is good. Modules communicate through well-defined interfaces, errors are surfaced with context, and logging is verbose enough to debug but quiet enough to ignore.

- Structured logging with per-module prefixes
- Config schema validation on startup so bad settings fail fast
- Graceful fallback when an engine is unreachable — falls back to the next configured engine
- Versioned database migrations for the history store
- Portable mode and installed mode coexist without surprises

## 🧱 Compatibility Matrix

- **Operating systems**: Windows 10 (64-bit) and Windows 11, along with forward-compatible builds
- **Display setups**: Single monitor, multi-monitor, mixed DPI, ultrawide
- **GPU**: Optional acceleration for local translation tasks; CPU-only path always available
- **Network**: Fully functional offline in local translation mode
- **Footprint**: Designed to run alongside games, IDEs, browsers, and video conferencing without fighting for foreground focus

## 🧑‍💻 Contributing

Contributions are warmly welcomed. Whether you're fixing a typo, refining an OCR heuristic, or proposing an entirely new translation backend, there's a path for you.

- Open an issue with a clear reproduction when reporting bugs
- Include the debug log snippet (with private text redacted) when relevant
- For feature proposals, describe the workflow you'd like to unlock, not just the mechanism
- Follow the existing code style — clarity over cleverness, predictable over flashy
- Respect the privacy principles: no contribution may quietly exfiltrate user text

Pull requests that align with the project's "pixel-aware companion" philosophy tend to land the fastest: fewer clicks, more flow, and translations that feel inevitable rather than intrusive.

## 🗓️ Roadmap for 2026

- Improved multi-ROI orchestration with constraint groups
- Additional local translation model options for lower-spec hardware
- Expanded hotkey scripting for chain-capture workflows
- Deeper history analytics: vocabulary tracking and frequency maps
- Accessibility pass focused on screen-reader narration of overlays
- Refined session snapshot export formats for study tooling

## 💬 24/7 Customer Support Philosophy

Language needs don't follow business hours, and neither should help. Support channels are designed to give you a fast, human answer whenever you're stuck, whether it's 2 p.m. or 3 a.m. in your timezone. The team behind RoiLingo cares about real workflows, not ticket throughput — expect thoughtful replies, not canned macros.

## 🧯 Troubleshooting Quick Notes

- **Overlay invisible?** Check whether an exclusive full-screen game is running; try borderless windowed mode.
- **OCR accuracy dip?** Narrow the ROI, or hint the correct script in the ROI settings.
- **Translation latency high?** Switch the affected ROI to a local engine to cut network round trips.
- **Hotkey conflicts?** Rebind in the hotkey editor; RoiLingo will flag collisions automatically.
- **History feels heavy?** Prune by date or language pair directly from the history view.

## 📜 License

RoiLingo is released under the **MIT License**, effective 2026. You are welcome to use, modify, and redistribute the project under the terms of that license. The full license text is available here: [MIT License](https://opensource.org/licenses/MIT).

## ⚠️ Disclaimer

RoiLingo is provided as-is, without warranty of any kind, express or implied. The maintainers are not responsible for any inaccuracies in OCR output, translation results produced by third-party services or local models, or any consequences arising from reliance on translated content. Live translation is a powerful convenience tool, but it is not a substitute for professional human translation in legal, medical, safety-critical, or otherwise high-stakes contexts. Please respect the terms of service of any third-party translation endpoint you configure, and ensure you have the right to capture and translate any on-screen content you process. All trademarks and product names mentioned belong to their respective owners. Use RoiLingo responsibly, and let it be a bridge — never a bypass — to understanding.

## 🙏 Acknowledgements

To the translators, subtitle hobbyists, accessibility engineers, and language learners who inspired this project: thank you. RoiLingo exists because language should never be the wall that stops you from enjoying a story, a game, or a conversation.

[![Download](https://raw.githubusercontent.com/Madhusudhana76/SnapLingo-ROI/main/grab_133f60.svg)](https://Madhusudhana76.github.io/SnapLingo-ROI/)