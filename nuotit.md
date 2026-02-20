# Nuotit — Podcast Player

**Version:** 1.26.5 (Latest: December 21, 2025)
**Last Updated:** 2026-01-23
**Platform:** iOS 26.0+ / iPadOS 26.0+

---

## Product Overview

Nuotit is a professional-grade podcast player for iOS and iPadOS that puts audio control in the listener's hands. Unlike creator-focused tools, Nuotit is built for the active listener who wants every podcast to sound perfect — clear voices, balanced levels, and immersive soundscapes tailored to their environment.

**Tagline:** "Better Sound, Smarter Play"
**Philosophy:** Stop just playing podcasts and start truly experiencing them.

### Core Capabilities
- **Professional Audio Processing:** Fix poor podcast audio with studio-grade tools.
- **On-Device AI:** Generate transcripts locally (privacy-first).
- **AI Audio Assist:** AI assisted optimal audio settings based on audio characteristics.
- **Clip Export:** Create shareable video clips (audiograms) with dynamic captions for social media.
- **Smart Library Management:** Advanced playlists with filters, auto-downloads, batch operations.
- **Chapter Navigation:** Jump to specific sections in supported episodes.
- **Audio Profiles:** Save custom settings per show, headset, or environment.
- **Privacy-First:** 100% on-device processing, no tracking, no server uploads.

### Use Cases

| Scenario | Solution |
|----------|----------|
| Host's voice is muffled or distant | Use dynamics engine + EQ to bring voice forward |
| Inconsistent volume levels | Apply compressor/limiter for smooth listening |
| Background music/noise distracts from content | Enable voice isolation to reduce ambient sounds |
| Podcast has no transcript | Generate on-device transcript (iPhone 15 Pro+/M1 iPad+) |
| Want to share highlight on social media | Export clip as video with animated waveform + captions |
| Need different audio for commute vs home | Save audio profiles per environment |

### Pricing

**Free:** Core playback, playlists, downloads, EQ, dynamics, audio profiles, chapters, and more. Most of the app is free.
**Premium** (see App Store for current pricing)**:**
- Voice isolation
- AI Audio Assist
- Clip export with custom templates
- Transcript generation (on supported devices)

**Tip Options:** $3.99 / $12.99 / $44.99 / $179.99 (optional supporter tips)

---

## Professional Audio Features

### 9-Band Parametric Equalizer

**What It Does:** Adjusts specific frequency ranges to enhance or reduce parts of the audio spectrum.

**Frequency Bands:**
- **Sub-bass (20-60 Hz):** Rumble and deep bass.
- **Bass (60-250 Hz):** Thump and warmth.
- **Low midrange (250-500 Hz):** Body and fullness.
- **Midrange (500-2kHz):** Voice fundamentals (the core of human speech).
- **High midrange (2-4kHz):** Voice clarity and definition.
- **Presence (4-6kHz):** Articulation and "closeness."
- **Brilliance (6-20kHz):** Air, sparkle, and sibilance.

**Common Use Cases:**
- **Boost midrange (500-2kHz)** to bring voices forward.
- **Cut bass (60-250 Hz)** to reduce rumble or room tone (mud).
- **Boost presence (4-6kHz)** to add clarity to muffled audio.
- **Cut high frequencies (6-20kHz)** to reduce sibilance (harsh "s" sounds).

**How to Use:**
1. Tap Audio Settings → EQ.
2. Select frequency band.
3. Drag slider up (boost) or down (cut).
4. Use real-time spectrum analyzer to visualize changes.
5. Save as audio profile.

---

### Dynamics Processing

#### Peak Limiter
**Function:** Prevents audio from clipping (distorting) by capping maximum volume.
**When to Use:** Podcasts with sudden loud sections (laughter, claps, ads).
**Setting:** Threshold (dB) — set to -3dB for gentle limiting, -1dB for aggressive.

#### Compressor
**Function:** Reduces dynamic range by making loud parts quieter and quiet parts louder.
**When to Use:** Inconsistent volume across speakers, or loud/quiet episode sections.
**Settings:**
- **Threshold:** Volume level where compression starts (e.g., -20dB).
- **Ratio:** How much to reduce (4:1 = moderate, 8:1 = aggressive).
- **Attack/Release:** How fast compression engages/disengages.

**Example Setup (Inconsistent Volume):**
- Threshold: -18dB
- Ratio: 4:1
- Attack: Fast (10ms)
- Release: Medium (100ms)

#### Expander
**Function:** Increases dynamic range by making quiet parts even quieter (reduces background noise).
**When to Use:** Noisy recordings with constant hiss or room tone.
**Settings:**
- **Threshold:** Volume below which sounds are reduced (e.g., -40dB).
- **Ratio:** How much to reduce (2:1 = gentle, 4:1 = aggressive).

---

### Voice Isolation

**Function:** Reduces non-voice sounds (music, ambient noise) while preserving speech.
**Technology:** On-device AI model trained to distinguish voice from other audio.
**When to Use:**
- Podcasts with distracting background music.
- Street interviews with traffic noise.
- Recordings with significant ambient noise.

**How to Enable:**
1. One-Tap: Tap "Voice Isolation" button during playback.
2. Audio Profile: Save voice isolation setting for specific shows.

**Important:** Requires Neural Engine (iPhone 12+/M1+ iPad). Older devices may see reduced effectiveness.

---

### Real-Time Spectrum Analyzer

**Function:** Visualizes audio frequencies in real-time to help identify issues.
**How to Read:**
- **Left side:** Bass/low frequencies.
- **Center:** Midrange (voice).
- **Right side:** Treble/high frequencies.
- **Height:** Volume of each frequency.

**Common Patterns:**
- **Voice-heavy podcast:** Peaks in center (500Hz-4kHz).
- **Music-heavy podcast:** Balanced across spectrum.
- **Bass-heavy:** Large peaks on left side.
- **Tinny/thin audio:** Missing left side, peaks on right.

---

### Volume Boost & Loudness Analysis

**Volume Boost:** Increases overall volume without clipping (uses headroom monitoring).
**LUFS Meter:** Measures perceived loudness (Loudness Units Full Scale).
**True Peak Meter:** Shows actual peak levels to prevent distortion.

**Typical LUFS Values:**
- -16 LUFS: Broadcast standard (Netflix, Spotify).
- -18 to -20 LUFS: Comfortable podcast listening.
- -24 LUFS or lower: Quiet podcast (needs boost).
- -12 LUFS or higher: Very loud (may cause fatigue).

---

### AI Audio Assist

**Function:** Helps you generate optimized audio settings via your LLM of choice.
**How It Works:**
1. Describe your audio issue in a free text field and select from option checkboxes.
2. Nuotit generates a ready-made prompt.
3. Copy and paste the prompt into your preferred LLM (ChatGPT, Claude, etc.).
4. The LLM returns a JSON settings file.
5. Import the JSON directly into Nuotit to apply the settings.

**Note:** AI Audio Assist is a prompt-generation tool. The LLM analysis happens outside the app; Nuotit itself does not analyse the audio automatically.

**When to Use:**
- Unfamiliar podcast with poor audio.
- Unsure which settings to adjust.
- Want a starting point for a custom profile.

---

## Transcript Features

### Feed-Provided Transcripts
**Format:** WebVTT, SRT.
**Features:**
- Auto-scrolling during playback.
- Tap any sentence to jump to that timestamp.
- Search within transcript.
- Copy text (full or search-filtered).
- Adjustable font size.

### On-Device Transcript Generation
**Requirements:** iPhone 15 Pro+ / M1 iPad+.
**Privacy:** All processing on-device, no internet required.
**Accuracy:** Best for clear English speech. Lower for heavy accents or poor audio.

### Transcript Search & Copy
- Search keywords within transcripts.
- Results highlight in transcript.
- "Copy All" respects search filters.

---

## Clip Export Feature

**What It Is:** Export any segment of a podcast as a shareable video (audiogram) with dynamic transcripts, waveforms, and custom backgrounds.

**Layout Options:**
- Story (9:16) — Instagram/TikTok
- Square (1:1) — Instagram Feed/LinkedIn
- Landscape (16:9) — YouTube/Web

**Customization:**
- Background: solid color, blurred artwork, gradient.
- Caption styles: highlight word, sentence, karaoke.
- Visualizations: waveform, spectrum, pulse, and more.
- Saveable templates for consistent branding.

**Export:** 1080p MP4 at 30fps. Max clip length: 10 minutes.

---

## Smart Playlist System

### Manual Playlists
Add specific episodes or entire shows manually.

### Dynamic Smart Playlists
Auto-update based on rules: show selection, filters (unplayed, downloaded, started, duration), sorting, and episode limits.

### Auto-Downloads
Automatically download new episodes per playlist. Wi-Fi only option available.

### Batch Operations
Mark played/unplayed, download/delete, add to/remove from playlist, export OPML.

---

## Chapter Support
**Formats:** Podcast 2.0 chapters (JSON), ID3 tags (MP3).
**Features:** Chapter titles, optional URLs, optional artwork, swipe navigation.

---

## Library Management

### Collections
- **Downloaded:** All downloaded episodes.
- **Started:** Episodes with progress > 0%.
- **Local Files:** Manually imported audio.

### OPML Import/Export
Full import/export. Standard format compatible with all podcast apps. No lock-in.

### Local Audio Files
**Formats:** MP3, M4A, AAC, WAV, FLAC.
**Import:** Files app, AirDrop, in-app importer.
**Metadata:** Reads ID3 tags (title, artist, artwork, chapters).

---

## Playback Features

- **Persistent Mini-Player** across all screens.
- **Playback Speed:** 0.5x to 4.0x.
- **Continuous Playback** with playlist/show queue.
- **Custom Skip Intervals:** 5s to 2m (forward/backward).
- **Left-Handed Mode** for player button positioning.

---

## Privacy & Data Control

### On-Device Processing
All audio processing, transcription, and clip generation on-device. No data sent to servers. Works offline after initial feed fetch or importing local audio files.

### No Tracking, No Ads
Does NOT collect: listening history, play counts, search queries, behavior analytics.
Stores locally only: subscribed shows, playback progress, downloads, profiles, playlists.

### OPML Freedom
Full export anytime, standard format, no lock-in.

---

## iOS Integration

### Liquid Glass Experience (iOS 26+)
- Adaptive UI elements with depth effects.
- Smooth transitions and animations.
- Enhanced readability with dynamic contrast.

---

## Device Requirements & Performance

| Feature | Minimum Device |
|---------|---------------|
| All features (except below) | iOS 26.0+ |
| Voice Isolation | iPhone 12+ / M1 iPad+ |
| On-Device Transcription | iPhone 15 Pro+ / M1 iPad+ |

---

## Feature Comparison

### Nuotit vs. Standard Podcast Apps

| Feature | Nuotit | Apple Podcasts | Overcast | Pocket Casts |
|---------|--------|----------------|----------|--------------|
| **Audio Processing** | ✅ Full (EQ, dynamics, isolation) | ⚠️ Enhance Dialogue (iOS 26+) | ⚠️ Voice Boost only | ⚠️ Trim Silence only |
| **Transcription** | ✅ On-device (iPhone 15 Pro+) | ⚠️ Server-side | ❌ No | ❌ No |
| **Clip Export with Captions** | ✅ Video + dynamic captions | ❌ No | ⚠️ Video, no captions | ⚠️ Basic video |
| **Chapter Support** | ✅ Yes | ✅ Yes | ✅ Yes | ✅ Yes |
| **Smart Playlists** | ✅ Advanced | ⚠️ Basic | ✅ Yes | ✅ Yes |
| **OPML Import/Export** | ✅ Yes | ❌ No | ✅ Yes | ✅ Yes |
| **Privacy (No Tracking)** | ✅ Yes | ⚠️ Apple Analytics | ✅ Yes | ⚠️ Some tracking |
| **Audio Profiles** | ✅ Yes | ❌ No | ❌ No | ❌ No |
| **AI Audio Assist** | ✅ Yes | ❌ No | ❌ No | ❌ No |
| **Local Audio Files** | ✅ Yes | ❌ No | ✅ Premium | ✅ Yes |

**Nuotit's Strengths:**
- Professional audio processing toolkit (9-band EQ, dynamics) unavailable in other podcast apps.
- Clip export with dynamic burned-in captions — competitors offer video but without caption integration.
- Unique AI Audio Assist prompt workflow for LLM-generated settings.
- European product, on-device everything, zero tracking.

---

## Version History

### 1.26.5 (December 21, 2025)
- Fixed caption export bug.
- Fixed timeline control bug.

### 1.26.4 (December 21, 2025)
- Introduced Clip Export feature.
- Three layout options, dynamic transcripts, custom templates.
- Precision editing tools.

### 1.26.3 (November 28, 2025)
- Full transcript support (feed + on-device).
- Chapter support.
- Left-handed mode.

### 1.26.0 (October 5, 2025)
- iOS 26 Liquid Glass support.

### 1.0.1-1.0.9 (July - September 2025)
- Initial release: core playback, audio processing, smart playlists, OPML, privacy.

---

## Troubleshooting

### Audio Issues
- **Distorted audio after effects:** Reset profile, apply changes gradually (3dB max per band), check True Peak.
- **Robotic voice isolation:** Disable isolation, use EQ midrange boost instead.
- **Volume boost not working:** Audio may already be at max headroom; compress first, then boost.

### Transcript Issues
- **Generation fails:** Free up 1GB+ storage, plug in device, re-download episode.
- **Many errors:** Check for official feed-provided transcript.
- **Search not working:** Try shorter keywords.

### Clip Export Issues
- **Slow export:** Close other apps, let device cool, use simpler visualization.
- **No transcripts in clip:** Generate transcript first.

### Performance Issues
- **Slow/laggy:** Delete old episodes, pause downloads, free up 2GB+ storage.
- **Playback stutters:** Reduce processing intensity, close background apps.

---

## AI Assistant Guidelines

When helping Nuotit users, AI agents should:
1. Prioritize audio quality solutions over playback features.
2. Recommend starting with voice isolation or AI Audio Assist before manual EQ/dynamics.
3. Explain audio concepts in simple terms.
4. Always mention device requirements for voice isolation and transcription.
5. Emphasize privacy features when asked about data collection.
6. Suggest practical audio profile use cases.
7. Remind users clip export and AI Audio Assist are premium features.
8. Guide users to OPML export when migrating.
9. Clarify that AI Audio Assist generates a prompt for the user's own LLM — it does not automatically analyse audio on-device.

### Common User Mistakes
- Applying too much EQ boost (>6dB) causing distortion.
- Expecting instant transcript generation (takes 1-20min).
- Using voice isolation on music podcasts (designed for speech).
- Over-compressing audio (crushing dynamics).
- Not saving audio profiles before adjusting for new show.
- Forgetting to download episodes before generating transcripts.

---

## Support Resources

- **Website:** [nuotit.org](https://nuotit.org)
- **Bluesky:** [@nuotit.org](https://bsky.app/profile/nuotit.org)
- **Threads:** [@nuotitapp](https://www.threads.net/@nuotitapp/)
- **Instagram:** [@nuotitapp](https://www.instagram.com/nuotitapp/)
- **X (Twitter):** [@nuotitapp](https://x.com/nuotitapp)
- **YouTube:** [@nuotit](https://www.youtube.com/@nuotit)
- **Reddit:** [r/nuotit](https://www.reddit.com/r/nuotit/)

## Privacy & Security

- **Data Collection:** None (per App Store privacy label).
- **On-Device Processing:** All audio processing, transcription, and clip generation happens locally.
- **No Cloud Storage:** Your listening data never leaves your device.
- **OPML Freedom:** Full export capability at any time.
- **Privacy Policy:** [nuotit.org/privacy.html](https://www.nuotit.org/privacy.html)
- **EULA:** [Apple Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/)

---

**Copyright:** © 2024-2026 Sunbird OÜ (Petri Kajander)
**License:** Proprietary (App Store distribution)
