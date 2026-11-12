# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **1.2.10**

- **Page 5 now actually makes your Short from a link, and much faster.** Clips from YouTube, Twitch and Kick links were being re-encoded in a very slow format while downloading (about one frame per second), so "Building your Short and its preview…" could sit for a very long time and sometimes failed. ClipForge now reads just the seconds it needs and starts each clip exactly on the right frame. If a site won't allow that, it downloads the video once, keeps it, and cuts every clip from that copy.
- **A progress bar on page 5.** While your Short is being made you see each step (getting the clips, recording the narration, laying out the edit, rendering the preview) and how far along it is, with a **Cancel** button. If something goes wrong, the reason now shows where the video would be, instead of the page staying stuck.
