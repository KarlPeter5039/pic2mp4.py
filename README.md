# Pic2MP4

A Python tool for converting folders of images into cinematic MP4 slideshow videos with intelligent sequencing modes.

Designed for photographers, film scans, travel imagery, and Instagram reel-style exports.

---

# Features

* Convert image folders into MP4 videos
* Supports:

  * JPG / JPEG
  * PNG
  * TIFF / TIF
* Automatic EXIF orientation correction
* Configurable output width
* H.264 MP4 export
* 1-second-per-image slideshow generation
* Multiple intelligent image sequencing modes

---

# Sequencing Modes

## 1 — Filename Order

Preserves chronological or filename-based order.

Best for:

* travel sequences
* documentary work
* film roll continuity

---

## 2 — Alternating Luminance

Alternates bright and dark images for stronger visual rhythm.

---

## 3 — Smooth Luminance Flow

Sorts images from darker → brighter for cinematic pacing.

---

## 4 — Output All Versions

Exports all sequencing modes automatically.

---

## 5 — RGB Balanced Sequencing

Balances:

* red-heavy images
* green-heavy images
* blue-heavy images
* black & white images

while also dispersing:

* portrait images
* landscape images

---

## 6 — Hue-Angle Balanced Sequencing

Advanced editorial sequencing using HSV hue clustering.

Distributes:

* reds
* oranges
* yellows
* greens
* cyans
* blues
* purples
* magentas
* black & white frames

for smoother visual variety.

---

## 7 — Filename + Balanced Sequence

Outputs both:

* filename_order
* balanced_sequence

simultaneously.

---

# Folder Structure

Input folders should be placed inside the `input/` directory.

Example:

```text
input/
├── iceland_trip/
│   ├── DSC001.jpg
│   ├── DSC002.jpg
│   └── DSC003.jpg
│
├── desert_roll/
│   ├── IMG001.tif
│   ├── IMG002.tif
│   └── IMG003.tif
```

The program automatically generates:

```text
output/
├── iceland_trip_filename_order.mp4
├── iceland_trip_balanced_sequence.mp4
├── desert_roll_filename_order.mp4
├── desert_roll_balanced_sequence.mp4
```

---

# Installation

## 1. Clone Repository

```bash
git clone https://github.com/yourusername/pic2mp4.git
cd pic2mp4
```

---

## 2. Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Usage

Place image folders inside:

```text
input/
```

Then run:

```bash
python pic2mp4.py
```

Generated videos will appear in:

```text
output/
```

---

# Adjustable Settings

Inside the script:

```python
SECONDS_PER_IMAGE = 1
FPS = 30
OUTPUT_WIDTH = 1080
ORDER_MODE = 7
```

---

# Requirements

* Python 3.10+
* FFmpeg installed and available in PATH

---

# FFmpeg Installation

## Windows

Download:
https://ffmpeg.org/download.html

Add FFmpeg to your system PATH.

---

# Example Use Cases

* Instagram reels
* Film photography slideshows
* Travel sequences
* Portfolio presentation videos
* Cinematic image pacing
* Gallery projection exports

---

# Future Ideas

Potential future additions:

* Beat-synced sequencing
* Motion transitions
* Ken Burns pan/zoom
* AI-based image pacing
* Audio/music integration
* Dominant palette sequencing
* Contrast-aware sequencing

---

# License

MIT License
