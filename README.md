# Play-Multi-Videos
Play multiple Videos Side by side , Speed Up Slow Down Zoom etc etc Binge Watch multiple movies TV episodes etc.. at the same time

# Scan · Select · Play — User Manual
_Media Matrix Viewer using VLC_

---

## 1. Overview

**Scan · Select · Play** is a multi-pane video matrix viewer powered by VLC.

You can:

- Scan large media folders
- Filter and sort by title / year
- Select multiple videos
- Open them in a grid (matrix) and play them simultaneously
- Double-click any pane to zoom it fullscreen inside the app
- Adjust playback speed, volume, and audio source globally

---

## 2. Main Window (Library)

### 2.1 Screen Layout

```text
+----------------------------------------------------------------------------------+
| Scan • Select • Play – Media Matrix                                             |
+----------------------------------------------------------------------------------+
| Media Library                 [Scan Library] [Open in Matrix] [Settings]         |
+----------------------------------------------------------------------------------+
| ① Pick source  ·  ② Scan Library  ·  ③ Filter & select  ·  ④ Open in Matrix     |
+----------------------------------------------------------------------------------+
| Library                                                               |          |
| ┌──────────────────────────────────────────────────────────────────────────────┐ |
| | Source folder: [ C:\Movies\FeatureFilms                 ] [Browse…] [Rescan] | |
| | Filter: [ matrix ]                      [Title ↑▼]         128 item(s)      | |
| └──────────────────────────────────────────────────────────────────────────────┘ |
|                                                                                |
| ┌──────────────────────────────────────────────────────────────────────────────┐ |
| | The Matrix (1999)                                                           | |
| | The Matrix Reloaded (2003)                                                 | |
| | The Matrix Revolutions (2003)                                              | |
| | Inception (2010)                                                           | |
| | Interstellar (2014)                                                        | |
| | ...                                                                        | |
| └──────────────────────────────────────────────────────────────────────────────┘ |
| Status: Scan complete. Select items and open in Matrix.                        |
+----------------------------------------------------------------------------------+

2.2 Steps to Use the Library Screen

Pick Source Folder

Use Browse… to choose your main media folder (e.g. F:\Media\Movie).

Or type/paste the path into Source folder.

Click Scan Library or Rescan.

Scan Library

A Scanning… dialog appears with a Cancel button.

The app recursively finds all video files with allowed extensions.

Files with unwanted words (e.g. “trailer”, “extras”, “featurette”) in their name are filtered out.

Filter & Sort Results

Use the Filter box to search by title or year:

Examples: matrix, 2014, avatar.

Use the sort dropdown:

Title ↑ / Title ↓

Year ↑ / Year ↓

The info label on the right shows: N item(s).

Select Videos

Use Ctrl+Click or Shift+Click to select multiple titles.

Or use right-click context menu on the list:

Toggle Select

Select All Visible

Clear Selection

Open Selected in Matrix

Open in Matrix

Select up to MAX_PREVIEW_PANES items.

Click Open in Matrix.

A new Matrix Viewer window opens.

3. Matrix Viewer (Multi-Pane Playback)
3.1 Screen Layout

Example with 2 panes (2×1), but layout scales to 1, 2, 4, 9, 12, 16 panes:

+----------------------------------------------------------------------------------+
| VLC Matrix Viewer — The Matrix.mkv | Inception.mkv                              |
+----------------------------------------------------------------------------------+
| [⏯ Play / Pause] [🔇 Mute All]   Audio from: [1: The Matrix]   Rate: [-][1.00×][+]|
+----------------------------------------------------------------------------------+
| Position: [==== global seek slider =====================]   Volume: [===slider==]|
+----------------------------------------------------------------------------------+
| [ Video: The Matrix (1999) — 1920×1080 • 3.4 GB • A2/S1 ]                       |
| +------------------------------------------------------------------------------+ |
| |                                                                              | |
| |                        (pane 1 video area)                                   | |
| |                                                                              | |
| +------------------------------------------------------------------------------+ |
| [ Video: Inception (2010) — 1920×800 • 4.1 GB • A3/S0 ]                         |
| +------------------------------------------------------------------------------+ |
| |                                                                              | |
| |                        (pane 2 video area)                                   | |
| |                                                                              | |
| +------------------------------------------------------------------------------+ |
+----------------------------------------------------------------------------------+
| Shortcuts: Space=Play/Pause   [ / ]=Rate ±5%   \=Reset   Esc=Exit pane fullscreen|
+----------------------------------------------------------------------------------+

3.2 Global Controls

Top bar:

⏯ Play / Pause

Toggles playback for all videos at once.

Keyboard: Space.

🔇 Mute All

Immediately mutes audio on all panes.

Audio from: [ pane ]

Only one pane provides audio output.

Select which video should be heard (others stay muted).

Rate:

−: slower by 5% (keyboard: [).

1.00×: reset playback rate to normal (keyboard: \).

+: faster by 5% (keyboard: ]).

Numeric field: type precise rates (e.g. 0.75, 1.25, 2.0).

Bottom bar:

Position slider:

Scrubs all videos to the same relative position.

Drag and release to seek.

Volume slider:

Global volume (0–100) applied to all VLC players.

4. Individual Panes & Fullscreen Zoom
4.1 Pane Layout

Each pane shows its own title and metadata:

┌ Video: Inception (2010) — 1920×800 • 4.1 GB • A3/S0 ┐  ← Title & metadata
│                                                      │
│     (VLC-rendered video area: double-click anywhere) │
│                                                      │
└──────────────────────────────────────────────────────┘


Title bar contents:

Video:

Parsed title and year (from filename)

Resolution (width×height)

File size (e.g. 3.4 GB)

Stream counts: A# = audio, S# = subtitles

Hover over the pane to see a tooltip with:

Title

Path

Approx. resolution & stream counts

4.2 Fullscreen per Pane (Zoom)

You can zoom any pane to fullscreen within the app:

Enter fullscreen:

Double-click anywhere inside the pane:

on the title bar, or

on the video area, or

on the black background inside the pane.

The Matrix Viewer switches to a single-pane layout:

+-------------------------------------------------------------------------------+
| VLC Matrix Viewer — The Matrix.mkv                                           |
+-------------------------------------------------------------------------------+
| [⏯] [🔇]  Audio from: [1: The Matrix]   Rate: [-][1.00×][+]                  |
+-------------------------------------------------------------------------------+
| Position: [===============]   Volume: [========]                             |
+-------------------------------------------------------------------------------+
| [ Video: The Matrix (1999) — 1920×1080 • 3.4 GB • A2/S1 ]                    |
| +---------------------------------------------------------------------------+ |
| |                                                                         | |
| |                    (single fullscreen pane)                             | |
| |                                                                         | |
| +---------------------------------------------------------------------------+ |
+-------------------------------------------------------------------------------+
| Shortcuts: Space=Play/Pause   [ / ]=Rate ±5%   \=Reset   Esc=Exit fullscreen |
+-------------------------------------------------------------------------------+


Exit fullscreen:

Double-click again inside the fullscreen pane, or

Press Esc.

Switch fullscreen pane:

Exit fullscreen and double-click a different pane, or

If a pane is fullscreen and you return to grid, just double-click another pane.

5. Keyboard Shortcuts

In the Matrix Viewer:

Space — Play/Pause all videos

[ — Slow down playback by 5%

] — Speed up playback by 5%

\ — Reset playback rate to 1.0×

Esc — Exit pane fullscreen (back to matrix)

6. Settings Dialog

Open Settings from the main window.

6.1 Screen Sketch
+-------------------------------- Settings -------------------------------------+
| Source folders (one per line):                                               |
| ┌─────────────────────────────────────────────────────────────┐               |
| | F:\Media\Movie                                             |               |
| | G:\External\Anime                                          |               |
| └─────────────────────────────────────────────────────────────┘               |
| Exclude keywords:      [ trailer, sample, extras, featurette ]               |
| Video extensions:      [ mp4, mkv, avi, mov, webm ]                          |
| Max preview panes:     [ 12 ]                                                |
|                                                                            |
| Default playback speed:     [ 1.00 ]                                        |
| Default volume (0–100):     [ 80 ]                                          |
| Default audio pane (1=first): [ 1 ]                                         |
| [x] Start playback automatically when matrix opens                          |
|                                                                            |
|                                 [  OK  ]   [ Cancel ]                       |
+-------------------------------------------------------------------------------+

6.2 Editable Options

Library:

Source folders (one per line).

Exclude keywords (comma-separated).

Video extensions (comma-separated).

Max preview panes (1–32).

Player defaults:

Default playback speed.

Default volume.

Default audio pane (1 = first pane).

Autoplay when matrix opens.

Settings are saved in a JSON file (scan_select_play_config.json) and loaded automatically.

7. Typical Workflow

First run

Launch Scan_select_play.py.

Open Settings and configure:

Source folder(s)

Max preview panes

Default speed & volume

Scan library

From main window:

Confirm source folder.

Click Scan Library or Rescan.

Wait for scan to complete (or cancel early).

Filter & select

Filter by title/year.

Sort results as needed.

Select multiple entries (Ctrl+Click, Shift+Click, or Select All Visible).

Open in Matrix

Click Open in Matrix.

A Matrix Viewer window opens with your selection.

Control playback

Use Play/Pause, Rate, and Volume controls.

Choose which pane’s audio is active.

Zoom in on a video

Double-click wherever you want on that pane.

Watch fullscreen inside the app.

Double-click again or press Esc to return to matrix.

8. Notes & Best Practices

For very large libraries, the scan may take time:

Use specific source folders.

Adjust exclude keywords to skip unwanted material.

Metadata (resolution, size, streams) is only probed for videos that you open in the matrix, not for the entire library.

Works great for:

Comparing different cuts / versions

Viewing scene coverage

Monitoring multiple camera angles

Analyzing security or test footage in parallel


