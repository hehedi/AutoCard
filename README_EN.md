[简体中文](README.md) | [English](README_EN.md)

# AutoCard · AutoPlay

**From media offload and verified backups to transcoding, review, and playback.**

[Download the latest release](../../releases) · [AutoPlay overview (Chinese)](https://www.bilibili.com/opus/1261109162464509972) · [License](LICENSE)

Free to use · Windows / Linux · macOS support in development · Chinese / English

## AutoCard

| Feature | What it does |
| --- | --- |
| **Offload & organize** | Identify devices and media from multiple cameras on one card; import by media type or copy the full card; organize by project, camera position, and card ID. |
| **Verification & backup** | Multiple backup destinations, incremental imports, duplicate detection, and disk-space checks; import verification, pre-deletion checks, and selectable verification modes. Retain source media if destination files have issues. |
| **Task management** | A shared queue for offload and transcoding jobs, with concurrency control, resumable transfers, task recovery after a restart, and task status viewing over the LAN. |
| **Transcoding & proxies** | Hardware acceleration, HDR → SDR, color conversion, LUT application, and loudness normalization; custom presets and parameters; automatic proxy generation and linking. |
| **Toolbox** | On-set automatic imports, batch image/audio/video conversion, frame extraction, and audio extraction; modular tool extensions. |
| **Logs & reports** | Search, filter, and inspect operation logs; choose a custom or network log folder; automatically generate an Excel report after each offload. |

Transcoding uses the bundled FFmpeg / ffprobe, with encoding options including H.264 / H.265 / H.266 / VP9 / AV1.

![AutoSD main interface](docs/images/主界面.png)

## AutoPlay

Bundled with AutoCard and can be launched separately for footage review and everyday media playback.

- **Multi-format playback**: Video, audio, images, and camera RAW, with support for DSD, embedded/external subtitles, and exclusive audio device access.
- **Frame-by-frame review**: Frame stepping, precise time entry, timecode, frame capture, and markers; zoom, pan, reduced-resolution playback, and dropped-frame diagnostics.
- **Video and audio analysis**: Luminance waveforms, histograms, white balance analysis, audio waveforms, and spectrum views; video scopes can be overlaid on the image.
- **A/B comparison**: Dual-view, single-view, and difference modes, with separate or linked playback, drag-and-drop media replacement, and captured-frame comparison.
- **Display and color controls**: Apply and compare custom LUTs, adjust HDR brightness and SDR luminance mapping, and choose whether picture cropping also affects subtitles.

**Quick preview from your memory card**: In AutoSD's media browser, hover over a media thumbnail, **hold Space to preview, and release to close**.

[Full AutoPlay overview and demos (Chinese) →](https://www.bilibili.com/opus/1261109162464509972)

## More screenshots

<details>
<summary>Completed offloads & logs</summary>

![Offload completion screen](docs/images/完成界面.png)

![Operation logs](docs/images/日志.png)

After each offload, the project folder contains an Excel report named `[日期][项目名]_导出详情.xlsx` (date + project name + export details). It records camera positions, card IDs, media counts, total size, destination paths, file status, and other details.

</details>

<details>
<summary>Transcoding, LUTs & task details</summary>

![Transcoding](docs/images/转码.png)

![LUT application](docs/images/LUT还原.png)

![Transcoding task details](docs/images/转码详情.png)

</details>

<details>
<summary>Media browser & quick preview</summary>

![Media browser details](docs/images/素材浏览器详情.png)

![Media browser quick preview](docs/images/素材浏览器快速预览.png)

</details>

<details>
<summary>Toolbox & automatic imports</summary>

![Toolbox](docs/images/工具箱界面.png)

![Automatic imports](docs/images/在线导入.png)

</details>

## Languages & license

Chinese and English are included. Add language files to the application's `language` folder to support additional languages.

This is **proprietary software**; its source code is not publicly available. See [`LICENSE`](LICENSE) for usage and distribution restrictions.

> Keep independent backups of important media, and verify that your backups are complete before deleting the originals.

Copyright © 2026 **hehedi**. All Rights Reserved.
