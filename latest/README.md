# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **2.0.9**

- **Your prompt's rules now win over the page-1 options.** "Video type: …", "Length: 30 seconds" and narration marked "use exactly / do not rewrite" are followed. Your lines are voiced word for word, never rewritten.
- **No "Follow for more" unless you ask for one**, neither spoken nor as an end card.
- **One title and one caption style:** no second, smaller title, and every caption uses the same bold style.
- **"Mute the game audio"** mutes it and drops captions of in-game speech.
- **Clips never end in the middle of a word.**
- **If your prompt asks for something ClipForge can't make yet** (old-vs-new comparisons, split screen, corner labels, music when no music file is set), it stops and tells you instead of making a video that only pretends to follow it.
- **Every export is checked against your prompt:** exact narration, length (±1 s), no call to action unless asked, one caption track and style, no overlapping text, and no audio cut mid-word. If a check fails, the file is renamed `…_CHECK-FAILED` and you're told why. The results are in each video's .txt file.
