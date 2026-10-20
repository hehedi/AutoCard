[English](README_EN.md) | [Chinese](README.md)

# One-Click Card Import AutoSD / One-Click Playback AutoPlay

**A media import and processing tool for photography, videography, and post-production workflows.**
**Comes with a highly professional and efficient player**

**The software includes English and makes it easy to add multiple languages; simply place a language file into the software's language folder**

One-Click Card Import was initially created to solve the problem of organizing, copying, and archiving footage from storage cards after shooting. Through continuous development, it has now become a tool that integrates **device identification, verified backup, multi-tasking, transcoding, media browsing, and professional playback**.

---

## Core Features

### Card Import

![Main interface](docs/images/主界面.png)

A media import workflow designed for camera cards and recorder cards.

* Automatically identify manufacturer, model, serial number, and camera position
* Support media files, video-only, photos, audio, and full-disk import modes
* Support incremental import and duplicate media detection
* Support resumable transfers and recovery of unfinished tasks
* Support multiple destination export and backup
* Support mixed-card identification and archiving by camera model
* Support archiving information such as project name, camera position number, and card number

### Media Safety

![Completion interface](docs/images/完成界面.png)

The card import process is designed around "**media can be confirmed, source files are not accidentally deleted**" as much as possible.

* Check destination disk space before import
* File import verification and duplicate media detection
* Pre-check before deletion, with multiple verification modes
* Automatically retain source media when destination files are abnormal
* Provide detailed reasons when import fails
* Generate export records after import completes

Duplicate detection uses information such as file name, size, and quick hash; stricter content verification can be used when performing safe deletion.

### Camera Identification

Determine device models through comprehensive evidence from multiple media sources.

For storage cards that have not been reformatted and have been used with different cameras successively, mixed-card identification and model arbitration are also supported, and media is archived according to the identification result.

Unknown devices will not be forcibly matched to an incorrect model; when identification cannot be confirmed, original information is retained as much as possible.

---

## Multi-Task Queue

Card import and transcoding tasks all enter the task queue.

Supports:
* Parallel multi-tasking
* Concurrency control
* Queued scheduling
* Task recovery after program restart
* Task completion summary
* LAN task status viewing

---

## Transcoding

![Transcoding](docs/images/转码.png)
![LUT Restoration](docs/images/LUT还原.png)

Built on bundled FFmpeg / ffprobe.

Supports:

* H.264 / H.265 / H.266 / VP9 / AV1 and other encodings
* Hardware encoding acceleration
* Basic encoding adjustment options
* HDR → SDR
* Color space conversion
* Audio loudness normalization
* LUT restoration
* Custom FFmpeg parameters
* Custom presets

![Transcoding details](docs/images/转码详情.png)

Also provides a proxy workflow:

* Automatically generate Proxy folders
* Associate proxy files with original media

---

## Media Browser / One-Click Playback AutoPlay

![Media browser details](docs/images/素材浏览器详情.png)

After inserting a storage card, you can directly browse the media on the card.

**Comes with a professional player**
**For more detailed features, please visit [bilibili]: https://www.bilibili.com/opus/1261109162464509972**

---

## Quick Preview

![Media browser quick preview](docs/images/素材浏览器快速预览.png)

The media browser provides a quick browsing method for on-site shot selection:

**Move the mouse over a media card → hold Space**

to preview quickly.

---

## Toolbox

![Toolbox interface](docs/images/工具箱界面.png)

The toolbox uses a modular design.

Tools are loaded as independent modules and can be added or removed without affecting the core functions of the main program.

Currently provides:

### Online Import

![Online Import](docs/images/在线导入.png)

Used for automatic card import on set.

### Quick Format Conversion

Used to quickly convert image, audio, and video formats.

Supports corresponding target formats based on media type, and provides batch processing, frame extraction, audio extraction, and other functions.

---

## Logs and Archiving

![Logs](docs/images/日志.png)

The software records major business operations, including:

* Import
* Import history
* Transcoding
* Deletion
* Deletion of original media after transcoding
* Import failure
* Related operation results

Logs support:

* Search
* Filtering
* Pagination
* Detail viewing
* Custom log directory
* Network shared log directory

After each card import completes, the following is also maintained in the project directory:

```text
[日期][项目名]_导出详情.xlsx
```

Used to record information such as project, date, export time, camera, camera position, card number, number of media files, total capacity, destination location, and file status.

---

## Performance and Reliability

The software has been specifically designed for large amounts of media, long-running tasks, and abnormal interruptions.

Includes:

* Large directory virtualization
* Thumbnail loading and caching based on viewport
* Background media scanning and metadata reading
* Task state persistence
* Atomic disk writes and backup recovery
* Resumable transfers
* Task recovery after abnormal exit
* Separation of technical logs and business logs

In actual tests, the interface remains interactive even when a large amount of media is present at the same time.

---

## Download

Go to GitHub Releases to get the latest version:

[Releases](../../releases)

Currently mainly provides the **Windows version**.
**The Linux version has been developed and runs normally, and is undergoing reliability testing**

This project is currently **closed-source software**, and the source code is not publicly available.

---

## System Requirements

The software currently targets the Windows desktop environment.
However, Mac and Linux versions are also within the development scope.

Some system runtime components are provided with the program package. During installation, if it detects that the computer does not have these components, it will automatically install them.

---

## License

### One-Click Card Import

One-Click Card Import itself is **Proprietary Software**.

```text
Copyright © 2026 hehedi. All Rights Reserved.
```

Except for the usage rights explicitly granted by this project, all copyrights and other intellectual property rights are reserved.

Without the written permission of the copyright owner, you may not:

* Copy or re-publish this software
* Modify or create derivative versions
* Decompile, disassemble, or attempt to obtain the source code
* Remove or modify copyright and rights notices
* Repackage this software as another product for distribution
* Sell, rent, sublicense, or provide unauthorized commercial redistribution

For the complete license terms, please refer to:

[`LICENSE`](LICENSE)

---

## Disclaimer

This software is used to assist with the import, organization, and processing of photography and videography media.
Although the software has designed corresponding protection mechanisms for import verification, abnormal recovery, safe deletion, and other situations, any storage device, operating system, file system, USB interface, and third-party media components may encounter unforeseen problems.
For important footage, it is recommended to always keep an independent backup and delete the original media only after confirming that the backup is complete.
Please do not upload files containing personal privacy, project privacy, or unreleased footage.

Designed by **hehedi**
Copyright © 2026 hehedi. All Rights Reserved.
