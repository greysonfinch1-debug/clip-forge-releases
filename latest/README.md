# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **2.0.4**

- Fixed: with **Gemini** (or another online AI) chosen in Settings, ClipForge stopped using Ollama for **meaning search** and **frame descriptions**, even when Ollama was running. It fell back to plain word matching and no frame descriptions. They now always use Ollama on your PC, whichever AI writes the scripts.
- The AI Models page shows Ollama's real status and downloads its models correctly while Gemini is selected.
- When a script can't be written, the message now gives the real reason, for example "no language model is selected" or "the API key was rejected". Before, it always said Ollama wasn't running.
