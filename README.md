# ShotMarker — High-Performance Pre‑Production Video Logger and Database Builder

ShotMarker is a fast, streamlined pre‑production tool for building local, easy‑to‑search video databases designed as a replacement for the pre-production workflow in Adobe Premiere Pro. It’s designed to make logging b‑roll and assembling selects frictionless — even across dozens of projects and tens of thousands of clips. Most importantly, it allows you to build large databases of footage that is fast, optimized, filterable and searchable across projects.

## Why ShotMarker

- Speed: MPV with GPU acceleration provides great scrubbing and playback performance.
- Focus: Optimized UI/UX streamlines tagging, in/out marking, and sequence assembly.
- Scale: SQLite + FTS5 full‑text search enable fast cross‑project queries over large libraries, allowing you to search and find footage across all your projects in your database.
- Portability: exports highly compressed local previews so you can preview footage anywhere without needing access to raw footage that could be spread out between many drives.

## Core Features

- Tagging System: apply, search, and preset tags; organize b‑roll by client, topic, or any taxonomy.
- Cross‑Project Database: search across multiple projects with combined tag and title filtering.
- MPV Playback: hardware‑accelerated playback (when supported), exact seeks, and responsive scrubbing.
- FFmpeg Export: create lightweight preview proxies (H.264/HEVC), native MOV, or ProRes; optionally store in/out only.
- Premiere Integration:
  - Drag‑and‑drop markers into Premiere; in/out points, names, and tags come along.
  - Generate importable Premiere sequences (XMEML/FCP XML) from selected markers.
  - Export in/out directly into .prproj files and add DVA‑style markers (project processing + repack supported).
- Localized Media Previews: auto‑export compact per‑marker clips on creation, turning e.g. 300 GB of raw into ~50 MB of previews for quick sharing or on‑the‑go review.
- Thumbnails & LUTs: capture thumbnails via FFmpeg, with optional LUT application.

## Designed for Scale

- Search Across Everything: query by title, tags, favorites, across many projects.
- Fast Data Access: SQLite schema with indexes and FTS5 keeps interactions snappy.
- Supports hardware-accelerated decoding, including H265 4:22 on latest generation nvidia cards.
- Hardware‑Aware Exports: detects NVENC/QSV/AMF to accelerate H.264/HEVC proxy creation.

## Typical Workflow

1. Add footage folders to a project and start playback.
2. Mark in/out points and apply tags and titles.
4. Drag markers or generated sequences into Premiere to start cutting immediately.
5. Search across projects to pull matching b‑roll for repeat clients or build reels.


## Installation
Download the latest release here: https://github.com/delisimedia/Shot-Marker/releases


## Notes

- Drag‑and‑Drop: Alt‑drag from ShotMarker to import into Premiere where supported.
- Database: local SQLite per project; cross‑project views let you query multiple projects at once.
- Performance: MPV options favor fast seeks/hardware decode; FFmpeg exports select hardware encoders when available.

## Acknowledgements

- MPV (libmpv)
- FFmpeg / FFprobe
- SQLite / FTS5
- PyQt6, lxml, OpenCV

---

ShotMarker replaces the slow, manual pre‑production logging stage with a high‑performance, organized system that gets you into the edit faster.
