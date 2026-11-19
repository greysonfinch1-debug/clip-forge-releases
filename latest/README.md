# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **2.0.3**

- Fixed: clips could come out **with no sound** after a YouTube download was interrupted.
- Fixed: switching to another video or project while the first was still being analysed could mix up their analysis.
- Fixed: exporting twice within the same minute **replaced the first export**. Each export now keeps its own file.
- Fixed: with transitions turned off, exports failed if a folder name had an apostrophe (e.g. `Zoë O'Neil`).
- Fixed: Cancel didn't respond while waiting to retry an online AI service (Gemini and others).
- Settings that would make the render or AI calls fail (for example 0 fps) are now corrected automatically.
- Half-finished temporary files are cleaned up properly, and no background FFmpeg is left running after a crash.
- Also includes 2.0.2: a one-click "Use Gemini" button in Settings, Paste/Show buttons for the API key, and more accurate scripts (research stays on topic, prices must come from the right item, hooks are written fresh).
