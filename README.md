# DICOM Extracts and 4D Visualization Gallery

A collection of images generated across other projects: DICOM images extracted from source series, and the 4D visualizations built from them.

- **Maintainer:** Shrushrita Sharma, Personal Project
- **Last updated:** 2026-10-09
- **Status:** Draft template. Replace every `<placeholder>` before use.

> **Data handling note:** Only de-identified images belong in this gallery. Confirm that burned-in annotations and DICOM header fields (patient name, ID, birth date, accession number) have been removed before adding an image.

---

## 1. Purpose and scope

This document frames the images in one place so each can be understood without opening the project that produced it. It covers two kinds of material:

1. **Extracted DICOM images:** 2D slices or frames exported from DICOM series.
2. **4D visualizations:** renderings that combine three spatial dimensions with time (X, Y, Z + t).

Out of scope: `<anything excluded, e.g. raw DICOM files, PHI-bearing data, unreleased builds>`.

---

## 2. How to read the 4D visualizations

Each 4D visualization maps four dimensions onto what you see. Unless a caption says otherwise, use the default mapping below.

| Dimension | Default meaning | Shown as |
|-----------|-----------------|----------|
| X | `<e.g. lateral position, mm>` | `<e.g. horizontal axis of each frame>` |
| Y | `<e.g. vertical position, mm>` | `<e.g. vertical axis of each frame>` |
| Z | `<e.g. depth / slice index>` | `<e.g. slice slider or stacked volume>` |
| t | `<e.g. acquisition time or frame index>` | `<e.g. animation playback or time slider>` |

Intensity and colour: `<e.g. grayscale window/level, colour map, what colour encodes>`.

Orientation convention: `<e.g. LPS / RAS, anatomical labels shown or not>`.

---

## 3. Source projects

| ID | Project | What it contributed | Link / location |
|----|---------|---------------------|-----------------|
| P1 | `<project name>` | `<e.g. extracted DICOM slices>` | `<path or URL>` |
| P2 | `<project name>` | `<e.g. 4D volume renders>` | `<path or URL>` |
| P3 | `<project name>` | `<...>` | `<path or URL>` |

---

## 4. Gallery: extracted DICOM images

### IMG-001: `<short title>`

![<alt text describing the image>](<relative/path/to/image-001.png>)

- **Source project:** `<P1: project name>`
- **Caption:** `<one or two sentences on what the image shows>`
- **Notes:** `<observations, window/level used, known artifacts, limitations>`

### IMG-002: `<short title>`

![<alt text>](<relative/path/to/image-002.png>)

- **Source project:** `<...>`
- **Caption:** `<...>`
- **Notes:** `<...>`

<!-- Copy the IMG block above for each additional image. -->

---

## 5. Gallery: 4D visualizations

### VIS-001: `<short title>`

![<alt text>](<relative/path/to/vis-001.gif>)

- **Source project:** `<P2: project name>`
- **4D axis mapping:**
  - X: `<...>`
  - Y: `<...>`
  - Z: `<...>`
  - t: `<...>`
- **Caption:** `<what the viewer should notice as time advances>`
- **Notes:** `<frame rate, number of time points, rendering method, limitations>`

### VIS-002: `<short title>`

![<alt text>](<relative/path/to/vis-002.gif>)

- **Source project:** `<...>`
- **4D axis mapping:**
  - X: `<...>`
  - Y: `<...>`
  - Z: `<...>`
  - t: `<...>`
- **Caption:** `<...>`
- **Notes:** `<...>`

<!-- Copy the VIS block above for each additional visualization. -->

---

## 6. Suggested folder layout

```
gallery/
├── DICOM_4D_Visualization_Gallery.md
├── images/
│   ├── img-001.png
│   └── img-002.png
└── visualizations/
    ├── vis-001.gif
    └── vis-002.gif
```

Keep image paths relative so the markdown renders correctly on GitHub and in other viewers.

---

## 7. Adding a new image

1. Confirm the image is de-identified.
2. Save it under `images/` or `visualizations/` with the next sequential ID.
3. Copy an IMG or VIS block and fill in source project, caption, and (for 4D) the axis mapping.
4. Add the source project to the table in section 3 if it is new.
5. Update the **Last updated** date at the top.

---

## 8. Change log

| Date | Change | By |
|------|--------|----|
| 2026-10-09 | Initial template created | Shrushrita |
