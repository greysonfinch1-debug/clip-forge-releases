# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **1.2.12**

- **A clip that downloads too slowly is now caught too.** In 1.2.11 the safety stop only triggered if reading from the link showed no activity at all. Now it also triggers when the clip stops moving forward for 40 seconds, or is crawling along at less than 1 second of video every 5 seconds. ClipForge then downloads the video once at full speed instead.
