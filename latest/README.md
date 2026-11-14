# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **1.5.0**

**Faster**
- Reopening a project or making a new video from an analysed one no longer waits for AI models it doesn't need.
- The first analysis of a video runs speech and pictures at the same time.
- AI models stay loaded between steps (unless your PC is short of memory, or you chose Low resource).
- The language model stays loaded in Ollama between steps and starts loading while you type your prompt.
- No more network checks for the picture model once it's downloaded.
- Rendering is quicker, with the same final quality settings.

**Production brief**
- Before making the video, the AI turns your prompt into a detailed production brief: the kind of video, hook, parts and talking points, what to show, ending, editing, narration and captions, and which facts must be checked. You see it as it's written, can edit it, ask for another, or skip it.
- Your prompt itself is never changed. The video, the script and the footage follow the brief you approve.
- Without Ollama running, ClipForge tells you why and how to fix it, and lets you continue with your prompt as typed.
- Your video is analysed while the brief is written, so no time is lost.
- Settings → Prompt expansion turns it off, or uses the brief without asking.
