# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **1.2.6**

**Fixes**
- Exporting a Short made from a **video link** failed with "You have requested downloading the video partially, but ffmpeg is not installed". The video downloader now finds ClipForge's built-in FFmpeg. Shorts made from video files on your PC were not affected.
