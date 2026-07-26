<p align="center">
  <img src="https://raw.githubusercontent.com/AlteredAJ/dualsense-haptics/release-free/src-tauri/icons/128x128.png" width="80" alt="logo">
</p>

<h1 align="center">AJ</h1>

<p align="center"><strong>Systems & haptics engineer. Rust, Tauri, DSP, game telemetry.</strong></p>

<p align="center">
  <a href="https://buymeacoffee.com/alt3red"><img src="https://img.shields.io/badge/Buy_Me_a_Coffee-Support-ffdd00?style=flat-square&logo=buymeacoffee&logoColor=black" alt="bmc"></a>
  <a href="https://alt3red.gumroad.com/l/universal-dualsense-haptics"><img src="https://img.shields.io/badge/Gumroad-%244-ff90e8?style=flat-square&logo=gumroad&logoColor=white" alt="gumroad"></a>
  <a href="https://alteredaj.github.io/dualsense-haptics/"><img src="https://img.shields.io/badge/Website-Landing_Page-4fc3ff?style=flat-square" alt="website"></a>
  <a href="https://www.linkedin.com/in/ajapaukese"><img src="https://img.shields.io/badge/LinkedIn-Connect-0a66c2?style=flat-square&logo=linkedin" alt="linkedin"></a>
  <img src="https://komarev.com/ghpvc/?username=AlteredAJ&style=flat-square&color=4fc3ff" alt="views">
</p>

---

### About

I build software that connects hardware to games. Currently shipping **[Universal DualSense Haptics](https://github.com/AlteredAJ/dualsense-haptics)** — a Windows desktop app that turns the PS5 DualSense into a full haptic peripheral, driving adaptive triggers and voice-coil rumble from real game telemetry at 60fps.

- **Rust + Tauri 2** — haptics engine, HID output, telemetry parsers
- **DSP** — low-pass filters, EWMA envelopes, Pacejka tire models, slip crossover
- **UDP telemetry** — Forza Data Out, F1 23, Assetto Corsa
- **TCP bridges** — Minecraft Fabric mod, custom JSON protocol
- **License infra** — Cloudflare Workers, Gumroad API, beta key minting
- **UI** — vanilla HTML/CSS/JS, glass-morphism design system, Manrope variable font

---

### Projects

#### [Universal DualSense Haptics](https://github.com/AlteredAJ/dualsense-haptics)

Desktop app that drives DualSense adaptive triggers, voice-coil rumble, and lightbar from real game data.

<table>
<tr>
<td width="50%">

- **Six haptic profiles** — Racing, Gun, Melee, Audio Reactive, Minecraft, Static
- **Telemetry-driven** — Forza Horizon/Motorsport, F1 23, Assetto Corsa via UDP
- **Minecraft mod** — Fabric bridge over TCP, per-item feels and lightbar colors
- **Virtual Xbox pad** — ViGEmBus XInput passthrough with HidHide cloaking
- **60fps haptic loop** — custom DSP pipeline in Rust
- **The Lab** — live preview, per-weapon tuning sliders, Racing Lab curves

</td>
<td width="50%">

| Key Metrics | |
|---|---|
| Language | Rust, JS, CSS |
| License | MIT (free) / Proprietary (paid) |
| Platform | Windows 10/11 x64 |
| Engine | Tauri 2 + hidapi + ViGEmBus |
| Pricing | Free (static) · $4 Full Immersion |
| Site | [alteredaj.github.io/dualsense-haptics](https://alteredaj.github.io/dualsense-haptics/) |
| Gumroad | [alt3red.gumroad.com](https://alt3red.gumroad.com/l/universal-dualsense-haptics) |

</td>
</tr></table>

<p align="center">
  <a href="https://github.com/AlteredAJ/dualsense-haptics/releases"><img src="https://img.shields.io/badge/⬇_Download_Free-2ea043?style=for-the-badge" alt="free"></a>
  <a href="https://alt3red.gumroad.com/l/universal-dualsense-haptics"><img src="https://img.shields.io/badge/🔓_Full_Immersion_$4-4fc3ff?style=for-the-badge" alt="paid"></a>
  <a href="https://buymeacoffee.com/alt3red"><img src="https://img.shields.io/badge/☕_Buy_Me_a_Coffee-ffdd00?style=for-the-badge&logo=buymeacoffee&logoColor=black" alt="bmc"></a>
</p>

<br>

#### [DesktopConsole](https://github.com/AlteredAJ/DesktopConsole)

A controller-first, 10-foot Windows couch launcher. Pick up a DualSense, triple-tap PS — your full-screen console appears.

<table>
<tr>
<td width="50%">

- **Controller-first navigation** — D-pad, stick, touchpad gestures. Cross select, Circle back
- **DualSense integration** — Haptics, lightbar sync, battery meter, trackpad-as-mouse
- **GPU fluid backgrounds** — Live WebGL simulations, three presets, zero-cost rendering
- **Glass UI** — Frosted glass, specular bloom, accent-glow focus indicators
- **Quick Menu overlay** — Double-tap PS mid-game for volume, RGB, capture
- **OpenRGB control** — Cycle and set RGB scenes on lightbar and motherboard LEDs

</td>
<td width="50%">

| Key Metrics | |
|---|---|
| Language | Rust, TypeScript, CSS |
| License | MIT |
| Platform | Windows 11 x64 |
| Engine | Tauri 2 + React 19 + Vite 5 |
| Site | [alteredaj.github.io/DesktopConsole](https://alteredaj.github.io/DesktopConsole/) |

</td>
</tr></table>

<p align="center">
  <a href="https://github.com/AlteredAJ/DesktopConsole"><img src="https://img.shields.io/badge/View_on_GitHub-5b9cf5?style=for-the-badge&logo=github" alt="github"></a>
  <a href="https://alteredaj.github.io/DesktopConsole/"><img src="https://img.shields.io/badge/Landing_Page-111?style=for-the-badge" alt="site"></a>
</p>

<br>

#### [Simple Jarvis](https://github.com/AlteredAJ/SimpleJarvis)

Personal conversational AI. Speak, interrupt mid-sentence, and get answers grounded in your own Obsidian vault.

<table>
<tr>
<td width="50%">

- **Voice-first loop** — continuous dialogue with hard/soft barge-in and grace-window follow-ups
- **Neural wake word + VAD** — openWakeWord `hey jarvis` + Silero VAD, no ambient false positives
- **Live transcript HUD** — radial waveform, both sides streaming, interruption markers
- **Obsidian grounding** — keyword RAG that follows `[[wikilinks]]`, no vector DB
- **Local TTS** — Kokoro-82M, 54 voices at 3.4× realtime, ElevenLabs fallback
- **Brain routing** — cheap model for chat, frontier model for hard analysis, local for time/date

</td>
<td width="50%">

| Key Metrics | |
|---|---|
| Language | Python 3.12 / 3.14 |
| License | MIT |
| Platform | Windows 11 |
| TTS | Kokoro-82M · ElevenLabs |
| Brain | DeepSeek · Claude |
| Cost | $0 per query on the local path |

</td>
</tr></table>

<p align="center">
  <a href="https://github.com/AlteredAJ/SimpleJarvis"><img src="https://img.shields.io/badge/View_on_GitHub-5b9cf5?style=for-the-badge&logo=github" alt="github"></a>
</p>

---

### Stack

<p align="center">
  <img src="https://img.shields.io/badge/Rust-dea584?style=for-the-badge&logo=rust&logoColor=white" alt="rust">
  <img src="https://img.shields.io/badge/Tauri_2-ffc131?style=for-the-badge&logo=tauri&logoColor=black" alt="tauri">
  <img src="https://img.shields.io/badge/TypeScript-3178c6?style=for-the-badge&logo=typescript&logoColor=white" alt="ts">
  <img src="https://img.shields.io/badge/Python-3776ab?style=for-the-badge&logo=python&logoColor=white" alt="python">
  <img src="https://img.shields.io/badge/CSS-glass_UI-4fc3ff?style=for-the-badge" alt="css">
  <img src="https://img.shields.io/badge/Cloudflare_Workers-f38020?style=for-the-badge&logo=cloudflare&logoColor=white" alt="cloudflare">
  <img src="https://img.shields.io/badge/HID-hidapi-333?style=for-the-badge" alt="hid">
</p>

---

<p align="center">
  <sub>
    <a href="https://github.com/AlteredAJ">github</a> ·
    <a href="https://alt3red.gumroad.com/l/universal-dualsense-haptics">gumroad</a> ·
    <a href="https://buymeacoffee.com/alt3red">buy me a coffee</a> ·
    <a href="https://alteredaj.github.io/dualsense-haptics/">landing page</a>
  </sub>
</p>
