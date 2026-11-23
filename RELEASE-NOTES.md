# Sonic Reference Player — Release Notes

Every release, newest first. Each links to its full notes below.

<a name="versions"></a>
## Versions

- **[0.1.58](#v0-1-58)** — 2026-11-23
  - Sonic Reference Player Pro. Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon.
- **[0.1.57](#v0-1-57)** — 2026-11-23
  - Sonic Reference Player Pro. Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon.
- **[0.1.56](#v0-1-56)** — 2026-11-22
  - Sonic Reference Player Pro. Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. ### Fixed - Metadata sheets: Album Artist. A sheet's plain "Main Artists" column is now always each track's artist. It no longer becomes the album artist when the sheet states none. The album artist comes only from a column that says so ("ALBUM | Main Artists", "Album Artist", "Artist Name on Cover Art").
- **[0.1.55](#v0-1-55)** — 2026-11-22
  - Sonic Reference Player Pro. Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. ### New - Dolby Atmos Renderer preset in Speaker Wiring. Audio I/O Settings > Speaker Wiring... > Presets now includes the Dolby Atmos Renderer's own routing: L R C LFE Lw Rw Lss Rss Lrs Rrs Ltf Rtf Ltm Rtm Ltr Rtr. - The user guide describes Speaker Wiring, pass-through (Dolby and DTS), Send Auro-3D Undecoded and AC Connect artwork. ### Fixed - An Auro-3D file played as 8 undecoded channels. Some Auro-3D carriers state their layout a moment after the Auro signal starts; the Player stopped looking too early and played them undecoded. They now decode to all their channels (an Auro 11.1 file to 12). - The Monitor layout after pass-through. Stopping pass-through now puts the Monitor back on the layout you chose; it could stay on the receiver's 7.1.
- **[0.1.54](#v0-1-54)** — 2026-11-22
  - Sonic Reference Player Pro. Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. ### New - Speaker Wiring, per output device. Audio I/O Settings > Speaker Wiring... shows a plan of the room. Click a speaker and choose the output it is wired to, once for each device. Presets set the Player's order, the P&E Wing order or the Film order in one click. With Monitor on Follow File, every layout then plays to the right speakers. Example: a 5.1 file's surrounds go to your side pair, and a 9.1.6 file finds the wides wherever they are wired. A layout that needs a speaker you have not wired is not offered in the Monitor menu. A Monitor layout you saved by name still uses its own map. This changes playback only, never a Render. - DTS pass-through. The PASS button now appears for DTS streams too, sending them undecoded to an HDMI receiver. A DTS-HD MA stream is sent as its DTS core for now. - Send Auro-3D Undecoded (Monitor menu). An Auro-3D file is sent to the outputs exactly as it is, without decoding, for a receiver or processor that decodes Auro-3D itself. The badge reads "Auro-3D sent undecoded" while it is on. Set the volume to 0 dB and leave the file's channels unchanged, or the receiver cannot find the Auro-3D signal. ### Changed - AC Connect: artwork. When the Pure Audio Streaming app sends a track's artwork, the Player shows it as that track's cover. ### Known - The Dolby speaker order is not yet a preset. It will be added from Dolby's own documentation. - A click at the join between two decoded Auro-3D files is still being looked into. If you hear it, please send the log (Help > Log File...) and the two files' names.
- **[0.1.53](#v0-1-53)** — 2026-11-22
  - Sonic Reference Player Pro. Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. ### Fixed - The Monitor layout after changing the output device. Changing the device in Audio I/O Settings now applies your Monitor layout again. Going from an HDMI receiver (eight outputs, Monitor shown as 7.1) back to a wider interface restores the full immersive layout; it no longer has to be chosen again by hand. ### Changed - ADM files mixed as 7.1.6. With Source on Auto, an ADM whose heights are fixed (non-moving) objects at the four top corners and the two top-middle positions now plays as 7.1.6, as does a 7.1.2 bed with fixed objects at the four top corners. These played as 7.1.4 before. With fixed wide objects as well, the file plays as 9.1.6, as before. An ADM with moving objects still plays as 7.1.4. ### Coming - Speaker wiring per output device. In Audio I/O Settings you will set, once for each device, which output carries each speaker, on a plan of the room, with presets for the Player's order and the P&E Wing order. Every layout will then play to the right speakers with Monitor on Follow File. Not in this build: until then, keep using your own saved Monitor layouts.
- **[0.1.52](#v0-1-52)** — 2026-11-21
  - Sonic Reference Player Pro. Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. This build has no changes you will notice. It is built from the same shared code as soundBlade 1.1.150, whose Edit Fade Mode was rebuilt; the Player has no Edit Fade Mode.
- **[0.1.51](#v0-1-51)** — 2026-11-21
  - Sonic Reference Player Pro. Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. This build adds pass-through to the User Guide. The program itself is unchanged from 0.1.50.
- **[0.1.50](#v0-1-50)** — 2026-11-21
  - Sonic Reference Player Pro. Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. This build fixes the click that could follow a seamless join between two files.
- **[0.1.49](#v0-1-49)** — 2026-11-21
  - Sonic Reference Player Pro. Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. This build adds pass-through of Dolby streams to a receiver over HDMI, and answers a tester's report on ADM, MKV and AC Connect.
- **[0.1.48](#v0-1-48)** — 2026-11-20
  - Sonic Reference Player Pro. Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. This build fixes two faults when playing from the phone (AC Connect): an album that skipped its first tracks, and the Player not closing when quit while a stream was playing.
- **[0.1.47](#v0-1-47)** — 2026-11-20
  - Sonic Reference Player Pro. This build fixes a crash on quit, refuses MKV files sent from the phone (AC Connect), and adds Clear List to the file list's menus.
- **[0.1.46](#v0-1-46)** — 2026-11-19
  - Sonic Reference Player Pro. This build adds choosing an MKV's audio stream and its picture, decodes Auro albums played from Artist Connection, and makes Play wait for the audio device after a sample rate change.
- **[0.1.45](#v0-1-45)** — 2026-11-17
  - Sonic Reference Player Pro. A maintenance build. It brings the Player up to date with the playback engine shipped in soundBlade 1.1.143, where part of the engine's plug-in and latency handling was rewritten.
- **[0.1.44](#v0-1-44)** — 2026-11-17
  - Sonic Reference Player Pro. This build carries the AC Connect fixes that were missing from 0.1.43, and a newer version of the iLok protection.
- **[0.1.43](#v0-1-43)** — 2026-11-15
  - A maintenance release of Sonic Reference Player Pro, built from the same playback engine as soundBlade 1.1.140.
- **[0.1.42](#v0-1-42)** — 2026-11-11
  - New Loop modes, selecting part of a file, object sizes in the room, and the Mac release is now Sonic Reference Player Pro.
- **[0.1.41](#v0-1-41)** — 2026-11-11
  - Upload to Artist Connection, export from Album Info, and a new layout for the top half.
- **[0.1.40](#v0-1-40)** — 2026-11-10
  - MKV files open quickly after the first time, the first open shows its progress, and a launch that got stuck no longer gets stuck again.
- **[0.1.39](#v0-1-39)** — 2026-11-10
  - You can say what a file's channels are, 9.1.6 and 9.1.4 now use the standard SMPTE channel order, and disc images bring their album and track details with them.
- **[0.1.38](#v0-1-38)** — 2026-11-08
  - Pyramix MTFF masters and DDP images play, their tracks are one click away, and the device can follow each file's sample rate.
- **[0.1.37](#v0-1-37)** — 2026-11-08
  - DTS, DTS-HD Master Audio and Dolby TrueHD in MKV files, through FFmpeg you install yourself.
- **[0.1.36](#v0-1-36)** — 2026-11-07
  - Bit-perfect playback with a DIRECT lamp, Exclusive Access, MKV files, and Export removed from this edition.
- **[0.1.35](#v0-1-35)** — 2026-11-06
  - One setting removed, and engine fixes shared with soundBlade.
- **[0.1.34](#v0-1-34)** — 2026-11-05
  - One fix.
- **[0.1.33](#v0-1-33)** — 2026-11-05
  - One addition: the 9.1.4 speaker layout.
- **[0.1.32](#v0-1-32)** — 2026-11-05
  - A file browser, artwork on your tracks, a three-column file list, and a window that scales.
- **[0.1.31](#v0-1-31)** — 2026-10-31
  - DSD (.dsf) playback — please test.
- **[0.1.30](#v0-1-30)** — 2026-10-26
  - Speaker Position correction — please test.
- **[0.1.29](#v0-1-29)** — 2026-10-25
  - Symbols stripped.
- **[0.1.28](#v0-1-28)** — 2026-10-24
  - Plug-in timing and exact renders.
- **[0.1.27](#v0-1-27)** — 2026-10-22
  - Layout fixes.
- **[0.1.26](#v0-1-26)** — 2026-10-22
  - Meters show where each speaker goes, the album cover in Album Info, and the iPad metadata window gets Import and Export.
- **[0.1.25](#v0-1-25)** — 2026-10-21
  - Named speaker layouts, video straight from Artist Connection, and Japanese, Chinese and Korean text shown correctly.
- **[0.1.24](#v0-1-24)** — 2026-10-19
  - Playback rendered ahead, the playhead and meters in step with the sound, and Keyboard Shortcuts fixed.
- **[0.1.23](#v0-1-23)** — 2026-10-12
  - Export to Artist Connection, and a Name field you can type in.
- **[0.1.22](#v0-1-22)** — 2026-10-11
  - Nothing in extra speakers, and a tidier object view.
- **[0.1.21](#v0-1-21)** — 2026-10-11
  - Export from the File menu, gapless play-through, and keyboard shortcuts.
- **[0.1.20](#v0-1-20)** — 2026-10-09
  - ADMs with objects keep their bed as the Source; the master is 7.1.4.
- **[0.1.19](#v0-1-19)** — 2026-10-09
  - ADMs with objects play in 7.1.4; Render for Binaural and 7.1.4 deliverables; heights kept silent in every render.
- **[0.1.18](#v0-1-18)** — 2026-10-09
  - Its own licence; Settings laid out as soundBlade's; binaural as authored, with Auro-Matic upmix as a choice; and Save for binaural, 7.1.4 and Surround.
- **[0.1.17](#v0-1-17)** — 2026-10-07
  - Auro files named as Auro names them, and Artist Connection's Library, Albums and Projects side by side.
- **[0.1.16](#v0-1-16)** — 2026-10-06
  - Auro-Cx and Auro speaker configurations, a room-centric object view, and a reorderable list.
- **[0.1.15](#v0-1-15)** — 2026-10-05
  - Artist Connection: uploads work again, and Create Album is easier to get right.
- **[0.1.14](#v0-1-14)** — 2026-10-04
  - A guided tour for first-time users, and a demo master to try it on.
- **[0.1.13](#v0-1-13)** — 2026-10-03
  - Checking a stereo album: lists, metadata, DDEX and loudness that stays with the file. And tooltips — the Player never showed any until now.
- **[0.1.12](#v0-1-12)** — 2026-09-28
  - Cleaner starts for streamed masters, and Channel Based monitoring that really claims nothing.
- **[0.1.11](#v0-1-11)** — 2026-09-27
  - Artist Connection: open masters straight from your studio's library.
- **[0.1.10](#v0-1-10)** — 2026-09-26
  - Steadier playback, from the engine the Player shares with soundBlade.
- **[0.1.9](#v0-1-9)** — 2026-09-24
  - DDEX arrives, plus a tidier button row.
- **[0.1.8](#v0-1-8)** — 2026-09-23
  - A small follow-up to 0.1.7.
- **[0.1.7](#v0-1-7)** — 2026-09-23
  - Metadata you can see, import and export, an album cover, and the Player's own icon.
- **[0.1.6](#v0-1-6)** — 2026-09-22
  - A Speakers page, speaker naming in SMPTE or ITU-R, a Room view seen from the listener's seat, and diffuse objects heard as diffuse.
- **[0.1.5](#v0-1-5)** — 2026-09-22
  - Object metadata and object timing, on top of the audio-engine corrections that were staged as 0.1.4 and never published.
- **[0.1.4](#v0-1-4)** — 2026-09-21
  - The audio-engine corrections from soundBlade 1.1.87, and the player's own licence.
- **[0.1.3](#v0-1-3)** — 2026-09-21
  - Auro-Cx playback, and the window remembering itself.
- **[0.1.2](#v0-1-2)** — 2026-09-20
  - Two corrections to 0.1.1's MP4 support, found by testing it against a real set of video files.
- **[0.1.1](#v0-1-1)** — 2026-09-20
  - Video files, an About window, and updates where you would look for them.
- **[0.1.0](#v0-1-0)** — 2026-09-20
  - The first build. Sonic Reference Player opens masters, tells you what they are, and plays them correctly on whatever rig you are sitting in front of. It is soundBlade's Preview window as an application of its own: the same engine, the same decoders, the same metering — with no EDLs, no editing and nothing to accidentally change about the file you were sent.

---

<a name="v0-1-58"></a>
## 0.1.58 — 2026-11-23

**Sonic Reference Player Pro.** Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon.

### New

- **Send DTS-HD MA Whole (Pass-through Test)**, in the Help menu, off until ticked and remembered.
  Pass-through normally sends a DTS-HD Master Audio stream as its 48 kHz 5.1 core, so an Auro-3D
  master inside DTS-HD MA reached the receiver as plain DTS 5.1. Ticked, the whole stream is sent
  (7.1, up to 192 kHz, Auro-3D inside). This has not yet been seen working on a receiver: please
  try it. A stream already passing through restarts in the new form from where it was.
- **Skip goes to the next or previous track** of a file that has tracks (an MTFF, a DDP, an MKV
  with chapters). Back within a second of a track's start goes to the one before. Any other file
  keeps the 5-second step.

### Changed

- **Switching between Binaural and speakers keeps playing.** Only the monitoring changes. An Auro-3D
  file is read again for its new decode and carries on from where it was, after a short gap.
- **Ctrl-click Peak Hold clears the held numbers and they stay clear while stopped.** The meters'
  fall after Stop was being held as a new peak (-66 and the like).

### Fixed

- **After pass-through the audio device could stay closed** ("the HDMI interface is no longer
  active" in Audio I/O), most likely when the format or rate changed between files. The Player now
  tries again for up to five seconds, and says so if the device still will not open.

---

**What we would like to hear from testers**

- Send DTS-HD MA Whole: your receiver, what its display shows (format, channels, rate, Auro), and
  whether it plays at all. If it does not, the log (Help > Log File...) has the "Pass-through:" lines.
- After pass-through: whether Audio I/O Settings shows the HDMI device again.

[Back to the list of versions](#versions)

---

<a name="v0-1-57"></a>
## 0.1.57 — 2026-11-23

**Sonic Reference Player Pro.** Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon.

### New

- **Energy and Phase in the object view.** Two new tick boxes along the bottom of the room, both
  off until ticked. **Energy** shows where the finished mix's sound is: a patch at each speaker for
  the level it carries, one patch between two speakers for sound they share, coloured by band
  (orange-red low, amber mid, pale blue high), a white ring where a transient lands, and a cross at
  the centre of the energy. **Phase** joins speakers that carry the same signal: a pale line in
  phase, a red line out of phase in the low, mid or high band, and the worst pair named at the top
  left. A red line means those two speakers cancel in that band when folded down. Both measure the
  mix as delivered, before Solo and Mute. A menu beside them shows all bands or the low, mid or
  high band alone; the boxes and the band are remembered. Phase compares speakers at the same
  instant, so a spaced-microphone recording reads as unrelated.
- **Object size and divergence are heard.** An ADM object with a width, depth or height is spread
  over the speakers around it by ITU-R BS.2127's rule, and divergence splits it into a centre and
  two flanking positions. An object with no size plays exactly as before. It follows the published
  rule, not Dolby's renderer.
- **The picture shows in the album column**, where the cover is. The arrow under it moves the
  picture to the video window; closing that window brings it back. The Video button turns the
  picture off for the file showing; the next file with a picture shows it again.
- **Assign Speakers is a 3-D room.** Seen from behind the listener, with the preset in use named
  above it (Current Setup for the layout as it stands), unassigned speakers hollow, and a Plan
  button for the view from above. Drag a speaker onto another to swap their outputs.

### Changed

- **Dragging the bottom edge of the window changes its height only.** A side or a corner still
  scales the window.
- **The Monitor meters sit 40 px to the right of the Source meters.**
- **Faster drawing on macOS 26.** The app now draws through JUCE's own image; macOS no longer scans
  each repaint.

### Fixed

- **Removing an MKV with DTS or TrueHD audio could hang the Player.** Two ffmpeg helpers started at the
  same moment each kept the other's pipe open, so closing the pipe never reached the helper and the
  app waited for it for ever. The pipes are now closed on exec and a helper's writer can no longer
  block past a stop. Reproduced in a test and fixed there; not yet checked in the app.
- **A hang when the Source layout changed with Energy or Phase showing** (Ctrl-click Source). The
  room drew a reading taken for the old layout against the new one.

---

### Known issues

- **The video in an MKV does not always show.** Still being investigated. If you see it, please
  send the file's name and the log (Help > Log File...), which now has "Video window:" lines.

---

**What we would like to hear from testers**

- Energy and Phase: whether the picture matches what you hear; a red line on material you know to
  be in phase (name the pair and the band shown); whether playback of a wide file breaks up with a
  layer ticked.
- Assign Speakers: your device, the order you set, and any layout that plays to the wrong speaker
  with Monitor on Follow File.

[Back to the list of versions](#versions)

---

<a name="v0-1-56"></a>
## 0.1.56 — 2026-11-22

**Sonic Reference Player Pro.** Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. ### Fixed - **Metadata sheets: Album Artist.** A sheet's plain "Main Artists" column is now always each track's artist. It no longer becomes the album artist when the sheet states none. The album artist comes only from a column that says so ("ALBUM | Main Artists", "Album Artist", "Artist Name on Cover Art").

**What we would like to hear from testers**

- A metadata sheet that imports with the wrong album fields: the sheet itself.
- Speaker Wiring: your device, the preset or order you set, and any layout that plays to the
  wrong speaker with Monitor on Follow File.
- The click between two Auro-3D files: the log (Help > Log File...) from a session where you
  heard it, and the two file names.

[Back to the list of versions](#versions)

---

<a name="v0-1-55"></a>
## 0.1.55 — 2026-11-22

**Sonic Reference Player Pro.** Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. ### New - **Dolby Atmos Renderer preset in Speaker Wiring.** Audio I/O Settings > Speaker Wiring... > Presets now includes the Dolby Atmos Renderer's own routing: L R C LFE Lw Rw Lss Rss Lrs Rrs Ltf Rtf Ltm Rtm Ltr Rtr. - **The user guide** describes Speaker Wiring, pass-through (Dolby and DTS), Send Auro-3D Undecoded and AC Connect artwork. ### Fixed - **An Auro-3D file played as 8 undecoded channels.** Some Auro-3D carriers state their layout a moment after the Auro signal starts; the Player stopped looking too early and played them undecoded. They now decode to all their channels (an Auro 11.1 file to 12). - **The Monitor layout after pass-through.** Stopping pass-through now puts the Monitor back on the layout you chose; it could stay on the receiver's 7.1.

**What we would like to hear from testers**

- Speaker Wiring: your device, the preset or order you set, and any layout that plays to the
  wrong speaker with Monitor on Follow File.
- The click between two Auro-3D files: the log (Help > Log File...) from a session where you
  heard it, the two file names, and whether Send Auro-3D Undecoded was on.
- An Auro 11.1 file that shows six heights: a screenshot with the file selected, and the file's
  name.
- DTS and Auro-3D to a receiver: which receiver, which file, and what its display showed.

[Back to the list of versions](#versions)

---

<a name="v0-1-54"></a>
## 0.1.54 — 2026-11-22

**Sonic Reference Player Pro.** Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. ### New - **Speaker Wiring, per output device.** Audio I/O Settings > Speaker Wiring... shows a plan of the room. Click a speaker and choose the output it is wired to, once for each device. Presets set the Player's order, the P&E Wing order or the Film order in one click. With Monitor on Follow File, every layout then plays to the right speakers. Example: a 5.1 file's surrounds go to your side pair, and a 9.1.6 file finds the wides wherever they are wired. A layout that needs a speaker you have not wired is not offered in the Monitor menu. A Monitor layout you saved by name still uses its own map. This changes playback only, never a Render. - **DTS pass-through.** The PASS button now appears for DTS streams too, sending them undecoded to an HDMI receiver. A DTS-HD MA stream is sent as its DTS core for now. - **Send Auro-3D Undecoded** (Monitor menu). An Auro-3D file is sent to the outputs exactly as it is, without decoding, for a receiver or processor that decodes Auro-3D itself. The badge reads "Auro-3D sent undecoded" while it is on. Set the volume to 0 dB and leave the file's channels unchanged, or the receiver cannot find the Auro-3D signal. ### Changed - **AC Connect: artwork.** When the Pure Audio Streaming app sends a track's artwork, the Player shows it as that track's cover. ### Known - The Dolby speaker order is not yet a preset. It will be added from Dolby's own documentation. - A click at the join between two decoded Auro-3D files is still being looked into. If you hear it, please send the log (Help > Log File...) and the two files' names.

**What we would like to hear from testers**

- Speaker Wiring: your device, the order your outputs are wired in, and any layout that plays
  to the wrong speaker with Monitor on Follow File.
- DTS and Auro-3D to a receiver: which receiver, which file, and what its display showed.
- An Auro 11.1 file that shows six heights: a screenshot of the Preview with the file selected.

[Back to the list of versions](#versions)

---

<a name="v0-1-53"></a>
## 0.1.53 — 2026-11-22

**Sonic Reference Player Pro.** Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. ### Fixed - **The Monitor layout after changing the output device.** Changing the device in Audio I/O Settings now applies your Monitor layout again. Going from an HDMI receiver (eight outputs, Monitor shown as 7.1) back to a wider interface restores the full immersive layout; it no longer has to be chosen again by hand. ### Changed - **ADM files mixed as 7.1.6.** With Source on Auto, an ADM whose heights are fixed (non-moving) objects at the four top corners and the two top-middle positions now plays as 7.1.6, as does a 7.1.2 bed with fixed objects at the four top corners. These played as 7.1.4 before. With fixed wide objects as well, the file plays as 9.1.6, as before. An ADM with moving objects still plays as 7.1.4. ### Coming - **Speaker wiring per output device.** In Audio I/O Settings you will set, once for each device, which output carries each speaker, on a plan of the room, with presets for the Player's order and the P&E Wing order. Every layout will then play to the right speakers with Monitor on Follow File. Not in this build: until then, keep using your own saved Monitor layouts.

**What we would like to hear from testers**

- An ADM that still plays in the wrong layout: the file, or its layout and how its heights are
  delivered (bed channels, fixed or moving objects).
- Pass-through (new in 0.1.49): which Mac, which receiver, which format, and what the receiver's
  display showed.

[Back to the list of versions](#versions)

---

<a name="v0-1-52"></a>
## 0.1.52 — 2026-11-21

**Sonic Reference Player Pro.** Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. This build has no changes you will notice. It is built from the same shared code as soundBlade 1.1.150, whose Edit Fade Mode was rebuilt; the Player has no Edit Fade Mode.

**What we would like to hear from testers**

- Pass-through (new in 0.1.49): which Mac, which receiver, which format, and what the receiver's
  display showed.

[Back to the list of versions](#versions)

---

<a name="v0-1-51"></a>
## 0.1.51 — 2026-11-21

**Sonic Reference Player Pro.** Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. This build adds pass-through to the User Guide. The program itself is unchanged from 0.1.50.

### User Guide

- **Pass-through to a receiver is now described** in the User Guide: when the PASS button
  appears, what is and is not in the path while it plays, how seeking and the next file behave,
  and that it works for files on disk only.

---

**What we would like to hear from testers**

- Pass-through (new in 0.1.49): which Mac, which receiver, which format, and what the receiver's
  display showed.

[Back to the list of versions](#versions)

---

<a name="v0-1-50"></a>
## 0.1.50 — 2026-11-21

**Sonic Reference Player Pro.** Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. This build fixes the click that could follow a seamless join between two files.

### Playback

- **No more click after a seamless join.** When one file in the list ran into the next with no
  gap, a short burst of the wrong audio could be heard about 30 to 50 ms into the new file. It
  came and went from one pass to the next, and only happened when the new file was longer than
  the one before it. Reported with two ADM files (2L-179 tracks 1 and 2). The join itself was
  always exact. Measured on a recording of the output: the join and the 13 seconds after it now
  match the files sample for sample.
- **The log says how each join was made** (lines starting "Join:"), which helps if anything
  like this is heard again.

---

**What we would like to hear from testers**

- If you still hear a click where two files join, please send the two files' names, where in
  the first file you pressed Play, and the log (Help > Log File...).
- Pass-through (new in 0.1.49): which Mac, which receiver, which format, and what the
  receiver's display showed.

[Back to the list of versions](#versions)

---

<a name="v0-1-49"></a>
## 0.1.49 — 2026-11-21

**Sonic Reference Player Pro.** Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. This build adds pass-through of Dolby streams to a receiver over HDMI, and answers a tester's report on ADM, MKV and AC Connect.

### Pass-through to a receiver (new, for testing)

A Dolby Digital, Dolby Digital Plus or Dolby TrueHD stream can be sent to a receiver over HDMI
**undecoded**, so the receiver decodes it, Atmos included.

- **The PASS button** appears above DIM when all of these hold: the selected file (or the MKV
  stream you chose) is one of those Dolby formats, the output device is an HDMI receiver that
  accepts it, and FFmpeg is installed as for DTS and TrueHD playback (see the User Guide).
- **Turn PASS on and press Play.** The receiver's display should show the format.
- **While it plays, nothing of the Player's is in the path:** no meters, no Desk, no volume, no
  Solo or Mute, no Binaural. Set the level on the receiver.
- **Seeking** starts the stream again from the new place; the receiver may take a moment to lock.
- **Files on disk only**, not files streamed from Artist Connection or the phone.
- Moving from one file to the next is not gapless.
- Turn PASS off to play the file through the Player as before.

**Tested so far** on one receiver with one Dolby TrueHD with Atmos stream. Dolby Digital and
Digital Plus have not been tried on a receiver yet. It relies on formats macOS offers on HDMI
but does not document, so it may behave differently on other Macs and receivers.

---

### ADM

- **A 9.1.4 or 9.1.6 mix delivered as a bed plus fixed objects now plays as 9.1.4 or 9.1.6.**
  When every object is fixed in place and a pair sits at the wide positions, Source: Auto
  chooses 9.1.4, or 9.1.6 with a top-middle pair as well. The wide objects play from the wide
  speakers alone. Choosing the layout by hand (Ctrl-click Source) still works.

---

### MKV

- **Auro-3D inside DTS-HD MA decodes with the surrounds and rears the right way round.**

---

### AC Connect

- **The phone is told when the Player quits**, so it stops trying.

---

### Window

- **The white bar beside the meters can be dragged further left**, giving the meters more room.
  It stops 40 px from the album cover. Double-click it to reset.

---

### Known issue

- A click between two ADM files that should join seamlessly (reported with 2L-179 tracks 1 and
  2). The files themselves join cleanly, so the fault is ours; it is being investigated.

---

**What we would like to hear from testers**

- Pass-through: which Mac, which receiver, which format, and what the receiver's display showed.
  If PASS does not appear, or there is no sound, please send the log (Help > Log File...).
- Does your 9.1.4 or 9.1.6 ADM now open with the wides on their own speakers?

[Back to the list of versions](#versions)

---

<a name="v0-1-48"></a>
## 0.1.48 — 2026-11-20

**Sonic Reference Player Pro.** Requires macOS 11 (Big Sur) or later, on Intel or Apple silicon. This build fixes two faults when playing from the phone (AC Connect): an album that skipped its first tracks, and the Player not closing when quit while a stream was playing.

### AC Connect (playing from the Pure Audio Streaming app)

- **An album no longer skips its first tracks.** The phone asks for play before the Player has finished
  reading the track. The Player started anyway, stopped when the track was ready, and then moved to the
  next one. It now waits for the track, and the phone shows it buffering until the sound starts.
- **A seek sent by the phone before the track is ready is kept**, and applied when it starts.
- The log now records each time the Player itself moves to the next track.

---

### Fixes

- **Quitting while a stream is playing no longer hangs.** In 0.1.47, quitting while a FLAC file was
  streaming from Artist Connection or the phone could leave the Player spinning, and the phone waiting.
- **A stream that stops answering no longer ties up the Player.** The same fault could occur without
  quitting, if the network dropped while a FLAC file was streaming.

---

**What we would like to hear from testers**

- From the phone, play an album you have not played since opening the Player. Does it start on track 1?
- Quit while a stream is playing. Does the Player close?
- If not, please send the log (Help > Log File...).

[Back to the list of versions](#versions)

---

<a name="v0-1-47"></a>
## 0.1.47 — 2026-11-20

**Sonic Reference Player Pro.** This build fixes a crash on quit, refuses MKV files sent from the phone (AC Connect), and adds Clear List to the file list's menus.

### Fixes

- **Quitting no longer crashes** when audio from Artist Connection or AC Connect was still loading, or an
  upload was in progress. Streaming and uploads are now stopped before the app closes.
- **An MP4 with a sound track is no longer taken for a picture** to pair with another file. Only an MP4 with
  no audio is offered as a picture.
- An MP4 whose first check found no picture is checked once more.

---

### AC Connect

- **A playlist from the phone that holds an MKV file is refused**, and the phone shows "MKV files are not
  supported." Whatever was playing carries on, and the list does not change.

---

### File list

- **Clear List** is on the file list's right-click menus.

---

**What we would like to hear from testers**

- Play an album from Artist Connection or the phone, then quit while it plays. Does the app close cleanly?
- If anything crashes on quit, please send the crash report and the log (Help > Log File...).

[Back to the list of versions](#versions)

---

<a name="v0-1-46"></a>
## 0.1.46 — 2026-11-19

**Sonic Reference Player Pro.** This build adds choosing an MKV's audio stream and its picture, decodes Auro albums played from Artist Connection, and makes Play wait for the audio device after a sample rate change.

### MKV files

- **An MKV with several audio streams lists one row per stream** under the file, above its chapters. Click a
  row to play that stream. A stream that cannot play is greyed, with the reason. The choice is kept with the
  list and the next session, and Measure and Render use it too.
- **Details names the stream playing**: its title, else its format.
- **The picture opens in the video window.** The MKV's video is copied, not re-encoded, into a cached file
  the first time (H.264 and HEVC only), then opens in step with the sound.
- **Cover art and liner notes**: a cover attached to the MKV shows as the file's artwork; a PDF attached to it
  opens from the row's right-click menu, "Liner Notes...".
- **An Auro-3D stream inside an MKV is now checked again when you choose it.** Before, a file first opened on
  another stream (a TrueHD stream, say) stayed "not Auro" whichever stream you then chose, and an Auro
  stream played its eight channels undecoded.
- Dolby TrueHD plays its 7.1 bed. The Atmos objects are not decoded.

---

### Artist Connection and AC Connect

- **Auro-3D albums streamed from Artist Connection or played from the phone (AC Connect) are decoded**, as
  files on disk are: the Auro badge, all their channels, and binaural through Auro's renderer. They played
  as their undecoded channels (e.g. 5.1) before.

---

### Playback

- **After the device's sample rate changes, Play waits for the device to start** (up to 6 seconds) before
  playing. If it never starts, Play does not start either, the window says so, and an AC Connect phone is told.
- Every line of the log now carries the time of day.

---

### Album Info

- Removing every file from the list no longer asks whether to delete Album Info you never set or changed:
  it is simply cleared. Album Info you entered or imported is still asked about.

---

**What we would like to hear from testers**

- Open an MKV with several audio streams (an Auro DTS-HD MA and a TrueHD, for example) and click each stream's
  row. Does an Auro stream show the Auro badge and all its channels? (FFmpeg must be installed for DTS and
  TrueHD; see the guide.)
- Play an Auro album from Artist Connection or from the phone. Auro badge, all channels, sound?
- If Play ever does not start after a sample rate change, please send the log (Help > Log File...).

[Back to the list of versions](#versions)

---

<a name="v0-1-45"></a>
## 0.1.45 — 2026-11-17

**Sonic Reference Player Pro.** A maintenance build. It brings the Player up to date with the playback engine shipped in soundBlade 1.1.143, where part of the engine's plug-in and latency handling was rewritten.

### Changes

- No new features and no visible changes.
- The playback engine is the same code as soundBlade 1.1.143. The rewritten parts handle plug-ins
  and latency on the soundBlade Desk, which the Player does not use, but they are in the
  same playback path.

---

**What we would like to hear from testers**

- Does everything play as it did in 0.1.44? Any difference in playback, meters or
  gapless play-through, please send the log (Help > Log File...).

[Back to the list of versions](#versions)

---

<a name="v0-1-44"></a>
## 0.1.44 — 2026-11-17

**Sonic Reference Player Pro.** This build carries the AC Connect fixes that were missing from 0.1.43, and a newer version of the iLok protection.

### AC Connect (playing from the Pure Audio Streaming app)

- **Fixed "Could not stream ... Item not found or not accessible" on the phone.**
  The Player replaced the link the phone sent with a reference to this computer's own
  Artist Connection studio. When the track was not in that studio, it could not play.
  Every track now plays the link the phone sent.
- **An old error is no longer sent to the phone.** A file list restored at launch could
  report its own failed reads against the phone's new playlist.
- **Stop and disconnect keep the playlist.** The phone goes on to send Play and seek for
  the same tracks, and they now work.
- **An expired Artist Connection sign-in says so**, and signs out, instead of failing
  on every request. Log in again in Settings > Accounts.
- Every AC Connect command is written to the log with its answer.

---

### iLok protection

- **The Player now uses PACE Fusion 6.** Your existing licence should carry over. With
  no licence, the activation window appears at launch.
- **If the licence is removed while the Player is open**, playback pauses and a message
  stays up until the licence is found again.

---

**What we would like to hear from testers**

- Does the Pure Audio Streaming app play to the Player through AC Connect? If not,
  please send the log (Help > Log File...).
- Does your iLok licence open this build without asking again?

[Back to the list of versions](#versions)

---

<a name="v0-1-43"></a>
## 0.1.43 — 2026-11-15

A maintenance release of **Sonic Reference Player Pro**, built from the same playback engine as soundBlade 1.1.140.

### What changed

- **The playback engine is the one in soundBlade 1.1.140.** That release changed
  where playback starts a plug-in, so that playback and an export match. The Player
  hosts no plug-ins on a timeline, so there is nothing new to see or hear here — the
  two applications are simply kept on one engine.
- Nothing else has changed since 0.1.42.

---

**What we would like to hear from testers**

- Anything that plays differently from 0.1.42. Nothing should.

[Back to the list of versions](#versions)

---

<a name="v0-1-42"></a>
## 0.1.42 — 2026-11-11

New Loop modes, selecting part of a file, object sizes in the room, and the Mac release is now **Sonic Reference Player Pro**.

### Sonic Reference Player Pro

- The Mac download is **Sonic Reference Player Pro** — the full feature set, for
  testers. It has its own name and settings; the first launch copies your existing
  settings across.
- The App Store and iPad edition is **Sonic Reference Player**.

---

### Loop

- **Loop** is a square button that moves on with each click:
  - **Off** (white arrows) — the list plays through and stops after the last file.
  - **Loop 1** (blue arrows with a 1) — this file, again and again, **from its start**.
  - **Loop All** (blue arrows) — the list, back to the first file after the last.
  - **Loop Selection** (blue arrows with a yellow bar) — the selection, again and
    again; offered when there is one.

---

### Selecting part of a file

- **Drag across the Layout's Overview column** to select part of the file, as in a
  soundBlade EDL (a yellow band with red edges). It is for playing only.
- When stopped, Play starts at the selection. A click clears it.

---

### ADM masters

- **An ADM with objects has a 7.1.4 Source** — its bed (7.1.2 at most in Dolby
  Atmos) and objects mixed together. The Overview still shows the bed as **Bed
  configuration**; the Monitor is yours to set.
- Objects in the room **scale with the view**, and an object with a size has a
  **faint ring** as wide as the area it spreads over.

---

### Also

- **Help ▸ Show Tour** is gone; the tour still shows on first launch.

---

**What we would like to hear from testers**

- Do the four Loop modes do what you expect?
- Does selecting in the Overview column feel like soundBlade's?
- Does Pro pick up your settings on first launch?

[Back to the list of versions](#versions)

---

<a name="v0-1-41"></a>
## 0.1.41 — 2026-11-11

Upload to Artist Connection, export from Album Info, and a new layout for the top half.

### Artist Connection tab

- **Upload** chooses files or folders (folders with their subfolders) and uploads into
  the selected library folder. A folder that already exists is added to, not duplicated.
  Hidden files and sidecars are skipped.
- **New Folder** creates a folder in the library.
- Files and folders can be dragged in.
- AC Connect plays plain web links, signed out as well.

---

### Album Info

- **Export** (CSV or DDEX) is in the Album Info window.
- A DDEX release that is missing details (label, UPC...) can still be written:
  **Export Anyway** leaves those fields blank.
- Titles and artists come from each file's own tags. No release date means today.
- Opening it fills a blank album and artist from the selected file, and the layout and
  genre when every file agrees.

---

### Layout

- The top half is in four columns: Overview | Loudness | the album, with the timecode
  under it | Desk and the Monitor meters with the fader. Play is under the album.
- **Help > Explore the Player** opens a page that shows what each part does.
- Save buttons turn blue when there is something to save.
- **Cmd-,** opens Settings.

---

**What we would like to hear from testers**

- Does Upload put everything where it should in the library?
- Does the new top half fit your screen?

[Back to the list of versions](#versions)

---

<a name="v0-1-40"></a>
## 0.1.40 — 2026-11-10

MKV files open quickly after the first time, the first open shows its progress, and a launch that got stuck no longer gets stuck again.

### MKV: fast after the first open

To play an MKV, the Player first reads the whole file once to find where its audio is. On a long film that
takes a while: about 10 seconds for a 65-minute Dolby TrueHD track, longer when it streams from Artist
Connection.

- **The first open now shows a progress bar**: *Reading "name.mkv" for the first time*, with a percentage.
  The Player has not stopped responding.
- **What it finds is saved**, so every later open of that file is fast, even after you quit and relaunch
  (about 10 seconds down to a fraction of a second on that film). It is kept in the Player's own cache folder,
  never beside your file, and read again only if the file changes.
- An MKV streamed from Artist Connection is read once, not again for each use.

---

### A launch that stopped responding

If the Player stopped responding while opening your list and had to be Force Quit, the next launch now
brings the list back **without opening any file**, and says so.

- Double-click a file, or select it and press Play, to open it.
- If one file stops the Player again, **right-click it and choose Remove from List**. That does not open it.

---

### Help > Log File...

Shows the Player's log file in Finder, so you can send it to us when something goes wrong.

---

**What we would like to hear from testers**

- Does an MKV open quickly the second time, including after a relaunch?
- If the Player stops responding, please send the log (Help > Log File...).

[Back to the list of versions](#versions)

---

<a name="v0-1-39"></a>
## 0.1.39 — 2026-11-10

You can say what a file's channels are, 9.1.6 and 9.1.4 now use the standard SMPTE channel order, and disc images bring their album and track details with them.

### Say what a file's channels are

**Ctrl-click (or right-click) the Source read-out** to choose the layout of the selected file: every
layout, Channel Based, or Auto (what the file itself says). Binaural is offered on a two-channel file.

- The choice decides the rows' speaker names, the Desk, routing, Measure and Render.
- It is kept for that file, with the list and the session. **It is never written into the audio file.**
- On an ADM it names the bed; the objects are unchanged.
- Choosing reloads the file from its start.

---

### 9.1.6 and 9.1.4 in SMPTE order

In SMPTE order the outputs now run 1 to 16 in order: L R C LFE Lss Rss Lrs Rrs, then the wides **Lw Rw on
outputs 9 and 10**, then the heights. The Speaker Layout window lists the rows in that order.

- A 16-channel (9.1.6) or 14-channel (9.1.4) file with no layout of its own is read in this order too.
- Film order is unchanged.

---

### Disc images: album and track details

- **MTFF masters open at any channel count** (a 12-channel 7.1.4 one has been seen). The channels are named
  Ch 1, Ch 2…, since the file does not say which speaker each one is; Ctrl-click Source to say.
- An MTFF's UPC, album title, artist, label, catalog number and genre fill in **Album Info** where it is
  blank. Nothing you already typed is replaced, and a disc naming another album adds nothing.
- A DDP's text file now gives each track's performer, and the disc's title and performer.
- Track rows read "Title — Performer", with the credits in the tooltip. **Right-click a track > Track
  Metadata...** shows everything the disc says about it (read only).

---

### AC Connect

When the Artist Connection app plays to the Player:

- The app is told when each track ends, so it moves on to the next one correctly.
- A stream that fails is reported to the app once, not over and over.
- Stop and disconnect from the app clear the playlist.

---

**What we would like to hear from testers**

- On a 9.1.6 or 9.1.4 system, does every speaker play what it should?
- Does choosing a layout from Source give the rows and the sound you expect?
- With AC Connect, does a playlist play through from one track to the next?

[Back to the list of versions](#versions)

---

<a name="v0-1-38"></a>
## 0.1.38 — 2026-11-08

Pyramix MTFF masters and DDP images play, their tracks are one click away, and the device can follow each file's sample rate.

### Pyramix MTFF

MTFF masters open as one row with their album name, artist, cover and track list. Only 32-bit float stereo
has been seen so far. Any other layout is refused, and says why.

---

### DDP images

The Player now plays DDP images: open the image file or drop its folder. The row is named after the folder.
In the Mac App Store and iPad versions, drop the folder.

---

### Tracks under the triangle

Click the triangle on an MTFF, a DDP or an MKV with chapters. Under the metadata you now get **one row
per track**: number and title, ISRC, and length (an MKV chapter has no ISRC).

- **Click a track to play from it.** Play carries on to the end of the file.
- The track you are hearing turns white.
- The tracks are in disc order however the list is sorted.

The same marks are drawn on the waveform.

---

### Change Sample Rate based on File

A new tick in **Audio I/O Settings**, off by default. Before a file plays, the app stops, sets the device
to the file's rate, waits up to half a second for the device to report it, then plays.

- It comes ahead of **Enable SRC**. If the device cannot take the rate, Enable SRC decides: on converts
  the file, off plays it at the wrong rate.
- The device stays at the last file's rate. Files needing different rates do not play gaplessly.

---

### Artist Connection

- **Streaming is faster to start and scrub.** Streamed audio is now held in memory while the app is
  open, shared by playback and waveform drawing, and read ahead further.
- **Double-click an album** in the Albums tab, or right-click and choose **Add Album to File Pane**,
  to add its tracks in album order at the bottom of the list. Each streams like a Library file.
  A row shows the track's title.
- **Downloading from Artist Connection is switched off for now.** Files stream. Copies you already
  downloaded still open.
- A file's **Type** column says PCM and its **Details** the channel count, and a name no longer ends in
  its layout and rate.

---

### Also

- **⌘-O** opens files.
- **Object view:** every speaker now meters from its own level, panned objects included. Speakers and object
  spheres are drawn in blue underneath.
- The User Guide covers all of this.

---

**What we would like to hear from testers**

- Do an MTFF's and a DDP's tracks and marks land where the disc says?
- With Change Sample Rate ticked, does your interface reach each file's rate before the sound starts?

[Back to the list of versions](#versions)

---

<a name="v0-1-37"></a>
## 0.1.37 — 2026-11-08

DTS, DTS-HD Master Audio and Dolby TrueHD in MKV files, through FFmpeg you install yourself.

### DTS and Dolby TrueHD in MKV

The Player does not include a DTS or Dolby TrueHD decoder. It now uses **FFmpeg**, a free program
you download and put in place yourself. With it, the DTS, DTS-HD MA and Dolby TrueHD tracks of an
MKV play **bit-exact**: an Auro-3D carrier inside DTS-HD MA survives.

- Put the `ffmpeg` program in `~/Library/Application Support/Sonic Reference Player/Codecs/`
  (the Player creates the folder the first time it needs it). An FFmpeg already installed in
  `/opt/homebrew/bin` or `/usr/local/bin` is found too.
- No restart needed: open the MKV again.
- Without FFmpeg, the file's row says so, and the Player tells you where to put it.
- If macOS blocks a downloaded copy, the Player says FFmpeg *would not run*. The User Guide's new
  section **Playing DTS and Dolby TrueHD** shows how to unblock it.
- Dolby TrueHD with Atmos plays its channel bed and says *Atmos not decoded*.
- Starting play or jumping takes about a twentieth of a second longer than other files, and the
  first opening of a long MKV takes some seconds while the Player reads through it.
- Mac only.

The Player plays the MKV's default audio track. Choosing between several tracks in one file comes later.

---

**What we would like to hear from testers**

- With FFmpeg in place, do your DTS and TrueHD MKVs play, and do the channel names look right?
- Without it, is it clear what to do?

Everything else is as in 0.1.36.

[Back to the list of versions](#versions)

---

<a name="v0-1-36"></a>
## 0.1.36 — 2026-11-07

Bit-perfect playback with a DIRECT lamp, Exclusive Access, MKV files, and Export removed from this edition.

### Bit-perfect playback, shown by the DIRECT lamp

When nothing in the path changes a PCM file, it reaches the output device with its own sample values.
The new **DIRECT** lamp lights when that is so. **DIRECT+G** means only the Main Output volume and
dither are applied after it; at 0.0 dB it is DIRECT. Hover over the lamp for what it means.

---

### Dither comes after the Main Output volume

The Main Output volume is now applied last, followed by dither. Automatic dither turns on only when
something changes the samples or the volume is not at 0.0 dB, so a DIRECT file is never dithered.

---

### Exclusive Access (hog mode)

A new tick in **Audio I/O Settings** claims the audio device for the Player alone, so no other
application can mix into it or change its sample rate. It is off by default. While it is on and
another application holds the device, playback stops and the Player says so. The first time a file
plays DIRECT with it off, the Player offers to turn it on.

---

### MKV files

Audio in MKV files now opens: PCM, FLAC (Auro-3D carriers included) and Dolby Digital / Dolby Digital
Plus. DTS, DTS-HD MA and Dolby TrueHD do not play. An MP4 with Dolby Digital Plus Atmos (JOC) says so
in its details: it plays as its channel bed, without the Atmos objects.

---

### Export and Name Tags removed

**File ▸ Export…** and the **Name Tags** settings page are gone from this edition. The Player plays
and checks masters; it does not make new audio files. Save Playlist, metadata and Measure reports
are unchanged.

---

### Also

- **Speaker Positions** is hidden in Settings for now. Saved positions are kept.
- The Sonic Studio logo is updated, and the Open, Save and loudness reference buttons have new tooltips.
- The User Guide has new screenshots.

---

**What we would like to hear from testers**

- Does the DIRECT lamp light for your 24-bit and 16-bit files at 0.0 dB, with the device at the file's rate?
- With Exclusive Access on, does another application (Music, a browser) stay silent, and does the
  Player recover when it is turned off?
- Do your MKV files open and play?

Everything else is as in 0.1.35.

[Back to the list of versions](#versions)

---

<a name="v0-1-35"></a>
## 0.1.35 — 2026-11-06

One setting removed, and engine fixes shared with soundBlade.

### Render Plug-ins Ahead is no longer a setting

Playback now always renders 4 blocks ahead, and the row has gone from Settings. It is a safety margin
for the CPU, not latency compensation: a plug-in that sometimes takes longer than a block, like a
linear-phase EQ, is absorbed instead of dropping out. If you had it set to Off, that is now ignored.
Controls respond that much later (4 blocks of 512 samples at 96 kHz is 21 ms), as they already did at
the default.

---

### Fix: no click when stopping or seeking during the wait after Play

Audio that had not been heard yet could come in abruptly if you pressed Stop or moved the playhead
while Play was waiting for plug-in latency. It now ramps up from silence.

---

### Fix: automation on a plug-in in the Master slots

If a Master slot's plug-in carries automation, it now follows the audio at that point, in 64-sample
steps while a value moves, as an export does. It used to land early by the latency ahead of it.

---

**What we would like to hear from testers**

- With a linear-phase EQ on the Master slots, is playback free of dropouts?
- Do you hear any click when pressing Stop or moving the playhead just after pressing Play?

Everything else is as in 0.1.34.

[Back to the list of versions](#versions)

---

<a name="v0-1-34"></a>
## 0.1.34 — 2026-11-05

One fix.

### Fix: the Layout pane's Out column follows the speaker layout

Changing the speaker layout left the **Out** column showing the old layout's speaker names until
something else redrew the list. It now updates straight away, from the Monitor menu, the Speakers
tab in Settings and a saved layout alike.

Everything else is as in 0.1.33.

[Back to the list of versions](#versions)

---

<a name="v0-1-33"></a>
## 0.1.33 — 2026-11-05

One addition: the 9.1.4 speaker layout.

### New: 9.1.4 speaker layout

**9.1.4** is now a layout: 9.1.6 without its top middle pair, in both SMPTE and Film channel
order. Choose it in the Monitor menu; it is offered when your device has at least 14 outputs.

A 14-channel file that does not say what it is still reads as 7.1.6. A file or an ADM bed that
does say reads as 9.1.4.

**What we would like to hear from testers**

- Does 9.1.4 land on the right outputs, in the channel order you use?

Everything else is as in 0.1.32.

[Back to the list of versions](#versions)

---

<a name="v0-1-32"></a>
## 0.1.32 — 2026-11-05

A file browser, artwork on your tracks, a three-column file list, and a window that scales.

### New: File > Files...

A file browser in its own window.

- **Double-click or drag** to add everything selected to the list. A **folder** brings all
  the audio inside it, sub-folders included.
- It lists only the audio files the Player can open.
- The first time it opens, macOS may ask for access to your Music folder and network volumes.
- Mac direct download only.

### New: artwork on a track

**Edit Metadata** has an **Album Artwork** row, with a picture and three buttons.

- **Select...** (or drop an image on the picture) and **Remove** take effect when you press
  **Save**.
- **Apply to Album...** asks first, then writes the image into every file in the list that
  names this file's album. Files on another album are skipped.
- The image goes **into the file** in a **DSF, FLAC or WAV**. Your image is stored as it is,
  and no audio sample is touched, though the file's size and date change.
- **ADM masters** carry no artwork. Other formats keep the image's location beside the file.

**Which picture a row shows:** the art in the file, always, if it has any. Otherwise the
image chosen for that file; the album's cover, if the file's metadata names that album; an
image named after the file; or a **cover, folder or front** image in the same folder, unless
the file names a different album. A folder's image is only shown, never written into a file.

### DSD files

- A DSF's **title, artist, album, genre and ISRC** now show and save, in the file's own tag.
- **DSD128 and DSD256 now play at 352.8 kHz** (384 kHz for the 48 kHz family). DSD64 stays at
  176.4 / 192 kHz. A device at another rate gets sample-rate conversion, as for any file.
- Each file gets a **3 ms fade at its start and end** during playback, because a DSF starting
  or ending on a hard cut can click. Exports and Measure do not include it. On one continuous
  recording split into tracks, you may notice a very short dip at each join.
- DSF waveforms build faster, one channel per processor core.

### The file list

- **Three columns: Name, Type, Details.** Click a heading to sort. The sort is the real order:
  what plays next and what a saved playlist holds.
- **Dragging in many files** now fills in each file's type and details straight away.
- **Dropping a folder brings its sub-folders too.**
- The **metadata triangle** has moved to the right-hand end of the row.
- **Save**, beside Open, saves the playlist. It lights when the list has changed, and saves
  over the playlist's own file. File > Save Playlist... still asks for a name.
- A newly loaded file always starts at the beginning. It could start partway through before.

### The window and the waveforms

- **The whole window scales as you resize it,** text included. Menus and alerts stay their
  usual size.
- **Mono and stereo files** get large, detailed waveforms that fill the layout pane.
- **Overs are marked in red.** An over is at least 3 samples in a row at full scale. This is
  not true peak, and it is not the meter's over lamp, which lights on one sample.
- **Stereo files** no longer show a Source read-out, and leave room for the cover, which is now
  centred beside the loudness.

### Smaller changes

- **Measure** no longer opens a report: it asks whether you want one, then where to save it.
- **Ctrl-click any meter** to clear every held peak and over lamp.
- **Fix: a click going from one track to the next** on resampled files. The hand-over between
  files is now a short crossfade.
- **Fix: saving tags into some WAV files could crash the app.** This affected a WAV being given
  a metadata block it did not already have.
- **Loudness:** the 2.0 and 5.1 fold-downs used for loudness measurement now follow Dolby's
  published Lo/Ro and BS.2127 rules. The EBU R128 / BS.1770-4 measurement itself is unchanged.

**What we would like to hear from testers**

- Does artwork stay put, and show in your other software, after Save and Apply to Album? Try it
  on copies of your masters first.
- Do you still hear a click between tracks? Tell us the file type and your device's sample rate.
- Does the window, the file list or the waveform drawing feel slow on a large folder or an ADM?

Everything else is as in 0.1.31.

[Back to the list of versions](#versions)

---

<a name="v0-1-31"></a>
## 0.1.31 — 2026-10-31

DSD (.dsf) playback — please test.

### New: DSD files (.dsf)

The Player now opens **DSF** files (DSD64, DSD128, DSD256; mono up to 5.1). Open one
from the file list or drag it in, like any other master.

How it plays:

- **Converted to PCM** — 176.4 kHz, 32-bit float (192 kHz for 48 kHz-family DSD),
  whatever the DSD rate. Everything works on it as on any other file: meters,
  loudness, binaural, speaker position correction, monitor solo/mute.
- The conversion filter is **flat to 30 kHz** and removes DSD's ultrasonic noise above
  70 kHz before it reaches your speakers.
- The file panel shows what the file really is — for example
  **DSD64 · 2.8224 MHz → 176.4 kHz**, **1 bit (DSD)**.

Things to know:

- **DSD masters read about 6 dB lower** than their PCM equivalent. The conversion is
  at unity: SACD's 0 dB reference is half modulation, so a DSD master peaking at
  "0 dB SACD" shows about -6 dBFS here. Nothing is added to make it louder, so nothing
  can clip.
- If your device is not at 176.4 kHz, the file is sample-rate converted to it, as for
  any other file (the SR lamp lights).
- Title and artist tags in a DSF (ID3) are not shown yet.
- **Not yet:** sending the DSD itself to a DSD DAC (DoP). That is coming in a later
  build; for now every output plays the PCM conversion.

**What we would like to hear from testers**

- Do your DSF files open and play, at every DSD rate you have?
- Does seeking and looping behave as with a WAV?
- Anything that clicks, drops out or sounds wrong — with the file's DSD rate and
  channel count.

Everything else is as in 0.1.30.

[Back to the list of versions](#versions)

---

<a name="v0-1-30"></a>
## 0.1.30 — 2026-10-26

Speaker Position correction — please test.

### New: Speaker Position correction

If your speakers are not exactly where the layout says they should be, the Player can
now make monitoring sound as if they were.

**Application Settings > Speaker Positions**

- Choose the layout you monitor on (Stereo, 5.1, 7.1.4, ...).
- For each speaker, enter where it really is, measured from your listening position:
  - **Azimuth** — degrees from front centre. Positive is to your left, negative to your
    right, up to 180 behind you. (L at 30 means 30 degrees to the left.)
  - **Elevation** — degrees above ear height.
  - **Distance** — metres from your listening position.
- Tick **Correct speaker positions**.

What it does:

- **Correct angles** — each channel is panned between your real speakers so it sounds
  from its ideal direction. A speaker within 3 degrees of where it should be plays its
  channel on its own.
- **Correct distances** — nearer speakers are delayed and turned down so every speaker
  arrives at the same time and level as the farthest one. The Delay / Trim column shows
  what each speaker gets.
- **Reset** puts every speaker of that layout back on its ideal position.

Things to know:

- **Monitoring only.** It is never in an export or a measurement.
- It is applied last, right before dither — after the meters and monitor solo/mute.
- It is off while Binaural is on (headphones have no speakers to move).
- **Changing anything stops playback**, so a change never clicks mid-programme.
- Each layout keeps its own measurements; the layout you monitor on decides which set
  is used.
- The Player keeps its own measurements — positions entered in soundBlade are not
  carried over.

**In the object view**

- **Cmd-Option-click a speaker** to change that speaker's position in a small pop-up.
- While correction is on, each speaker that is off its ideal angle shows an **orange
  ring where it really is**, joined to its cabinet by a dashed line. The cabinets stay
  at the ideal positions — that is where the sound is now placed.

**What we would like to hear from testers**

- Does the image move where you expect when you enter your real positions?
- Do phantom images (a channel panned between two speakers) sound stable at your
  listening position?
- Does the time alignment sound tighter with **Correct distances** on?
- Anything that clicks, drops out or sounds wrong — with your layout and the numbers
  you entered.

### Fixed

- **Object view:** the Ctrl-click Mute/Solo menu now opens where you click, not at the
  bottom of the view.

Everything else is as in 0.1.29.

[Back to the list of versions](#versions)

---

<a name="v0-1-29"></a>
## 0.1.29 — 2026-10-25

Symbols stripped.

### Copy protection

- The app is now shipped with its debug symbols stripped, as a release should be.
  Nothing else changes.

Everything else is as in 0.1.28.

[Back to the list of versions](#versions)

---

<a name="v0-1-28"></a>
## 0.1.28 — 2026-10-24

Plug-in timing and exact renders.

### Playback

- **Playback is now in time with plug-ins whose latency is over half a second.**
  Delay compensation was capped at 0.5 s and quietly cut anything longer short --
  MAAT thEQred alone reports 0.68 s at 96 kHz -- so with such a plug-in in an EDL,
  tracks played out of time with each other and with a render. Every delay is now
  compensated in full.
- **Play flashes while it waits for plug-in latency.** With long-latency plug-ins
  the first sound can take a second or more to arrive; the Play button flashes
  until it does.

### Renders

- **A render is exactly the samples from its start to its end**, both rounded to
  the nearest sample on the timeline, and plug-in edges land on the same sample in
  every render and in playback.
- **Plug-ins running at the start or end of a render are fed the audio around
  them**, as playback feeds them, and only the render's own span is written.
- **A render never leaves out a plug-in without saying so** -- one that should
  print but cannot stops the render and is named.

### For testers

- Play an EDL with MAAT thEQred (or any plug-in reporting more than half a second
  of latency) next to a track without it: the two stay in time.

Everything else is as in 0.1.27.

[Back to the list of versions](#versions)

---

<a name="v0-1-27"></a>
## 0.1.27 — 2026-10-22

Layout fixes.

### Layouts

- The Speaker Layout dialog lists 5.1.2, 5.1.4, 7.1.2, 7.1.4 in that order, as
  the menus do.
- A line above the Auro layouts in every layout list.
- An EDL opened in the Player shows its own layout (Auro 13.1, not 7.1.6), and
  the Monitor menu offers the Auro layouts for it.
- The time read-out draws reliably wherever it appears.

### For testers

- Open the Speaker Layout dialog and check the order.
- Open an Auro EDL: it reads its Auro layout.

Everything else is as in 0.1.26.

[Back to the list of versions](#versions)

---

<a name="v0-1-26"></a>
## 0.1.26 — 2026-10-22

Meters show where each speaker goes, the album cover in Album Info, and the iPad metadata window gets Import and Export.

### Meters

- Each **Monitor** meter shows, under its speaker name, the **output** it goes
  to (in gold) -- the meters stay in speaker order, so a room wired out of order
  reads at a glance (Ltm 15, Rtm 16, Ltr 13, Rtr 14).
- The **Source** meters show their channel number at the same height, so the two
  rows line up. Both rows are a little shorter.

### Album Info

- The album's **cover** is shown in Album Info, with **Change...** to pick a new
  image (JPEG or PNG). It is applied on Save; Cancel keeps the old one.

### iPad

- The metadata window has **Import** and **Export**, as on the Mac. An exported
  CSV or DDEX report is saved wherever you choose in Files.
- With the metadata window open, **tapping another file** shows that file in it.
  Unsaved edits are asked about first (Save / Don't Save / Cancel); Cancel keeps
  the window on its file.

### For testers

- A layout with outputs out of order: check the numbers under the Monitor meters.
- Album Info > Change...: pick an image, Save.
- iPad: open Metadata, edit a field, tap another file -- answer each choice.

Everything else is as in 0.1.25.

[Back to the list of versions](#versions)

---

<a name="v0-1-25"></a>
## 0.1.25 — 2026-10-21

Named speaker layouts, video straight from Artist Connection, and Japanese, Chinese and Korean text shown correctly.

### Named speaker layouts

- **Custom is replaced by layouts you name and save** -- "AURO-Room",
  "STEREO MONITOR". In **Speaker Layout** (Monitor menu, or Settings >
  Speakers): pick a layout, set its outputs, type a **Name** and press
  **Save**. Output changes are applied once the layout is saved.
- Saved layouts are listed **by name** in the Monitor menu and the Speaker
  Layout list, and the Monitor button shows the name. **Delete** removes one.
- Output assignments and saved layouts are **kept between launches**.
- A device with fewer outputs switched on than the monitor layout needs now has
  the missing ones **switched on** (7.1.4 on a 16-output interface with two
  ticked gets 12) -- it only adds, never removes, and never changes the device.

### Video

- **Streamed Artist Connection movies show their picture** -- no download
  needed. The video opens when the file is selected and follows the sound.
- A **Video** button appears while the selected file has video; it opens and
  closes the video window.

### Text

- **Japanese, Chinese, Korean** and other scripts are shown correctly
  everywhere -- in names, metadata and every text field. They used to show as
  unrelated Latin letters (the text itself was always stored correctly).

### Also

- Layout lists run 5.1.2, 5.1.4, 7.1.2, 7.1.4.
- Artist Connection: a folder whose triangle did nothing now opens.
- Auro-Matic Upmix is removed from the Monitor menu for now.

### iPad

- **Metadata** and **Album** buttons, as on the Mac.
- **Open** also takes a movie (.mov, .m4v, a picture-only .mp4) and pairs it
  with the selected master.
- **Hold a file name** to read the whole of it; the file's menu opens when you
  let go.
- The file list's divider follows your finger and can always be dragged back.

### For testers

- Speaker Layout: set outputs on 9.1.6, name it, Save; pick it from the Monitor
  menu after another layout; quit and reopen.
- Select a streamed movie from Artist Connection: the picture plays in step.
- Type ありがとう in a name field.

Everything else is as in 0.1.24.

[Back to the list of versions](#versions)

---

<a name="v0-1-24"></a>
## 0.1.24 — 2026-10-19

Playback rendered ahead, the playhead and meters in step with the sound, and Keyboard Shortcuts fixed.

### Playback

- Playback now renders a few audio blocks **ahead** of what you hear, so a
  moment of heavy processing no longer drops out. On by default (4 blocks --
  21 ms at 512 samples / 96 kHz): **Settings > General > Render Plug-ins Ahead**
  (Off / 2 / 4 / 8 blocks; Off is the old behaviour). Controls are heard that
  much later; Main Output Volume is not.
- **The playhead shows what you hear** -- it no longer runs ahead of the audio,
  waits at the start until the sound arrives, and Stop leaves it where the
  sound stopped. The video follows it.
- **The channel meters** are in step with the sound.
- **Loop is sample-exact**: the end plays out in full and the start follows
  with no gap; a file played to its end is no longer cut short.

### Keyboard Shortcuts

- Setting a shortcut works: the dialog shows the keys as you press them.
- **Option-letter keys** (Option-I, Option-E... which start an accented letter
  on a Mac keyboard) can be set and now work as shortcuts.
- **Delete** in the dialog erases what you pressed, to try again.
- A key already in use asks first, naming the command that has it.

### For testers

- Play a long file with Loop on over its end: no gap, no click, nothing cut.
- Settings > Keyboard Shortcuts: set Option-I on a command and use it.

Everything else is as in 0.1.23.

[Back to the list of versions](#versions)

---

<a name="v0-1-23"></a>
## 0.1.23 — 2026-10-12

Export to Artist Connection, and a Name field you can type in.

### Export

- **Add to Artist Connection** (File > Export..., shown while signed in):
  uploads what the export writes — **each type into its own Library folder
  and album**, "<name> - (7.1.4)", "<name> - (Binaural)" — optionally with a
  share link per album. You are asked the name, the album and the link before
  anything renders. **No share link = nothing published.** A folder that
  already exists can be **replaced**, files and album tracks, so each album
  and its link stay the same. A message says when the upload is done, with
  any links copied to the clipboard.
- **Quitting while an upload runs asks first.**
- **Name field**: type between the tags — typed text becomes fixed-text tags;
  Delete next to a tag takes it out.

### For testers

- Sign in, export a 7.1.4 and a Binaural with Add to Artist Connection and a
  share link; export again to the same name and choose Replace — the link
  should still play the new files.

Everything else is as in 0.1.22.

[Back to the list of versions](#versions)

---

<a name="v0-1-22"></a>
## 0.1.22 — 2026-10-11

Nothing in extra speakers, and a tidier object view.

### Monitoring: nothing in extra speakers

- **On a wider monitor, the speakers the master does not have stay silent.**
  7.1.4 on a 9.1.6 system plays channel for channel, with nothing at all in
  the wides or top middles. Before, every speaker was spread a little into its
  neighbours.
- A speaker the monitor lacks goes to the two nearest speakers at its own
  height. Folding down to 5.1 or stereo still folds the heights in.
- **Auro-Matic Upmix** is unchanged — still in the Monitor menu, off by
  default.

### Object view

- **Room / Side / Top on top; zoom and the checkboxes along the bottom**, the
  zoom slider a third of the width.
- **Stacked objects:** the list over a stack stays open as you move onto it;
  click a name to bring that object to the front.

### For testers

- 7.1.4 material on a 9.1.6 monitor: the wides and top middles silent.

Everything else is as in 0.1.21.

[Back to the list of versions](#versions)

---

<a name="v0-1-21"></a>
## 0.1.21 — 2026-10-11

Export from the File menu, gapless play-through, and keyboard shortcuts.

### Export

- **File > Export…** replaces the Render button: the export window, with
  your name tags, bit depth and BWF details, and the layouts — Stereo,
  Binaural, 5.1, 7.1.4, 9.1.6.
- **Type**: Interleaved, or **Individual** — one file per speaker of each
  layout, named by speaker.
- **Open in Player** adds the exported files to the list.
- **A progress window with Cancel** shows each file as it is written.

### Playing

- **The list plays through**: with Loop off, the next file starts when one
  ends — gapless when it has the same layout, after a short pause otherwise.
  Loop on repeats the current file.

### Loudness

- **Integrated is coloured against the reference** — green under it, yellow
  to red over it.
- Reference presets, **Save to ADM** for a measured ADM, and a PDF loudness
  report.

### Also

- **Keyboard Shortcuts** — every menu command, change, add, clear, reset,
  with search and Save / Import. The menus' shortcuts now always work.
- File menu: Open, Open Video, Save Playlist, Export.
- ADM column after #; shorter tooltips throughout.
- **Artist Connection**: with one studio you go straight to it.

### For testers

- Export with **Individual**: one file per speaker, each playable.
- Let the list play through two files of the same layout: no gap at the join
  — also with Binaural on.

Everything else is as in 0.1.20.

[Back to the list of versions](#versions)

---

<a name="v0-1-20"></a>
## 0.1.20 — 2026-10-09

ADMs with objects keep their bed as the Source; the master is 7.1.4.

### ADMs with objects: the bed is never changed

- **Correcting 1.1.109**, which showed such an ADM's Source as 7.1.4: **the
  Source is the bed, exactly as the file states it** — a 7.1.2 bed reads
  7.1.2, in the Preview and in an EDL, and is never rewritten.
- **The Monitor starts on the bed** (7.1.2), to match the file; set it to
  7.1.4 to hear the objects in all four heights.
- **The master is 7.1.4** — the Desk, Render and every export: objects go
  straight to its four heights, and the bed's own channels to their own
  speakers.
- **A 7.1.2 bed's top-middle channels feed the front and rear heights on
  their side only** (−3 dB each). In 1.1.109 part of them reached the side
  surrounds at ear level.
- **An ADM export never writes a position into a bed channel.**
- Renders and exports keep heights to the two nearest speakers at their own
  height (was three).

### What each file becomes

What the Preview — and a file opened as an EDL — does with each kind of
master. **Source** is the file's own layout, exactly as it states it — never
changed. **Master** is what it is mixed into: the Desk, and every render and
export.

| Your file | Source / Master | On speakers | On headphones (Binaural) | Render 7.1.4 | Render Binaural |
|---|---|---|---|---|---|
| Stereo | Stereo | folded to your speakers | not binauralized | skipped | skipped |
| 5.1 / 7.1 | its own layout | folded to your speakers | the renderer chosen in Settings | the original channels, **heights silent** (you are warned first) | the renderer chosen in Settings |
| 5.1.4, 7.1.4, 9.1.6 … | its own layout | folded | Settings renderer | 7.1.4 as is; wider is folded, heights into heights | Settings renderer |
| ADM, bed only | its bed | folded | Settings renderer | as its bed's layout | Settings renderer |
| **ADM with objects** (bed with fewer than four heights, or no bed) | Source **the bed (e.g. 7.1.2)**, Master **7.1.4** — the Monitor starts on the bed; set it to 7.1.4 to hear all four heights | folded from the 7.1.4 master | Settings renderer | the master, as is | Settings renderer |
| ADM with objects, bed with four or more heights | its bed | folded | Settings renderer | folded, heights into heights | Settings renderer |
| Auro-3D carrier | its Auro layout | a smaller system gets Auro's own decode; otherwise straight through | **Auro's renderer, always** | its own layout into 7.1.4 | Auro's renderer |
| Auro-Cx | its bed | folded | Settings renderer | as a channel file | Settings renderer |

- **Folded** means each speaker of the file goes to where it belongs among your
  speakers; nothing is added.
- **Heights stay heights in every render and export**: a speaker the target has
  goes straight across, any other to the two nearest speakers at its own
  height. A narrower master's heights stay silent; a downmix (to Stereo or 5.1)
  still folds them in.
- **Binaural plays the master as authored.** The Settings renderer is Auro
  (the default), SOFA with your HRTF, or Apple Spatial Audio.
- **Auro-Matic Upmix** (Monitor menu, off by default) upmixes on speakers and
  headphones where Auro supports both layouts — never in a render or export.
- **A Render carries no Solo, Mute, DIM, Main volume or upmix**, and in a batch
  no Desk faders: each file is rendered as authored.

### For testers

- An ADM with a 7.1.2 bed and objects: Source 7.1.2, Monitor 7.1.2; set the
  Monitor to 7.1.4 to hear all four heights.

Everything else is as in 0.1.19.

[Back to the list of versions](#versions)

---

<a name="v0-1-19"></a>
## 0.1.19 — 2026-10-09

ADMs with objects play in 7.1.4; Render for Binaural and 7.1.4 deliverables; heights kept silent in every render.

### ADMs with objects play in 7.1.4 — this changes the sound

- **An ADM whose bed has fewer than four height speakers now plays in 7.1.4.**
  Until now its objects were squeezed into the bed's own speakers (a 7.1.2
  bed's two top middles) and spread again over a 7.1.4's four heights. Objects
  now go straight to the four heights.
- **Bed channels go to the speaker their label names**; Dolby's labels are
  recognised as heights, and a 5.1.4 bed is no longer taken for 7.1.2.

### Render

- **Render...** replaces the Save buttons: the selected files' **Binaural**
  and/or **7.1.4**, one at a time in the background, 24-bit WAV beside each
  master (or in the download folder), with its metadata, added to the list.
- **A small bar at the end of each row** shows that file's progress.
- **A master narrower than 7.1.4 is named first** — its heights stay silent.
- Renders of MP4, FLAC and Auro files are much faster.

### What each file becomes

What the Preview — and a file opened as an EDL — does with each kind of
master, on each output. "Plays in" is the layout the Desk shows and every
render starts from; it is set when the file is opened and does not change when
you switch monitors.

| Your file | Plays in | On speakers | On headphones (Binaural) | Render 7.1.4 | Render Binaural |
|---|---|---|---|---|---|
| Stereo | Stereo | folded to your speakers | not binauralized | skipped | skipped |
| 5.1 / 7.1 | its own layout | folded to your speakers | the renderer chosen in Settings | the original channels, **heights silent** (you are warned first) | the renderer chosen in Settings |
| 5.1.4, 7.1.4, 9.1.6 … | its own layout | folded | Settings renderer | 7.1.4 as is; wider is folded, heights into heights | Settings renderer |
| ADM, bed only | its bed | folded | Settings renderer | as its bed's layout | Settings renderer |
| **ADM with objects** (bed with fewer than four heights, or no bed) | **7.1.4** — objects placed straight into it | folded from 7.1.4 | Settings renderer | as is | Settings renderer |
| ADM with objects, bed with four or more heights | its bed | folded | Settings renderer | folded, heights into heights | Settings renderer |
| Auro-3D carrier | its Auro layout | a smaller system gets Auro's own decode; otherwise straight through | **Auro's renderer, always** | its own layout into 7.1.4 | Auro's renderer |
| Auro-Cx | its bed | folded | Settings renderer | as a channel file | Settings renderer |

- **Folded** means each speaker of the file goes to where it belongs among your
  speakers; nothing is added.
- **Every layout render — Render, Export, Album Renders — keeps heights where
  they are**: a speaker the file has goes straight across, any other only among
  speakers at its own height, so a narrower master's heights stay silent. A
  downmix (to Stereo or 5.1) still folds the heights in.
- **Binaural plays the master as authored.** The Settings renderer is Auro
  (the default), SOFA with your HRTF, or Apple Spatial Audio.
- **Auro-Matic Upmix** (Monitor menu, off by default) upmixes on speakers and
  headphones where Auro supports both layouts — never in a render or export.
- **A Render carries no Solo, Mute, DIM, Main volume or upmix**, and in a batch
  no Desk faders: each file is rendered as authored.


### For testers

- An ADM with a 7.1.2 bed and objects should read 7.1.4.
- Render a 5.1 and an ADM to 7.1.4 and Binaural; compare with the Preview.

Everything else is as in 0.1.18.

[Back to the list of versions](#versions)

---

<a name="v0-1-18"></a>
## 0.1.18 — 2026-10-09

Its own licence; Settings laid out as soundBlade's; binaural as authored, with Auro-Matic upmix as a choice; and Save for binaural, 7.1.4 and Surround.

### Licensing — CHANGED

- **This build needs its own Sonic Reference Player iLok licence.** It is now
  wrapped with the Player's own product licence, so **a soundBlade licence no
  longer unlocks it.** Ask us for a Player licence before installing if you do
  not have one.

### Binaural now plays the master as authored

- **The Auro binaural renderer no longer upmixes.** Until now it ran in a mode
  that upmixes everything (Auro-Matic for Headphones), so a 5.1 or 7.1.4 master
  on headphones was heard upmixed. It now plays the material as it is. **Binaural
  through Auro will sound different — drier, with no added height.**

### Auro-Matic Upmix (monitoring only)

- **Monitor menu > Auro-Matic Upmix** — off by default, remembered. On
  speakers, Auro's engine upmixes the material to the Monitor layout; on
  headphones, Auro's binaural upmixes again. Offered only where Auro renders
  both layouts (5.1, 7.1, 5.1.4, 7.1.4 and the Auro configurations — not 9.1.6).
  The Monitor read-out says "→ Auro-Matic". Never in a Save or Measure.

### Save

- **Binaural Save** — beside Binaural while it is on: the master through the
  binaural renderer chosen in Settings (Auro's for Auro material), 2-channel
  24-bit WAV, "<name> - Binaural".
- **Monitor Save** — beside the Monitor button on 7.1.4 or 5.1: what you are
  monitoring, rendered by our own renderer (an ADM's objects placed in the room),
  "<name> - 7.1.4" or "<name> - Surround", 24-bit.
- Saved beside the master, or in the download folder for an Artist Connection
  download, with its metadata, and added to the list.
- **A Save runs in the background** — pick other files and play them while it
  works; the button shows its progress and cancels it. (Measure renders its own
  copy too.)

### Menus and Settings

- **The Sonic Reference Player menu** has **Application Settings...** and
  **Audio I/O Settings...** (⌥A). The Monitoring menu is gone; Settings is no
  longer in the File menu; Help no longer has Open Demo Master (the tour still
  offers it).
- **Settings > General**: **Enable SRC** (on by default) and updates.
- **Settings > Speakers**: the layout, then **Enable Binaural Monitoring** and
  the renderer / HRTF at the bottom — as soundBlade has them.
- **Settings > Accounts**: Artist Connection — status, one **Login / Logout**
  button that follows the sign-in live, **Reveal Log** — and **AC Connect**
  (the Artist Connection app on your phone plays to the Player; off by default).
- Small text in Settings is easier to read.

### Artist Connection

- **The cloud button appears only while signed in.** File > Artist
  Connection... signed out opens Settings > Accounts.
- **Downloads go to a folder you choose** (asked once, remembered, shown with
  **Set Folder...**), **keep their extension**, and can be removed with
  right-click > **Delete Downloaded File...**. Clear Downloads is gone.
- **Double-click a picture** in the Library to make it the album cover.
- **Uploading is no longer offered in the Player** — upload from soundBlade.

### Preview

- **Solo and Mute under every meter**; a silenced channel draws no meter.
- **Monitor meters**: level readout, Solo/Mute per speaker, follow **P/H**.
- **Right-click a file > Show File Location...**
- **Clicking a file with video opens the video window** if it is closed.
- **Drop a picture** anywhere to make it the album cover.

### For testers

- **Install with a Player licence** — a soundBlade one will not open it.
- Binaural on a 5.1/7.1.4 master with the Auro renderer: still binaural, no
  added height? Then try Auro-Matic Upmix.
- Save a binaural and a 7.1.4 version; play each against the Preview.

Everything else is as in 0.1.17.

[Back to the list of versions](#versions)

---

<a name="v0-1-17"></a>
## 0.1.17 — 2026-10-07

Auro files named as Auro names them, and Artist Connection's Library, Albums and Projects side by side.

### Licensing

- **Unchanged.** This build is wrapped with soundBlade's product licence, so a
  soundBlade iLok unlocks it exactly as before.

### Auro-3D: named as Auro names them

- **An Auro file (a carrier or Auro-Cx) is named by the configuration it
  declares**, as listed in Auro's own licensee manual — for example
  "Auro 11.1 (7.1+4H)" or "Auro 9.1 (5.1+4H)" — and its channels take Auro's
  own names in Auro's own order: L R C LFE Ls Rs Cs Lb Rb HL HR HC T HLs HRs.
- **Every Auro configuration is recognised**, from LCR and Quad to Auro 13.1.
- **A 7.1.4 Auro master now reads "Auro 11.1 (7.1+4H)"** with HL/HR/HLs/HRs
  rows. **It sounds the same**: on a monitor of the same speakers (7.1.4,
  5.1.4, 7.1, 5.1) it goes straight through, channel for channel.
- **Auro configurations appear in the Monitor menu and Speaker Layout dialog
  only when the selected file is Auro.**

### Artist Connection

- **Library | Albums | Projects**: the cloud view now has all three.
  - **Albums** lists the studio's albums with their covers; Set Cover, Share
    and End Review as your sign-in allows.
  - **Projects** lists the studio's whole project list, wherever each was made,
    newest first; **Get Links** shows a published project's share links.
- **The Open (folder) button returns from the cloud view** to the file list as
  you left it; from the list it opens the file chooser as before.

### For testers

- Open an Auro 7.1.4 master: rows should read HL HR HLs HRs and it should
  sound exactly as in 0.1.16.
- Artist Connection: try the Albums and Projects tabs.

Everything else is as in 0.1.16.

[Back to the list of versions](#versions)

---

<a name="v0-1-16"></a>
## 0.1.16 — 2026-10-06

Auro-Cx and Auro speaker configurations, a room-centric object view, and a reorderable list.

### Licensing

- **Unchanged.** This build is wrapped with soundBlade's product licence, so a
  soundBlade iLok unlocks it exactly as before.

### Objects: room-centric (changes what you hear)

- **Speakers stand in the room's corners**, as engineers lay out a room
  (ITU-R BS.2127), and polar (EBU) object positions are converted into the
  room the same way. **The panner follows the same rule**, so an object is
  heard where it is drawn — this changes the sound of Dolby-style (Cartesian)
  objects near the corners.
- **Room-centric** tick in the object view switches back to the old
  listener-centred sphere, for comparison.
- **Isometric** tick: the room drawn as macOS Audio MIDI Setup draws one,
  with a lounge chair at the listening position.
- Soloing an object shows the others as muted (visible, dimmed, no level).

### Auro-3D and Auro-Cx

- **Auro speaker configurations**: Auro 9.1, 10.1, 11.1, 12.1 and 13.1 —
  for monitoring, and to name files that declare one.
- **Auro-Cx**: the Auro badge, "Auro-Cx" with its declared quality, speaker
  names, declared loudness, and its tags and cover.
- **Auro-Cx inside a movie MP4 now decodes** (it showed as "A3DS lossy").
- Auro carrier detection is lighter on ordinary files.

### The list

- **Reorder it**: drag rows, the row menu, or Cmd-Option-Up/Down. After a
  metadata sheet import it offers to follow the sheet's track order.
- **Cmd-A** selects every file.

### Monitoring

- **Monitor menu**: Follow File (the default) or pin a layout for every file;
  only layouts your output device can carry; "Channel Based" removed.
- **Stereo**: Source says Stereo (or Binaural); no Monitor control or
  headphones button when it is stereo in and stereo out.
- **Source** is a read-out of what the file declares. The ADM column shows
  only for ADMs. **DIM** lights when engaged.
- **Export DDEX** clears waveform cache folders from the delivery first.

### For testers

- Open an Auro-Cx movie (or .mp4a) and an ADM with objects; toggle
  Room-centric and Isometric.

Everything else is as in 0.1.15.

[Back to the list of versions](#versions)

---

<a name="v0-1-15"></a>
## 0.1.15 — 2026-10-05

Artist Connection: uploads work again, and Create Album is easier to get right.

### Licensing

- **Unchanged.** This build is wrapped with soundBlade's product licence, so a
  soundBlade iLok unlocks it exactly as before.

### Artist Connection

- **Fixed: every upload was refused by storage** and never arrived.
- **Create Album** now opens as a list with nothing selected — tick the
  tracks you want. They go in Track Number order, titled from each file's
  Title tag, and you can reorder and rename them before the album is made.
- **Uploads keep their subfolders.**
- **Fixed: a studio's top level was listed twice.**

### Demo master

- The built-in "Deep Note" demo now carries its album info.

### DDEX

- If a delivery's files cannot be read, the report says so, rather than
  reporting MD5 mismatches.

### For testers

- Upload a small folder of tagged files to your studio, then Create Album
  from it and check the track order and titles.

Everything else is as in 0.1.14.

[Back to the list of versions](#versions)

---

<a name="v0-1-14"></a>
## 0.1.14 — 2026-10-04

A guided tour for first-time users, and a demo master to try it on.

### Licensing

- **Unchanged.** This build is wrapped with soundBlade's product licence, so a
  soundBlade iLok unlocks it exactly as before.

### First-run tour

- **The first time the Player opens, a short tour walks through the window**,
  part by part from the top left: the part being described is highlighted in
  gold, with a card explaining it — Back, Next and Skip Tour (arrow keys,
  Return and Esc work too). Parts not on screen are skipped.
- **Help > Show Tour** runs it again at any time.

### Demo master

- **"Deep Note" by James Andy Moorer**, six channels, is built in. The tour's
  first page offers to open it, and **Help > Open Demo Master** does at any
  time.

### For testers

- Hover anything in the Player — tooltips now work throughout (since 0.1.13).
- To see the tour again as a new user would, use Help > Show Tour.

Everything else is as in 0.1.13.

[Back to the list of versions](#versions)

---

<a name="v0-1-13"></a>
## 0.1.13 — 2026-10-03

Checking a stereo album: lists, metadata, DDEX and loudness that stays with the file. And tooltips — the Player never showed any until now.

### Licensing

- **Unchanged.** This build is wrapped with soundBlade's product licence, so a
  soundBlade iLok unlocks it exactly as before.

### Artist Connection

- **The cloud button opens your studio's library as a tab**, where the file
  list is. Every format streams — WAV, FLAC, MP4, Auro-Cx and ADM — and a
  download is offered, never required.
- **Upload files and create albums** from the Player.

### Lists

- **Save List** saves the list, with its Featured and Skip ticks; **Open** asks
  whether to replace the list or add to it, and opens a saved list or an EDL.
- Remove from List removes every selected row, without a question.
- Drop a folder to add the audio files in it (not its sub-folders).

### Stereo files

- A simpler window: no F/Skip columns, no Source button, and **Binaural is a
  choice in the Monitor menu**, which stops at Stereo. The object view folds
  away, and the Monitor meters hide when they would only repeat the Desk.

### Metadata and DDEX

- **Drop a CSV, TXT, TSV or Excel sheet to import it.** Rows match files by
  ISRC, by name, or by track number; review, then **Import All** or **Import
  ISRC Only**. Album fields come in where a column repeats the album on every
  row.
- **Album Info** (button beside Export, or right-click the cover): the album's
  details, including a **description** and its **delivery layout** (e.g.
  Binaural).
- **Drop a DDEX message** to replace the list with its whole release.
  **Export > DDEX never asks for a layout** — two channels are Stereo unless
  the file or the album says otherwise.
- **Drop an image on the cover square** to use it.
- Removing the last file asks whether to delete the album info too.
- Hover a file to see its whole name; hover the room for how to rotate it.

### Loudness and level

- **Measure saves its figures with the file** and shows them whenever the file
  is selected, until the file changes. Save to File writes them into a WAV's
  bext.
- **The main volume fader shows what is going out**, after the fader.
- **The SR lamp lights green when the file is sample-rate converted.**
- The bar beside the Desk can be dragged to move the loudness figures right.

### Fixes

- **Tooltips now show** — the Player had no tooltip window, so none ever did.
- **Auro binaural was silent** — fixed.
- Fixed a crash pressing Import in the DDEX report.

### For testers

- Drop a folder of stereo masters and its spreadsheet; check every row
  matches, Import All, then Export > DDEX.
- Measure a file, select another, come back — the figures should read
  "measured" with the date.
- Hover the buttons and the loudness block — every one should explain itself.

Everything else is as in 0.1.12.

[Back to the list of versions](#versions)

---

<a name="v0-1-12"></a>
## 0.1.12 — 2026-09-28

Cleaner starts for streamed masters, and Channel Based monitoring that really claims nothing.

### Licensing

- **Unchanged.** This build is wrapped with soundBlade's product licence, so a
  soundBlade iLok unlocks it exactly as before.

### Artist Connection

- **Streams start cleanly.** A streamed master now buffers about three seconds
  before it plays, and the Player says "Buffering the stream…" while it does,
  instead of starting in silence or breaking up in the first seconds.
- **ADMs, MP4, Auro-Cx and IAMF files ask before downloading.** They cannot be
  streamed — they need the whole file — so the Player now asks "download to
  play?" rather than starting a download on its own.
- **Download icons.** Every playable row in the Library shows whether the file
  is on this Mac: an arrow (not downloaded), a ring (downloading) or a tick
  (downloaded). Streamed rows in the file list show the arrow too.

### Monitoring

- **Channel Based now claims nothing.** Choosing Channel Based in the Monitor
  menu used to keep the previous layout underneath — its speaker map and its
  loudness weighting went on applying. Now the channels go out exactly as they
  are, one per output with no fold, while the Desk, the monitor meters and the
  Out column keep the file's own width. Patching a row's output in Channel Based
  moves only that channel.

### For testers

- **Artist Connection:** double-click a WAV in the Library — you should see
  "Buffering the stream…" briefly, then clean playback from the first second.
- **Double-click an ADM** in the Library: it should ask before downloading.
- **Channel Based:** open a 5.1 or 7.1.4 file, choose Monitor > Channel Based.
  Every channel should play on its own output, the monitor meters should show
  the file's full width, and re-patching one row in the Out column should move
  only that channel.
- **If you still hear breakup**, please send the log
  (`~/Library/Logs/Sonic Reference Player/`), your interface, buffer size and
  sample rate.

Everything else is as in 0.1.11.

[Back to the list of versions](#versions)

---

<a name="v0-1-11"></a>
## 0.1.11 — 2026-09-27

Artist Connection: open masters straight from your studio's library.

### Licensing

- **Unchanged.** This build is wrapped with soundBlade's product licence, so a
  soundBlade iLok unlocks it exactly as before.

### Artist Connection

- **File > Artist Connection…** opens your studio's media Library. Sign in
  with your Artist Connection studio admin account (the same one soundBlade
  uses); the approval happens in your browser.
- **Double-click a file to play it.** It streams straight away — the row says
  "streaming" and plays as one row carrying all its channels.
- **Right-click a streamed row > Download** brings the original file onto this
  Mac. Once it lands, the same row becomes a normal master: one row per
  channel, the overview, Auro-3D decoding, cover and metadata. Downloaded
  files open instantly next time, with no network.
- **ADMs, MP4 and Auro-Cx files download rather than stream** — they need the
  whole file. Progress and Cancel are in the Artist Connection window.
- **Settings > Clear Downloads** frees the space; the list keeps the masters
  and streams them again.
- The Library is read-only here: nothing in the Player can change the studio's
  files.

### Monitoring

- **Binaural on an Auro-3D file keeps all its channels.** The rows stay at the
  decoded layout (12 for 7.1.4) and only the monitor becomes the headphone
  pair, rendered by Auro's own binaural renderer.
- **Apple Spatial Audio** is a new binaural renderer choice in Settings, beside
  Auro and SOFA.
- **"Custom" is shown** on the Monitor button when the speaker-to-output map is
  hand-built, and the Monitor menu has a **Custom** item to bring it back. The
  Speaker Layout dialog agrees with the button.

### The window

- **Drag bar between the file list and the Layout list** — drag to resize the
  file list, double-click to reset. The waveform (Overview) column is the one
  that grows.
- The Featured column is gone (the Player never opens masters into an EDL);
  ADM and Name get its space.
- **Measure** fills the loudness rows with the measured figures, and an ADM's
  own declared loudness is shown where it states one.
- **Double-click a file to play it**, again to stop.
- Icons on Open, Video and Binaural; bigger triangles; the object view folds
  away; removing a file asks first.
- **Help > Sonic Reference Player Guide** opens the user guide.
- Waveform caches are one folder beside each file instead of one file per
  channel.

### For testers

- **Artist Connection:** sign in, double-click a stereo or 7.1.4 WAV — it
  should play within a few seconds. Then Download it and check the rows split
  per channel.
- **Try an ADM** from the Library: it should download, then open as usual.
- **Binaural on an Auro master:** 12 rows, two monitor meters.
- **If you still hear breakup**, please send the log
  (`~/Library/Logs/Sonic Reference Player/`), your interface, buffer size and
  sample rate.

Everything else is as in 0.1.10.

[Back to the list of versions](#versions)

---

<a name="v0-1-10"></a>
## 0.1.10 — 2026-09-26

Steadier playback, from the engine the Player shares with soundBlade.

### Licensing

- **Unchanged.** This build is wrapped with soundBlade's product licence, so a
  soundBlade iLok unlocks it exactly as before.

### Playback

- **No silent gaps when the disk falls behind.** If the read-ahead has not
  reached the part of a file that is about to play — a slow drive, a very
  wide file, a seek — the Player now reads that audio directly from the file
  instead of playing silence in its place. The read-ahead also runs further
  ahead (about a second) and keeps its place when the list changes.
- The log (`~/Library/Logs/Sonic Reference Player/`) notes how often this
  happened in a pass, so a slow drive shows up as a number rather than as a
  dropout.

### For testers

- **Play a wide master** (7.1.4, an ADM, an Auro carrier) and **seek around
  quickly**. There should be no dropouts to silence.
- **If you still hear breakup**, please send the log, your interface, buffer
  size and sample rate.

Everything else is as in 0.1.9.

[Back to the list of versions](#versions)

---

<a name="v0-1-9"></a>
## 0.1.9 — 2026-09-24

DDEX arrives, plus a tidier button row.

### Licensing

- **Unchanged.** This build is wrapped with soundBlade's product licence, so a
  soundBlade iLok unlocks it exactly as before.

### DDEX (ERN 4.3)

- **Export... now asks: CSV or DDEX.** DDEX writes an ERN 4.3 release
  message from the list: each file is one recording, in list order, its
  metadata record the track and the album record the release. Files that
  share a **Track** number are one song in different layouts, and each layout
  is its own recording with its own ISRC.
- **Before it writes**, it lists anything the release is missing — album
  title, artist, UPC, label, genre, release date (YYYY-MM-DD); per file a
  title, an ISRC and a Layout — and writes nothing until it is complete.
- Sender and recipient, each with an **optional DDEX Party ID** (without one
  the message carries `PADPIDAUNASSIGNED`, fine for internal use). **"Copy
  audio and artwork into the delivery folder"** is off unless you tick it.
- **Import... now also takes a DDEX `.xml`**, even on an empty list. It checks
  the message and every file it names — references, UPC and ISRC check
  digits, track order, files present, MD5 checksums, and each file's channels,
  rate, bit depth and duration against the message — and shows a **report**
  you can save. **Add to List**, only when there are no errors, brings the
  files in and writes a metadata record beside each.
- **Edit Metadata** has a new **Track** and **Layout** row. Layout (Stereo,
  5.1, 7.1.4, Auro-3D, Auro-Cx, Binaural) fills itself only when the file says
  what it is; a binaural file is two channels like stereo, so that one is
  yours to set.

### Button row

- Source, Binaural and Monitor now sit on the bottom row under the meters
  they set, full height. The window cannot be made narrow enough for them to
  overlap.

[Back to the list of versions](#versions)

---

<a name="v0-1-8"></a>
## 0.1.8 — 2026-09-23

A small follow-up to 0.1.7.

### Licensing

- **Unchanged.** This build is wrapped with soundBlade's product licence, so a
  soundBlade iLok unlocks it exactly as before.

### Cover images

- **An X to remove a chosen cover.** A cover image you chose now shows a small
  **X** in its top-right corner — click it to remove the image. A file's own
  artwork, or a `cover.jpg` beside it, is not something the Player can delete,
  so it shows no X.

Everything else is as in 0.1.7 — see its notes for the metadata, import /
export and cover work.

[Back to the list of versions](#versions)

---

<a name="v0-1-7"></a>
## 0.1.7 — 2026-09-23

Metadata you can see, import and export, an album cover, and the Player's own icon.

### Licensing

- **Unchanged.** This build is wrapped with soundBlade's product licence, so a
  soundBlade iLok unlocks it exactly as before.

### Metadata

- **Each file's metadata in the list.** A triangle on each file opens a line
  under it with its title, artist, ISRC and ISWC. Click again to close it.

- **Kept beside the file, not in it.** A file's metadata is kept in a small
  record beside it (`<file>.sbmeta.xml`), so it travels with the file. Files
  exported from soundBlade with Create Tracks from Marks arrive with theirs.
  **Edit Metadata**'s **Save** writes the record and never changes the audio;
  **Save to File** also writes the tags into the file, and **ISRC Only**
  writes just the ISRC.

- **Import… from CSV or Excel.** Reads a CSV or an Excel workbook (.xlsx) onto
  the files in the list — the track list is found wherever it is, and each row
  is matched to its file by ISRC or by the track number the file name starts
  with. **You review the matches before anything is written.** A UPC a
  spreadsheet rounded to `6.09E+11` is refused with the reason, and text
  garbled by the wrong encoding is repaired.

- **Export…** writes the list's metadata as a CSV that Import reads back.

- **Edit Metadata** steps through the list with **Prev / Next**, and **Save**
  turns yellow while there are unsaved edits.

### Album cover

- **The cover is shown beside the loudness read-outs**: the file's own artwork,
  else an image you choose (click the square), else a `cover.jpg` beside the
  file. Under it: the image's size, its data size and where it came from.

### Look

- **The Player has its own icon**, so it can be told apart from soundBlade.
- The loudness read-outs are narrower, with Reset and Measure under the title,
  and the Binaural button sits on the Monitor row.

### For testers

1. **Open a row's triangle** on files exported from soundBlade, and on files
   with no metadata.
2. **Import a label's CSV or workbook**, review the matches, and open the rows.
3. **Click the cover square** on a file with no artwork and choose an image.

None of this changes audio. It is covered by soundBlade's in-app test suite,
which the two applications share, and by nothing else.

[Back to the list of versions](#versions)

---

<a name="v0-1-6"></a>
## 0.1.6 — 2026-09-22

A Speakers page, speaker naming in SMPTE or ITU-R, a Room view seen from the listener's seat, and diffuse objects heard as diffuse.

### Read this first

**The breakup reported against the 0.1.4 test build has not been reproduced**,
and the leading explanation is another application taking the audio device.
If you hear the audio break up, please report it with the machine, the
interface, the device buffer size, the sample rate, and whether 0.1.3 does the
same on the same file. `~/Library/Logs/Sonic Reference Player/` holds the log,
which records under-runs and their cause; please attach it.

### Licensing

- **Unchanged.** This build is wrapped with soundBlade's product licence, so a
  soundBlade iLok unlocks it exactly as before.

### Speakers

- **Settings has a Speakers tab.** The layout, the channel order, the speaker
  naming and the output each speaker plays from, on one page — the same page
  soundBlade has in Project Settings. It edits the same settings as the
  window's own Speaker Layout dialog.

- **Speaker naming: SMPTE or ITU-R.** Speakers can be named the familiar way
  (L R C LFE Lss Rss Ltf …) or by ITU-R BS.2051 position (M+030 M-030 M+000
  LFE M+090 U+045 …). Set it with **Naming** on the Speakers tab or in the
  Speaker Layout dialog. It changes labels only — never routing or audio. The
  master meters always keep SMPTE names; the monitor meters follow the
  setting.

- **A file that names its channels is believed.** A WAV or FLAC that declares
  its speakers (its channel mask) now gets those names, and its layout comes
  from the declaration instead of being guessed from the channel count — the
  only way to tell ten channels of 7.1.2 from ten of 5.1.4. Each named channel
  plays to the speaker it names, so a WAV-order 7.1 — rears before sides —
  reaches the right speakers.

- **A 5.1.4 was shown and played as 7.1.2**, including a 5.1.4 Auro decode.
  Fixed.

- **The Speaker Layout dialog** now applies a change to a single speaker's
  output. Before, only picking a whole layout took effect.

- **The monitor meters scroll** when they do not all fit beside the fader, as
  the master meters do. A 7.1.4 monitor used to be cut off unless the window
  was widened.

### Object audio

- **The Room view is seen from the listener's seat.** The front of the room is
  now the far wall and the rear the near one, looking down towards the front
  as from a theatre seat, with **FRONT** marked on the front wall under the
  centre speaker. It used to be drawn back to front. The flat Front and Side
  views were corrected the same way.

- **Diffuse objects sound diffuse.** An object an ADM declares as diffuse is
  now rendered that way — decorrelated across the speakers — instead of as a
  hard point. Two commercial Atmos releases tested here declare most of their
  objects fully diffuse, so this is audible on real masters. Measured loudness
  follows it too.

### For testers

1. **Does the audio break up?** See "Read this first" — a clean report is as
   useful as a broken one.
2. **Open Settings > Speakers** and try Naming; check the labels change where
   you expect and nowhere else.
3. **Open the Room view** and check it reads the right way round — front far,
   L on the left.
4. **Play an ADM with diffuse objects** and compare against 0.1.5.

None of this has had a listening test here; it is covered by soundBlade's
in-app test suite, which the two applications share, and by nothing else.

[Back to the list of versions](#versions)

---

<a name="v0-1-5"></a>
## 0.1.5 — 2026-09-22

Object metadata and object timing, on top of the audio-engine corrections that were staged as 0.1.4 and never published.

### Read this first

**0.1.3 is the last build known to play cleanly.** A build made from the
engine work in this release broke up badly on playback here, and the cause has
not yet been found. soundBlade's matching release was withdrawn for the same
reason. This build is going out so the problem can be characterised on more
than one machine — not because it is believed fixed.

**If you hear the audio break up, that is the thing to report**, with the
machine, the interface, the device buffer size and the sample rate, and
whether 0.1.3 does the same on the same file. `~/Library/Logs/Sonic Reference
Player/` holds the log, which records under-runs and their cause; please
attach it.

### Licensing

- **Unchanged from 0.1.3.** This build is wrapped with soundBlade's product
  licence, so a soundBlade iLok unlocks it exactly as before. The player's own
  separate licence was prepared and then reverted — it is still coming, but it
  is not in this build. (The 0.1.4 notes, which were written and never
  shipped, said the opposite.)

### Object audio

- **An imported ADM keeps its objects' size.** Every object's `width`,
  `height`, `depth`, `diffuse` and divergence was being read from the file and
  then dropped on the way into the timeline, so an object arrived as a bare
  point. Anything that wrote the file back out then wrote those lost values
  over the originals as zeros. They now survive.

  Note this is metadata, not yet sound: the renderer still plays every object
  as a point source, so a wide object is not yet heard as wide. What changes
  today is that the file's description of it stops being destroyed.

- **Object moves happen when the file says they happen.** An ADM states where
  an object arrives and how long the move takes; we were reading that as the
  moment the move *begins*, which put every imported trajectory up to one
  metadata block early — around 20 ms on a typical master, and a whole block
  wherever the blocks are longer.

- **A move that the file says is instant is now instant.** Where a file states
  a short interpolation and then a hold — a common authoring convention, and
  the one the THX reference master uses — the object moved over the whole
  block instead, smearing a 5 ms step across 20 ms. It now moves over the
  stated time and holds.

  Objects you position by hand are unaffected and still glide between their
  keyframes, which is what that gesture means.

### Playback

The player shares its engine with soundBlade, so the corrections staged as
1.1.87 are here too.

- **Nothing left over when the playhead jumps.** The delay lines that keep
  everything in time were fed only while playing and never cleared, so
  pressing Play or seeking began with a fragment of whatever was last heard.
  Both those lines and the plug-ins' own internal buffers are now cleared at a
  transport jump.

- **A moving object no longer steps.** The panner read an object's position
  once per audio block and held one gain across the whole of it — at a
  1024-sample buffer that is a step every 10 ms, and each step is a click.
  Position and gain now update every 64 samples and ramp between. A stationary
  object costs exactly what it did before.

- **Playback and export agree about time.** Positions were rounded down to the
  sample in playback where an export rounds to the nearest, so material could
  sit one sample earlier in what you heard than in what you printed.

### For testers

In priority order:

1. **Does the audio break up?** See "Read this first". This is the question
   that matters most, and a clean report is as useful as a broken one — please
   say either way, and say what you played.

2. **Play an ADM with moving objects and compare against 0.1.3.** Object
   motion should now sit very slightly later than it did, and land where the
   file says. Anything that sounds like it drifts, lags or jumps wrongly is
   worth reporting.

3. **Confirm your existing soundBlade licence still unlocks the player.** It
   should — nothing about the wrap changed in this build.

4. **A fast object move is worth a listen**, and so is starting playback part
   way into a file.

- No part of this release has had a listening test here. The object timing and
  metadata work is verified by soundBlade's in-app test suite, which the two
  applications share, and by nothing else. The import has not been run against
  a real ADM file carrying sized objects.

[Back to the list of versions](#versions)

---

<a name="v0-1-4"></a>
## 0.1.4 — 2026-09-21

The audio-engine corrections from soundBlade 1.1.87, and the player's own licence.

### Licensing

- **The player now has its own product licence.** Up to 0.1.3 it was wrapped
  with soundBlade's, so a soundBlade iLok unlocked both. It no longer does:
  this build needs a licence issued for the Sonic Reference Player itself.

### Playback

The player shares its engine with soundBlade, so every correction in
soundBlade 1.1.87 is here too.

- **Nothing left over when the playhead jumps.** The delay lines that keep
  everything in time were fed only while playing and never cleared, so
  pressing Play or seeking began with a fragment of whatever was last heard.
  Both those lines and the plug-ins' own internal buffers are now cleared at a
  transport jump.

- **A moving object no longer steps.** The panner read an object's position
  once per audio block and held one gain across the whole of it — at a
  1024-sample buffer that is a step every 10 ms, and each step is a click.
  Position and gain now update every 64 samples and ramp between. A stationary
  object costs exactly what it did before.

- **Playback and export agree about time.** Positions were rounded down to the
  sample in playback where an export rounds to the nearest, so material could
  sit one sample earlier in what you heard than in what you printed.

### For testers

- **Confirm the player launches at all.** With a new licence and a new wrap,
  that is the one thing worth checking first — a mismatch stops the app before
  it opens a window, with nothing written to the log.

- **A fast object move is worth a listen**, and so is starting playback part
  way into a file.

- Nothing in this release has had a listening test. It is verified by
  soundBlade's in-app test suite, which the two applications share.

[Back to the list of versions](#versions)

---

<a name="v0-1-3"></a>
## 0.1.3 — 2026-09-21

Auro-Cx playback, and the window remembering itself.

### Auro-Cx

- **Auro-Cx files open and play.** This is a different format from the Auro-3D
  carrier the player already read: a carrier is ordinary PCM with its height
  channels hidden in the low bits, while **Auro-Cx is a coded bitstream** in an
  `a3ds` track described by an `acxd` box, meaningless until a Cx decoder has
  had it.

  Nothing in macOS can open one — both AVFoundation and CoreAudio refuse the
  container — so this uses Auro's own MP4 parser and Cx engine end to end.

- **The layout comes from the file.** A 5.1 master opens as 5.1, a 7.1.4 one as
  7.1.4: the decoder is asked what the content *is*, not what it can render to.

- **Seeking is exact**, re-priming from 32 access units earlier — measured
  against real files rather than guessed.

### The window

- **It remembers its size and position.** Every launch used to centre it at a
  fixed size. A position saved on a monitor that is no longer attached is
  ignored rather than leaving the window somewhere you cannot see it.

- **A video window you closed stays closed.** Opening a file that carries
  picture shows the picture — but closing that window is a decision, and it now
  survives a relaunch. Asking for it again through File > Open Video brings the
  automatic behaviour back.

- **The monitor meters show the right number straight away.** They were correct
  but drawn inside a strip sized for the previous count, so the window could
  open showing two.

- **The Monitor read-out says when the device has narrowed the layout**, as
  `5.1 → Stereo`.

- **Quitting no longer reports a leak.** The background waveform scan pool was
  never shut down in this application.

### For testers

- **Auro-Cx is new and has had one day of use.** The decode was measured; the
  reader around it is a day old. Anything that sounds wrong is worth reporting
  at once.

- **A note for Auro:** the Cx components in the SDK drop we hold work as
  documented. What is not clear from the package is whether our existing
  agreement covers *shipping* them — the drop is named "Passthrough", which is a
  narrower thing than decoding. We would like that confirmed.

[Back to the list of versions](#versions)

---

<a name="v0-1-2"></a>
## 0.1.2 — 2026-09-20

Two corrections to 0.1.1's MP4 support, found by testing it against a real set of video files.

- **Dolby soundtracks are named properly.** A 5.1 film mix delivered as Dolby
  Digital Plus was labelled `EC-3`, which is its four-character code and tells
  you nothing. Rows now read **Dolby Digital Plus** and **Dolby Digital**, and
  HE-AAC is named too. A codec still not recognised keeps its four-CC — that
  says the file can be read and its name was not recognised, rather than
  inventing one.

- **A lossless track reports the depth it was written at.** A 24-bit FLAC
  inside an MP4 read `FLAC 48/32` — 32 being the depth the player decodes to,
  which describes the player rather than your file. It now reads `FLAC 48/24`,
  taken from what the file itself declares.

  A lossy track has no source depth to report, so it still says "lossy" with no
  number.

[Back to the list of versions](#versions)

---

<a name="v0-1-1"></a>
## 0.1.1 — 2026-09-20

Video files, an About window, and updates where you would look for them.

### Video and MP4

- **Open an MP4 and hear it.** Raw PCM, FLAC and ALAC inside an MP4 are read
  **bit-exactly** — nothing on the path converts through floating point, which
  is what lets an **Auro-3D carrier inside a video file** decode properly. AAC
  is supported too and is **labelled "lossy"**, since what it cannot be is a
  master.

- **The picture opens with it.** A file that carries video shows its own video
  window, muted — what you hear is the decoded audio through this app's engine,
  not the movie's own playback.

- **The file row names the codec, not the extension.** ".mp4" tells you nothing
  about what is inside; a row now reads `PCM 48/24`, `FLAC 96/24` or
  `AAC 48 lossy`.

- **Channel names come from the file.** A file that declares what its channels
  are gets real speaker names; one that declares nothing gets `Ch 1..N`.
  Nothing is reordered — a file that lists rears before sides keeps that order,
  and the Out column re-patches it.

### The window

- **Binaural is a button you can see**, under the loudness read-outs, lit when
  it is on. It was a checkbox positioned past the edge of its column — invisible
  since it was added — so only the menu item ever worked. The Monitor read-out
  also says `7.1.4 → Binaural` while it is on: binaural monitoring is a stereo
  pair, so two monitor meters beside a box reading "7.1.4" looked exactly like
  a fault and was not one.

- **About Sonic Reference Player**, in the application menu, with the version
  you are running.

- **Check for Updates has moved into Settings**, beside the running version —
  which is what every update comparison is made against, so "why was I not
  offered X" is answerable without asking anyone.

- **"Add Files..." is now "Open..."**, and it offers every format the
  application can actually read rather than a fixed list — which is how `.mp4`
  appears in it at all.

- **File > Open Video...** shows the picture for the selected master, or points
  it at a different cut.

### For testers

- MP4 support is new. The decode was checked against independent decoders — raw
  PCM against the file's own bytes, FLAC against ffmpeg — and seeking is
  sample-exact, but **the reader has had one day of use**. Anything that sounds
  wrong in an MP4 is worth reporting straight away.

- A FLAC inside an MP4 reports its bit depth as 32, which is the depth it is
  decoded to rather than the depth it was written at. Cosmetic today; it will be
  read properly from the file.

- **This build still ships with soundBlade's licence identity**, so one licence
  unlocks both applications.

[Back to the list of versions](#versions)

---

<a name="v0-1-0"></a>
## 0.1.0 — 2026-09-20

The first build. Sonic Reference Player opens masters, tells you what they are, and plays them correctly on whatever rig you are sitting in front of. It is soundBlade's Preview window as an application of its own: the same engine, the same decoders, the same metering — with no EDLs, no editing and nothing to accidentally change about the file you were sent.

### What it does

- **Open any number of masters and compare them.** ADM (BW64), Auro-3D
  carriers, and plain multichannel PCM — WAV, FLAC, AIFF, RF64, W64. Drag them
  in, or File > Add Files.
- **See what the file actually is** before you trust it: sample rate, bit
  depth, duration, start timecode, channel count, bed and object counts, and
  the loudness it declares.
- **Play it on the layout it was made for**, or on the one you have. Pick the
  Source layout the material IS and the Monitor layout you are LISTENING on,
  and it folds between them.
- **Meter it properly** — a Desk strip with one column per channel, monitor
  meters showing what reaches the device, and true-peak/loudness read-outs.
- **Watch the objects move**, for an ADM master, in the object view.
- **Listen on headphones** with binaural monitoring.

### Auro-3D

- **An Auro-3D carrier is detected and decoded on open.** A carrier hides its
  height channels inside an ordinary 5.1 or 7.1 PCM stream, so an 8-channel
  file opens as the twelve channels it really holds — not as eight.
- The decode happens at the reader, so the channel list, the waveforms, the
  meters and playback all see the real thing.
- **On headphones, an Auro master is rendered by Auro's own engine**, not by
  ours, so it is spatialised once and by the renderer that made it.

### Channel Based, and not inventing names

- **A file that does not say what its channels are is listed as `Ch 1..N`.**
  Eight channels could be 7.1 or 5.1.2 and the file does not say, so the
  Player does not guess. Speaker names appear where the file actually supports
  the claim — an ADM's beds and objects, or an Auro carrier stating its layout.
- **"Channel Based"** in the monitor menu means exactly that: no layout
  claimed, no fold, each channel straight out to its own output.

### Your room

- **Click a row's Out column to send it to a different output.** Useful when a
  rig is not wired in layout order, and the only way to patch an unlabelled
  multichannel master.
- **Speaker Layout…** does the same thing for a whole layout at once.
- Both are remembered, because they describe the room rather than the file.
- **Audio I/O…** picks the device, rate and buffer size.

### Binaural

- **Auro renders it, by default.** For headphone monitoring the Player uses
  Auro's own renderer — the same engine that decodes Auro masters, and the
  path Auro's encoder itself offers for 7.1.4.
- **An Auro master always uses Auro's renderer**, whatever this is set to. It
  is already binaural by the time it is decoded, and rendering it again would
  spatialise it twice.
- **SOFA (HRTF)** is the alternative: our own convolution, using an HRTF file
  you supply. It works for any layout with directions, including ones Auro
  does not carry — and if the Source layout is one Auro cannot render, the
  Player falls back to it and tells you so in Settings.

### Settings

- **Binaural renderer** — Auro or SOFA (HRTF).
- **The HRTF** used by the SOFA renderer. One ships with the Player; load your
  own `.sofa` if you have one. Not used while Auro is the renderer, and shown
  as unavailable then rather than looking live.
- **Check for Updates**, and whether to check on launch.

### Known limitations

- **It cannot share an audio interface with soundBlade.** Both open the
  device; whichever gets there first keeps it. Run one at a time, or give
  them different devices.
- **Its settings are its own**, separate from soundBlade's, with the
  deliberate exception of the HRTF choice — that describes your ears and your
  room, so both applications follow it.
- **Nothing here writes to your files.** The Player reads. Edit Metadata is
  the one exception and it asks first.

### For testers

The things most worth breaking:

- **Binaural on a layout Auro does not carry** — it should fall back to SOFA
  and say so in Settings, not go quiet or render something it should not.
- **Binaural loudness against the speaker render.** Toggling it should not
  jump in level, and should not clip.

- Open a master whose layout your device cannot carry — a 7.1.4 file on an
  8-output interface. It should fold to something the device can play and say
  what it is doing, not play to outputs that are not there.
- Mute and unmute channels while it plays, in any order.
- Re-patch outputs with the Out column, then check the file still plays to
  where you put it after reopening.
- Compare an Auro carrier against the same material decoded elsewhere.

Please report what you were doing, what you expected and what happened.

[Back to the list of versions](#versions)

---
