# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **2.0.6**

- Fixed: with **Gemini**, planning a video stopped with "'str' object has no attribute 'values'". Gemini "thinks" before it answers, and that thinking used up the room ClipForge gave each answer, so the script plan came back cut off. Online AI now gets room to think, and a cut-off answer is asked again with more room. The backup script writer that then crashed is fixed too.
- Fixed: with a long prompt, the main window became taller than the screen and its bottom (CREATE, Number of clips, Projects…) went under the Windows taskbar. Every page now scrolls when it doesn't fit, so the window always fits your screen.
