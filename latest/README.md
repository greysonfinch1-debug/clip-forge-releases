# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **1.4.0**

**Three kinds of video**
- **Clip-driven** (as before): moments from your footage tell the story.
- **Narration-driven** (new): the narration tells the story, and footage is picked to go with each part of it. For explainers, lists, documentaries, news-style reports, commentary, stories, even a poem.
- **Hybrid** (new): real moments with their own sound, plus narrated parts over supporting footage. For example, open with a real moment, explain something, cut to the real reactions, end strong.
- Just describe the video in the prompt box. ClipForge works out which kind it is, the style, pacing and subject, and step 2 says what it understood. You can also set the type, style and pacing yourself.

**Footage that fits the narration**
- The picture model (CLIP) matches every second of your footage to the meaning of each part of the narration. The footage doesn't have to show exactly what's said, just something that fits.
- Within a part, the shots follow the narration in order, and the picture changes at the end of a sentence.
- Shots never cross a scene change, aren't reused, avoid near-identical pictures, and prefer sharp, well-lit footage. A part can keep the previous part's shot running ("same shot").
- Footage that has nothing to do with the subject (a cartoon in a video about a mall) is only used when nothing else fits.
- Low-resolution footage is shown whole (blurred background) instead of being blown up.
- Every shot says how well it fits: strong, good, loose (only the mood or setting) or weak (nothing in your footage really shows it). Parts nothing fits are listed so you can add footage or pick shots yourself.
- If the prompt names footage ("use the cartoon footage"), that footage is preferred.
- This needs the picture model: **AI Models → Install visual understanding** (about 2 GB, once). Without it, footage is picked for quality and movement only, and ClipForge says so.

**Footage library**
- Add more videos for the narration to draw on: more streams, b-roll, openly licensed footage. Each has a role (main, b-roll, reaction, atmosphere).
- ClipForge asks how you're allowed to use every video, and never uses one without a recorded permission. Credits for every video used go in the export's `.txt` file.

**Script & Visuals (step 2)**
- Every part of the video with its narration, what to show, the footage chosen and why.
- Change one part without touching the others: rewrite it, find different footage, replace one shot, carry the previous shot on, move, add or delete parts, keep footage you like. Change the pacing or style for the whole video.

**Narration**
- With the AI language model (Ollama), ClipForge writes the script: a strong opening, no filler, your number of points, your style (informative, documentary, educational, entertaining, dramatic, conversational, storytelling, commentary, news-style), fitted to the length you picked.
- Facts: with notes or source links it uses only those facts. Without them, it uses general knowledge and marks those parts "check before publishing"; anything unconfirmed is marked speculation. Pages behind a login or paywall are refused, not bypassed.
- Or paste your own script and use it word for word.
- Without Ollama, ClipForge can't write narration: paste your own script (clip-driven videos work as before).

**Sound and captions**
- Captions follow the narration word by word; real moments keep their own speech captions.
- The footage's own sound is turned down under the narration (further when someone is talking in it); real moments keep their sound.

**Music**
- "No music" in the prompt turns music off for that video. "Calm music" (or any other word) picks a file from your music folder with that word in its name. ClipForge doesn't include music, so use music you're allowed to use.

**Command line**
- `clipforge-cli create --spec video.json` makes a video from a prompt without the window.
- `clipforge-cli creativecheck "D:\Videos\stream.mp4" --rights own` tries five kinds of prompt with yo
