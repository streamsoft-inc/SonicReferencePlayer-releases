# Sonic Reference Player — Release Notes

Every release, newest first. Each links to its full notes below.

<a name="versions"></a>
## Versions

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
