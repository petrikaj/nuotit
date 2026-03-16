# Nuotit — Podcast Player

**Version:** 1.26.7 (Latest: March 15, 2026)
**Last Updated:** 2026-03-16
**Platform:** iOS 26.0+ / iPadOS 26.0+

---

## Product Overview

Nuotit is a professional-grade podcast player for iOS that puts audio control in the listener's hands. Unlike creator-focused tools, Nuotit is built for the active listener who wants every podcast to sound perfect—clear voices, balanced levels, and immersive soundscapes tailored to their environment.

**Tagline:** "Better Sound, Smarter Play"
**Philosophy:** Stop just playing podcasts and start truly experiencing them.

### Core Capabilities

- **Professional Audio Processing:** Fix poor podcast audio with studio-grade tools.
- **On-Device AI:** Generate transcripts and optimize audio profiles locally (privacy-first).
- **Clip Export:** Create shareable video clips (audiograms) with transcripts for social media.
- **Smart Library Management:** Advanced playlists with filters, auto-downloads, batch operations.
- **Chapter Navigation:** Jump to specific sections in supported episodes.
- **Audio Profiles:** Save custom settings per show, headset, or environment.
- **Privacy-First:** All processing on-device, no tracking, no server uploads.

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

**Free:** Core playback, playlists, downloads, EQ, dynamics, audio profiles, chapters, and more (everything else except the premium features)
**Premium (see App Store for current pricing):**

- Advanced audio processing (voice isolation)
- AI Audio Assist
- Clip export with custom templates
- Transcript generation (on supported devices)

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
**Setting:** Threshold (dB) - set to -3dB for gentle limiting, -1dB for aggressive.

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

**Function:** Reduces non-voice sounds (music, ambient noise, echo) while preserving speech.
**Technology:** On-device AI model trained to distinguish voice from other audio.
**When to Use:**

- Podcasts with distracting background music.
- Episodes with heavy reverb or echo.
- Street interviews with traffic noise.

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

**How to Use:**

1. Open episode → Audio Settings → Analysis.
2. View LUFS/True Peak readings.
3. Adjust Volume Boost if LUFS < -20.
4. Apply compressor if dynamic range is too wide.

---

### AI Audio Assist

**Function:** AI assisted optimal audio settings based on episode characteristics.
**How It Works:**

1. Suggests EQ adjustments, compression settings, voice isolation.
2. Provides one-tap application or manual tweaking.

**When to Use:**

- Unfamiliar podcast with poor audio.
- Unsure which settings to adjust.
- Want a starting point for custom profile.

**Limitations:**

- Suggestions are starting points (manual tweaking may improve).

---

## Transcript Features

### Feed-Provided Transcripts

**What They Are:** Transcripts included by podcast creators in the RSS feed.
**Supported Formats:** WebVTT, SRT (standard subtitle formats).
**How to Access:**

1. Play episode.
2. Tap Transcript icon.
3. Read along with playback (auto-scrolls).
4. Tap any sentence to jump to that timestamp.

**Features:**

- **Search:** Find specific words or topics within transcript.
- **Copy Text:** Select and copy portions of transcript.
- **Font Size:** Adjust for readability (Settings → Transcript Font Size).

---

### On-Device Transcript Generation

**Requirements:**

- iPhone 15 Pro or later
- M1 iPad or later

**How It Works:**

1. Download episode.
2. Tap Transcript → Generate.
3. App processes audio on-device (no internet required).
4. Transcript appears when complete (time varies by episode length).

**Processing Time:**

- App can run in background during generation.

**Accuracy:** Uses Apple's native models, accurate for clear English speech. Lower for heavy accents, poor audio quality, or technical jargon.

**Privacy:** All processing is on-device. Transcript data never leaves your phone.

---

### Transcript Search & Copy

**Search Function:**

- Tap search icon in transcript view.
- Enter keyword or phrase.
- Results highlight in transcript.
- "Copy All" respects search results (copies only matching sections).

**Use Cases:**

- Find specific topics mentioned in long episodes.
- Copy quotes for notes or social media.
- Verify facts or names.

---

## Clip Export Feature

### Overview

**What It Is:** Export any segment of a podcast as a shareable video (audiogram) with dynamic transcripts, waveforms, and custom backgrounds.
**Use Case:** Share highlights on Instagram Stories, TikTok, LinkedIn, Twitter/X, YouTube Shorts.
**Visualizations:** Move freely around the canvas, snap-to alignment guides, new circular and rounded waveforms, classic animated waveform, spectrum analyzer, pulse, and more.
**Saveable Templates:** Save layouts, colors, and visualization styles for consistent branding.

**Export:** 1080p MP4 at 30fps. Max clip length: 10 minutes. Includes a direct "Save to Photos" option for fast sharing.

**Formats:**

- **Story (9:16):** Instagram/Facebook Stories, TikTok.
- **Square (1:1):** Instagram Feed, LinkedIn.
- **Landscape (16:9):** YouTube, Twitter/X, blog embeds.

---

### How to Create a Clip

#### Step 1: Select Audio Segment

1. Play episode.
2. Tap "Share Clip" icon.
3. Use timeline scrubber to set start/end points.
4. **Zoom Timeline:** Pinch to zoom for precise selection.
5. **Loop Mode:** Toggle to preview clip repeatedly.
6. **Snap to Playhead:** Enable for easier segment selection.

**Max Clip Length:** 10 minutes.

#### Step 2: Choose Layout

- **Story (9:16):** Full-screen vertical video (Instagram Stories, TikTok).
- **Square (1:1):** Centered design (Instagram Feed, LinkedIn).
- **Landscape (16:9):** Traditional video format (YouTube, Web).

#### Step 3: Customize Background

**Options:**

- **Solid Color:** Choose from palette or custom hex.
- **Blurred Episode Art:** Automatically blurs and scales artwork.
- **Gradient:** Two-color gradients (vertical/horizontal/diagonal).

**Pro Tip:** Blurred artwork creates cohesive branding when posting multiple clips from same show.

#### Step 4: Add Transcript Captions (Optional)

**Requirements:** Episode must have transcript (feed-provided or generated).

**Caption Styles:**

1. **Highlight Current Word:** One word highlights at a time.
2. **Sentence by Sentence:** Full sentence appears, then fades.
3. **Karaoke:** Words highlight in sequence within sentence.

**Customization:**

- Font size, Text color, Background box, Position (top/center/bottom).

**Important:** If transcript unavailable, clip exports with audio waveform only.

#### Step 5: Audio Visualization

**Options:**

- **Waveform:** Classic animated waveform (bars or line).
- **Spectrum Analyzer:** Frequency bars (circular or linear).
- **Minimalist:** Pulse circle (clean, subtle) + many more.

**Style Customization:**

- Color (single or gradient), Animation speed, Bar count.

#### Step 6: Save as Template

**Function:** Save layout, colors, visualization, and caption style as reusable template.
**Use Case:** Maintain consistent branding across multiple clips from different episodes.

**How to Save:**

1. Configure clip design.
2. Tap "Save as Template".
3. Name template (e.g., "Instagram Stories - Brand Blue").
4. Access from template library for future clips.

---

### Export & Share

**Export Settings:**

- Resolution: 1080p (Full HD).
- Frame Rate: 30fps.
- Format: MP4 (H.264).

**Share Options:**

1. **Direct Share:** Instagram, TikTok, Twitter (via share sheet).
2. **Save to Photos:** Edit further or post later.
3. **Copy Link:** (requires upload to hosting if using third-party scheduler).

**File Size:** Typically 5-15MB for 60-second clip (depends on complexity).

---

## Smart Playlist System

### Playlist Types

#### Manual Playlists

**Function:** Add specific episodes or entire shows manually.
**Use Case:** Curate thematic playlists (e.g., "Morning Commute," "Deep Learning").

#### Dynamic Smart Playlists

**Function:** Auto-update based on rules (filters, sorting, episode count).
**Use Case:** Always have latest episodes from favorite shows without manual management.

**Configuration Options:**

- **Shows:** Select specific shows to include.
- **Filters:** Unplayed, Downloaded, Started, Duration range.
- **Sorting:** Newest first, Oldest first
- **Episode Limit:** Max episodes to keep in playlist (e.g., "Latest 5").

**Example 1: Morning Commute Playlist**

- Shows: News podcasts + short interview shows.
- Filter: Unplayed
- Sort: Newest first.
- Limit: 10 episodes.

**Example 2: Research Playlist**

- Shows: Academic/deep-dive podcasts.
- Filter: Downloaded
- Sort: Oldest first (chronological learning).
- Limit: None.

---

### Playlist Auto-Downloads

**Function:** Automatically download new episodes from shows in playlist.
**Configuration:**

- Enable per playlist.
- Set download limit (e.g., "Download latest 3 episodes").
- Download only on Wi-Fi (optional).

**Use Case:** Ensure offline access for commutes or flights without manual intervention.

---

### Batch Operations

**Function:** Perform actions on multiple episodes simultaneously.
**Actions:**

- Mark as played/unplayed.
- Download/delete downloads.
- Add to/remove from playlist.
- Export OPML (for shows).

**How to Use:**

1. Tap "Select Multiple".
2. Check episodes/shows.
3. Choose action from bottom toolbar.

---

## Chapter Support

**What Are Chapters?**
Timestamped sections within an episode (e.g., "00:00 Intro," "05:30 Guest Interview," "45:00 Q&A").
**Supported Formats:** Podcast 2.0 chapters (JSON), ID3 tags (MP3).

**How to Use:**

1. Play episode with chapters.
2. Chapter list appears in player.
3. Tap chapter to jump to that section.
4. Swipe left/right to navigate between chapters.

**Metadata Support:**

- Chapter titles.
- Optional URLs (links to resources mentioned).
- Optional images (chapter-specific artwork).

---

## Library Management

### Collections

#### Smart Collections

**Built-In Collections:**

- **Downloaded:** All downloaded episodes.
- **Started:** Episodes with progress > 0%.
- **Local Files:** Manually imported audio files.

**Sorting Options:**

- Date added, Episode date (oldest/newest), Duration, Playback progress.

#### Custom Playlists

See "Smart Playlist System" section above.

### Local Audio Files

**Formats:** MP3, M4A, AAC, WAV, FLAC.
**Import:** Files app, AirDrop, in-app importer. The Add view highlights your last imported files and shows. Direct import option available from custom playlists.
**File Management:** Rename imported files directly via swipe or the context menu.
**Metadata:** Reads ID3 tags (title, artist, artwork, chapters).
**Use Cases:**
- Play audiobooks.
- Listen to conference recordings or voice memos.
- Import paid podcast subscriptions or personal audio files.
- Listen and read along (using the app's on-device transcription)

---

### OPML Import/Export

**What Is OPML?**
Open Podcast Markup Language—standard format for exporting/importing podcast subscriptions.

**Import OPML:**

1. Settings → Import Subscriptions.
2. Select OPML file (from Files app, email, cloud storage).
3. Choose shows to import (or select all).
4. Confirm import.

**Export OPML:**

1. Settings → Export Subscriptions.
2. Generates OPML file with all current subscriptions.
3. Save to Files, share via email, or upload to cloud.

**Use Cases:**

- Migrate from another podcast app (Apple Podcasts, Overcast, Pocket Casts).
- Backup subscriptions.
- Share your podcast list with friends.

---

### Local Audio Files

**Supported Formats:** MP3, M4A, AAC, WAV, FLAC.
**Import Methods:**

1. **Files App:** Open audio file → Share → Open in Nuotit.
2. **AirDrop:** Send from Mac/iPhone → Open in Nuotit.
3. Import within the app from Files or Clipboard

**Metadata Support:**

- Reads ID3 tags (title, artist, artwork, chapters).

**Use Cases:**

- Play audiobooks.
- Listen to conference recordings.
- Import paid podcast subscriptions.

---

## Playback Features

### Persistent Mini-Player

**Function:** Always-accessible player bar at bottom of screen (across all views).
**Controls:**

- Play/pause.
- Skip forward/backward (customizable intervals).
- Playback progress bar.
- Tap to expand full player.

**Customization:**

- Position: Left or right side of screen (Settings → Left-Handed Mode).
- Skip intervals: Set forward/backward skip durations (5s, 15s, 30s, 45s, 60s, 90s, 2m).

---

### Playback Speed

**Range:** 0.25x to 4.0x (incremental).
**Features:** Scrollable menu with a dedicated "Reset to 1.0x" button. You can also tap-and-hold the menu to instantly reset your speed. Includes advanced pitch correction for natural voice rendering across speeds.

**Use Cases:**

- 1.2-1.5x: Comfortable for most content, saves time.
- 1.5-2.0x: Advanced listeners, information-dense podcasts.
- 2.0x+: Review or skim content.
- 0.8-0.9x: Language learning, complex topics.

---

### Continuous Playback

**Function:** Automatically plays next episode when current episode finishes.
**Priority:**

1. Next episode in current playlist.
2. Next episode in show (chronological).
3. Stops if no next episode.

**Configuration:**

- Enable/disable per playlist.
- Global setting (Settings → Playback → Continuous Play).

### Audio Visuals (Real-Time Visualiser)

**Function:** Watch a live, animated visual representation of the audio currently playing right inside the Quick Audio settings view.
**Controls:**

- **Double Tap:** Toggle the visualiser on or off.
- **Tap and Hold:** Change the style of the visualiser.

---

## Privacy & Data Control

### On-Device Processing

**What It Means:** All audio processing, transcription, and clip generation happens on your device—no data is sent to servers.
**Benefits:**

- Complete privacy (no one sees your listening habits).
- Works offline (after initial feed fetch).
- Faster processing (no network latency).

**Technologies:**

- Neural Engine (voice isolation, transcription).
- Core Audio (EQ, dynamics, filtering).
- AVFoundation (playback, export).

---

### No Tracking, No Ads

**Data Nuotit Does NOT Collect:**

- Listening history, Episode play counts, Search queries, User behavior analytics.

**Data Nuotit DOES Store (Locally Only):**

- Subscribed shows, Playback progress, Downloaded episodes, Audio profiles, Playlists.

**Exception:** Some podcasts embed tracking in their RSS feeds (standard practice). Nuotit doesn't block or interfere with these.

---

### OPML Freedom

**Philosophy:** Your subscriptions belong to you, not the app.
**Implementation:**

- Full OPML export anytime (no limitations).
- Standard format (works with all podcast apps).
- No lock-in.

---

## Device Requirements & Performance

### Minimum Requirements

**All Features (except Voice Isolation & Transcription):**

- iOS 26.0+ / iPadOS 26.0+

**Voice Isolation:**

- iPhone 12 or later / M1 iPad or later

**On-Device Transcription:**

- iPhone 15 Pro or later / M1 iPad or later

---

### Performance Optimization

**Background Processing:**

- Transcription continues in background (can leave app).
- Downloads managed by iOS (automatic resume if interrupted).
- Playback uses minimal battery.

**Storage Management:**

- View storage usage
- Batch delete old episodes.
- Auto-delete played episodes (optional, per show).

---

## iOS Integration

### Liquid Glass Experience (iOS 26+)

**What It Is:** iOS 26's new visual design language (translucent, depth-based UI).
**Nuotit Implementation:**

- Adaptive UI elements with depth effects.
- Smooth transitions and animations.
- Enhanced readability with dynamic contrast.

---

## Version History

### 1.26.7 (March 2026)

- Under-the-hood optimizations and minor improvements.

### 1.26.6 (March 2026)

**Visualizer Upgrades & Export Polish:**

- Completely revamped visualizers for Clip Export (freely movable circular and rounded waveforms with snap-to alignment guides).
- **Quick Audio Visuals:** Real-time playback visualizers inside the Quick Audio settings view.
- New direct "Save to Photos" option for exported clips.

**Player & Playback Enhancements:**

- Bigger controls with widened tap areas for easier on-the-go use.
- Smarter Speed Menu: Scrollable, dedicated reset button, and tap-and-hold to instantly reset to 1.0x.
- Audio fixes: Improved pitch correction when changing speeds and resolved a robotic voice effect on iOS 26.

**Library Organization:**

- Add view now highlights recently imported files and shows.
- Rename imported files directly via swipe/context menu.
- Direct import option added to custom playlists.

**Under the Hood:**

- iPadOS 26 tab view UI layout fixes, better memory management, and overall performance boosts.

### 1.26.5 (December 21, 2025)

**Holiday Hotfix:**

- Fixed caption export bug (captions now only export when enabled).
- Fixed timeline control bug (clip limits stay clamped).

### 1.26.4 (December 21, 2025)

**Major Update: Clip Export**

- Introduced Clip Export feature (video clips for social media).
- Three layout options: Story, Square, Landscape.
- Dynamic transcripts with multiple highlight styles.
- Custom templates for consistent branding.
- Precision editing tools (timeline zoom, loop mode, snap to playhead).
- Transcript search improvements.

### 1.26.3 (November 28, 2025)

**Transcripts & Chapters:**

- Full transcript support (feed-provided + on-device generation).
- Chapter support (podcast 2.0 + ID3 tags).
- Adjustable font sizes for transcripts and chapters.
- Left-handed mode (floating player button positioning).
- Animated skip buttons and show notes parsing improvements.

### 1.26.0 (October 5, 2025)

**iOS 26 Support:**

- Liquid Glass experience support.
- Small improvements and bug fixes.

### 1.0.1-1.0.9 (July - September 2025)

**Initial Release Phase:**

- Core playback, Audio processing (EQ, dynamics, voice isolation).
- Smart playlists, OPML import/export.
- On-device privacy focus.

---

## Troubleshooting

### Audio Issues

#### "Audio sounds distorted after applying effects"

**Cause:** Over-processing (too much EQ boost or compression).
**Solution:**

1. Reset audio profile (Audio Settings → Reset).
2. Apply changes gradually (boost/cut by 3dB max per band).
3. Check True Peak meter (should stay below -1dB).

#### "Voice isolation makes audio sound robotic"

**Cause:** Aggressive noise reduction on poor-quality audio.
**Solution:**

1. Disable voice isolation.
2. Use EQ to boost midrange (500-2kHz) instead.
3. Apply gentle compression to balance levels.

#### "Volume boost not working"

**Cause:** Audio already at maximum headroom.
**Solution:**

1. Check LUFS meter (if > -12 LUFS, audio is already loud).
2. Use compressor to reduce dynamic range first, then boost.

---

### Transcript Issues

#### "Transcript generation fails/never completes"

**Causes:** Insufficient storage, Low battery, Episode not fully downloaded.
**Solutions:**

1. Free up 1GB+ storage.
2. Plug in device and retry.
3. Re-download episode (delete + re-download).

#### "Transcript has many errors"

**Causes:** Poor audio quality, Heavy accents, Multiple overlapping speakers.
**Solutions:**

1. Check if podcast provides official transcript (feed-based).

#### "Transcript search not working"

**Cause:** Search query too specific or misspelled.
**Solution:**

1. Try shorter, more general keywords.
2. Use "Copy All" → paste in Notes → use Notes search.

---

### Clip Export Issues

#### "Clip export is slow"

**Causes:** Complex visualization, Long clip duration, Device thermal throttling.
**Solutions:**

1. Close other apps.
2. Let device cool down.
3. Use simpler visualization (minimalist pulse).
4. Export shorter clips.

#### "Transcripts not showing in clip"

**Causes:** Episode has no transcript, Transcript not fully loaded.
**Solutions:**

1. Generate transcript first (Transcript → Generate).
2. Wait for transcript to load (spinner visible).

---

### Playlist Issues

#### "Smart playlist not updating"

**Causes:** Feed refresh interval, Filters too restrictive.
**Solutions:**

1. Manually refresh feeds (pull down on show list).
2. Check filter settings (tap playlist → Edit → Filters).
3. Verify shows are still subscribed and have new episodes.

---

### Performance Issues

#### "App is slow/laggy"

**Causes:** Large library (1000+ episodes), Many active downloads, Low device storage.
**Solutions:**

1. Delete old episodes (batch operations).
2. Pause downloads temporarily.
3. Free up 2GB+ storage.
4. Restart app.

#### "Playback stutters/skips"

**Causes:** Real-time audio processing on older devices, Background app interference.
**Solutions:**

1. Reduce processing intensity (disable voice isolation, simplify EQ).
2. Close background apps.
3. Re-download episode.

---

## AI Assistant Guidelines

When helping Nuotit users, AI agents should:

1. **Prioritize audio quality solutions** over playback features (users choose Nuotit specifically for audio control).
2. **Recommend starting with voice isolation or AI Assist** before diving into manual EQ/dynamics.
3. **Explain audio concepts in simple terms** (avoid jargon like "attack," "Q factor" unless user is familiar).
4. **Always mention device requirements** for voice isolation and transcription features.
5. **Emphasize privacy features** when users ask about data collection or tracking.
6. **Suggest practical audio profile use cases** (commute vs home, wired vs wireless headphones).
7. **Remind users that clip export is a premium feature** if they can't find it.
8. **Guide users to OPML export** when migrating or backing up subscriptions.

### Common User Mistakes

- Applying too much EQ boost (> 6dB) causing distortion.
- Expecting instant transcript generation (takes 1-20min).
- Using voice isolation on music podcasts (designed for speech).
- Over-compressing audio (crushing dynamics).
- Not saving audio profiles before adjusting for new show.
- Forgetting to download episodes before generating transcripts.

---

## Feature Comparison

### Nuotit vs. Standard Podcast Apps

| Feature | Nuotit | Apple Podcasts | Overcast | Pocket Casts |
|---------|--------|----------------|----------|--------------|
| **Audio Processing** | ✅ Full (EQ, dynamics, isolation) | ❌ None | ⚠️ Voice Boost only | ⚠️ Trim Silence only |
| **On-Device Transcription** | ✅ Yes (iPhone 15 Pro+) | ✅ Yes (all devices) | ❌ No | ❌ No |
| **Clip Export with Transcripts** | ✅ Yes | ❌ No | ❌ No | ❌ No |
| **Smart Playlists** | ✅ Advanced | ⚠️ Basic | ⚠️ Basic | ✅ Yes |
| **OPML Import/Export** | ✅ Yes | ❌ Export only | ✅ Yes | ✅ Yes |
| **Privacy (No Tracking)** | ✅ Yes | ⚠️ Apple Analytics | ⚠️ Some tracking | ⚠️ Some tracking |
| **Audio Profiles** | ✅ Yes | ❌ No | ❌ No | ❌ No |
| **Chapter Support** | ✅ Yes | ✅ Yes | ✅ Yes | ✅ Yes |
| **AI Audio Assist** | ✅ Yes | ❌ No | ❌ No | ❌ No |

**Nuotit's Unique Strengths:**

- Only app with professional audio processing (9-band EQ, dynamics).
- Only app with clip export + transcript integration.
- Only app with AI-assisted audio profiles.

---

## Support Resources

- **Main Website:** [nuotit.org](https://nuotit.org)
- **Social Media:**
  - Bluesky: [@nuotit.org](https://bsky.app/profile/nuotit.org)
  - Threads: [@nuotitapp](https://www.threads.net/@nuotitapp/)
  - Instagram: [@nuotitapp](https://www.instagram.com/nuotitapp/)
  - X (Twitter): [@nuotitapp](https://x.com/nuotitapp)
  - YouTube: [@nuotit](https://www.youtube.com/@nuotit) (tutorials and feature demos)
  - Reddit: [r/nuotit](https://www.reddit.com/r/nuotit/) (community support)

---

## Privacy & Security

- **Data Collection:** None (per App Store privacy label).
- **On-Device Processing:** All audio processing, transcription, and clip generation happens locally.
- **No Cloud Storage:** Your listening data never leaves your device.
- **OPML Freedom:** Full export capability at any time (no lock-in).
- **Privacy Policy:** [nuotit.org/privacy.html](https://www.nuotit.org/privacy.html)
- **EULA:** [Apple Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/)

---

**Copyright:** © 2024-2026 Sunbird Ou
**License:** Proprietary (App Store distribution)
