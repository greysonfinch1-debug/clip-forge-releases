# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **1.2.7**

**Edit & Captions (page 5)**
- **Build edit** now also renders the preview, so the video appears without a second click.
- **Any changes?** understands general requests such as "make it cooler", "make it better" or "more hype", even without Ollama. It switches to another hook, speeds the voice up slightly, makes the captions bigger and uses snappier cuts, then lists each change. Undo puts it all back.
- Fixed garbled text (`&#x27;`, `&quot;`) in the Any changes? results.
- If a preview can't play inside the app, ClipForge now says so and points you to **Open externally** instead of showing an empty area.
- Includes 1.2.6's fix for Shorts made from video links ("ffmpeg is not installed"), which also stopped the preview and the captions from building.
