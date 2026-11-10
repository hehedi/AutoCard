[简体中文](README.md) | [English](README_EN.md)

# AutoCard

**Import, verify, back up, transcode, and review your media—from memory card to organized project archive.**

[Download the Latest Release](../../releases) · [AutoPlay](https://github.com/hehedi/AutoPlay) · [AutoLibrary](https://github.com/hehedi/AutoLibrary) · [License](LICENSE)

Free to use · Works offline · Windows / Linux · Chinese / English

AutoCard is designed for video production, photography, and audio recording workflows. It identifies media on storage devices, organizes files by date, project, camera, and card number, backs up to multiple destinations, and keeps verification results and task reports.

![AutoCard main window](docs/images/主界面.png)

## Key Features

| Feature | Description |
| --- | --- |
| **Card Offloading & Organization** | Identifies cameras and storage devices, and recognizes cards containing media from multiple sources. Import selected media types or all files on a device, organized by date, project, camera, and card number. |
| **Verification & Backup** | Supports multiple backup destinations, incremental imports, duplicate checks, and available-space checks. Verifies file contents with xxHash (default), MD5, or SHA-256, and performs additional checks before deleting source files after offloading. If a check finds an issue, the affected source files are retained and the reason is shown. |
| **Task Management** | Manage offload and transcoding tasks in one queue, with concurrency controls, pause and retry, resumable offloads, and recovery of eligible transcoding tasks. View task status across the same local network. |
| **Transcoding & Proxies** | Hardware acceleration, HDR → SDR conversion, color conversion, LUT processing, and loudness normalization. Customize presets and parameters, and generate proxy files linked to their source media. |
| **Media Browser** | Browse, search, and filter media on a card; inspect shooting parameters and media information. Hold Space for quick previews, capture frames, and mark media items. |
| **Toolbox** | Live ingest on set, batch conversion for images, audio, and video, frame and audio extraction, and support for modular extensions. |
| **Logs & Reports** | Search and filter operation logs, view detailed entries, and store logs locally or on network shares. Generate PDF task reports after offloading, with media details, verification results, archive locations, and deletion records. |

## Media Browser

Hover over an item in the media browser and hold **Space** to preview it. You can also keep the preview open, capture frames, and mark media items.

- **Professional Media Playback**: Play professional media such as MXF, ProRes, BRAW, R3D, and ARRIRAW / ARRICORE, view camera RAW photos, and inspect shooting parameters and media metadata.
- **Frame-Accurate Review**: Step forward or backward one frame at a time, use SMPTE timecode and precise seeking, and capture frames. Choose full-resolution playback or reduced-resolution modes to inspect detail or reduce playback load.
- **LUT & HDR Preview**: Apply LUTs to preview color transforms, with support for HDR display, brightness adaptation, and HDR → SDR mapping. Preview adjustments do not modify the source media.
- **A/B Comparison**: Compare originals, proxies, and differently processed versions using reference images or videos, an adjustable split view, side-by-side comparison, frame alignment, and a difference view.
- **Video & Audio Analysis**: Inspect exposure, color, and sound with a luma waveform, RGB histogram, white balance aids, and per-channel audio waveforms and spectrograms.

## Download & Installation

1. Download a version from [Releases](../../releases). See its release notes for supported platforms.
2. For the Windows installer, keep `Setup.exe` and its matching `Setup-1.bin` data file from the same release in the same folder, then run `Setup.exe`.
3. Select AutoCard, AutoPlay, and the components you need during installation. Some professional decoders and additional features are provided as optional components. All components are free; install only what you need to save disk space.

## More Screenshots

<details>
<summary>Completed Offloads & Logs</summary>

![Offload completion screen](docs/images/完成界面.png)

![Operation logs](docs/images/日志.png)

After an offload, a PDF task report is generated in the project folder. It includes an import summary, media thumbnails, technical parameters, verification results, and full destination paths, and records subsequent deletion operations.

</details>

<details>
<summary>Transcoding, LUTs & Task Details</summary>

![Transcoding](docs/images/转码.png)

![LUT processing](docs/images/LUT还原.png)

![Transcoding task details](docs/images/转码详情.png)

</details>

<details>
<summary>Media Browser & Quick Preview</summary>

![Media browser details](docs/images/素材浏览器详情.png)

![Quick preview in the media browser](docs/images/素材浏览器快速预览.png)

</details>

<details>
<summary>Toolbox & Live Ingest</summary>

![Toolbox](docs/images/工具箱界面.png)

![Live ingest](docs/images/在线导入.png)

</details>

## Languages & License

Chinese and English are included. Add language files to the application's `language` folder to enable additional languages.

This software is **free to use under a proprietary license; its source code is not publicly available**. See [`LICENSE`](LICENSE) for usage and distribution restrictions. Third-party license notices are available on the application's About page and in the included license files.

> Keep independent backups of important media. Verify that your backups are complete before deleting the original files.

Copyright © 2026 **hehedi**. All Rights Reserved.
