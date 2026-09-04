# Sonora — Install

Native multi-source music, podcasts and audiobooks for macOS.
## Install

1. Open the `.dmg`.
2. Drag **Sonora** onto the **Applications** folder.
3. Eject the disk image.

## First launch (important)

This build is **ad-hoc signed, not notarized**, so Gatekeeper will refuse to
open it the normal way the first time. Do one of the following — **once**:

**Option A — right-click**
Open your Applications folder, **right-click** (or Control-click) *Sonora* →
**Open** → **Open** in the dialog. macOS remembers this and it launches normally
after that.

**Option B — Terminal**
```sh
xattr -dr com.apple.quarantine /Applications/Sonora.app
```

If macOS says *"Sonora is damaged and can't be opened"*, that's Gatekeeper on an
un-notarized app — use Option B, it clears it.

## Requirements

- **macOS 26 (Tahoe) or later.**
- **`yt-dlp`** for reliable YouTube playback:
  ```sh
  brew install yt-dlp
  ```
  Without it, YouTube still searches but only embeddable videos play. Keep it
  updated (`brew upgrade yt-dlp`) — YouTube breaks it periodically.

## What you get

Search across YouTube, SoundCloud and internet radio at once · podcast directory
+ RSS · audiobooks from RSS or a local folder (resume, speed, skip) · playlists,
incl. import from a Spotify / Apple Music share link · immersive Now Playing with
synced lyrics & transcripts · media keys, Control Center, and a menu-bar
mini-player · queue that survives relaunch.

Open **Settings** (⌘,) to set default podcast speed, skip intervals, and to clear
caches.

## Notes

- Personal-use tool. It reaches several services in ways their terms don't
  strictly allow (YouTube extraction, a scraped SoundCloud key, Spotify/Apple
  page scraping for playlist import). Nothing is redistributed; no accounts, no
  telemetry.
- Everything it stores is local metadata in `~/Library/Preferences` — no media,
  no tokens.
- To remove: drag `Sonora.app` to the Trash and,

<img width="1272" height="872" alt="Screenshot 2026-09-04 at 8 11 48 PM" src="https://github.com/user-attachments/assets/2c4695df-7716-41a3-a867-18fc2ea6e654" />
<img width="1272" height="872" alt="Screenshot 2026-09-04 at 8 11 45 PM" src="https://github.com/user-attachments/assets/98d17c6e-51c7-419d-bfcc-391b668d64b1" />
<img width="1272" height="872" alt="Screenshot 2026-09-04 at 8 11 28 PM" src="https://github.com/user-attachments/assets/6e6dc05f-2ebf-4edc-9bdd-8d1a902d7739" />
<img width="1272" height="872" alt="Screenshot 2026-09-04 at 8 11 25 PM" src="https://github.com/user-attachments/assets/de095361-5a3b-450f-a158-7ad13d0cb5e7" />
<img width="1272" height="872" alt="Screenshot 2026-09-04 at 8 10 32 PM" src="https://github.com/user-attachments/assets/5bb3b20c-d8c6-4f1b-80ec-49ca6278ab8e" />
<img width="1272" height="872" alt="Screenshot 2026-09-04 at 8 10 27 PM" src="https://github.com/user-attachments/assets/0c937b3b-335a-4f4c-87cb-63631afee65a" />
