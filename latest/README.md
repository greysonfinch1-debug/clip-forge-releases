# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **1.2.9**

**Better Shorts**
- **Clips no longer open on the wrong scene.** A clip could start with a second of whatever came before it (a different game scene, a menu), and the footage under the narration could cross into it too. ClipForge now finds scene changes (ignoring flashing lights, explosions and camera moves) and starts the clip on the right side of them, unless someone is talking across the change.
- **Bigger captions** that are easier to read on a phone. A caption that wouldn't fit on one line is shrunk to fit. If you set your own caption size, it's kept.
- **Two people talking are told apart properly.** Speaker detection could put two different people under one label. Each voice now gets its own caption colour, and the person who talks most keeps the main colour.
- **Silent pauses are cut out.** A long pause inside a clip (nobody talking, nothing happening) is tightened with a quick jump cut, the way an editor would. It never cuts the key moment, and you can turn it off on page 5.
- **"After this clip" narration lines** now play right after that clip. Before, every such line was moved to the very end of the Short.

**Fixes**
- Exporting failed for anyone whose Windows user name (or folder) contains an apostrophe, bracket or comma, such as *O'Neil*.
- Videos recorded on a phone and stored sideways failed to export.
- OBS recordings with several audio tracks: the transcript and the Short now always use the same (first) track.

**For testing**
- New `clipforge-cli fieldtest` runs a list of your permitted recordings from start to finish and saves everything to a `ClipForge_Test_Results` folder: the chosen clips, the Shorts, quality reports, a frame-by-frame contact sheet, a loudness graph, timings and memory use. `clipforge-cli review` checks one finished Short. See TESTING_WINDOWS.md.
- The model check now also tests the narration voice and whether speaker detection can tell two voices apart.
