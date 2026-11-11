# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **1.2.2**

**New: fully automatic updates**
- ClipForge downloads and verifies new versions in the background while you work. The update installs the next time you open ClipForge.
- A yellow **"Restart to finish"** button lets you install it straight away if you prefer.
- To go back to one-click updates, untick **About & Updates → Install updates automatically**.
- ClipForge now checks for updates every time it opens. Before, it waited 6 hours between checks.
- Updates now come from the `updates` branch of your releases repository, which Claude publishes to directly. There are no files to upload yourself. Releases still work as a fallback.

**Security**
- ClipForge now verifies updates with a new signing key. The previous key was retired after it was accidentally published.
