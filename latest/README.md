# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **1.2.11**

- **Page 5 no longer gets stuck "finding the video stream".** If reading a clip straight from the link stalls, ClipForge stops it after 40 seconds and downloads the video once instead, the same way it got your video in the first place. Looking up the link has a time limit, and a download that stops moving is abandoned after 2 minutes with a clear message, so nothing can hang forever.
- **Cancel works immediately**, even while ClipForge is waiting on the internet.
- **The timer on page 5 keeps counting**, and shows "waiting N s" when a step is waiting on the internet.
- **Activity log:** each step, the video streams chosen, and any download or FFmpeg error are written to `logs\activity.log` in the ClipForge data folder (%APPDATA%\ClipForge), so a problem can be traced.
