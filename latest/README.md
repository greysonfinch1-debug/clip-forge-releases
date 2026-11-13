# ClipForge update channel

The ClipForge app downloads its updates from this folder. Every file is checked against ClipForge's signature and SHA-256 before anything is installed.

Current version: **1.3.0**

**Tell ClipForge how to make the Short**
- The topic box now understands instructions as well as the topic. Type, for example, *"make the video about the police chases and describe the 4 craziest ones"* or *"top 5 funniest NPC moments, explain why each one is funny"*.
  - **How many:** "the four coolest things" picks 4 moments.
  - **Countdown:** "top 5", or a number plus "best / coolest / craziest…", gives a countdown: #5 … #1 on screen, the best moment last.
  - **Story order:** "tell the story … in order" keeps the clips in the order they happened.
  - **Narration:** "describe / explain each one" gives every clip its own line about that moment; "no narration" turns the voice off.
- With the AI language model (Ollama) running, each line says what happens in that clip and why it fits your request. Without it, ClipForge can't see what happens, so each line is the moment's number plus the most telling thing actually said in it, word for word (never anything made up, never swearing). Page 4 tells you which one you got.
- If Ollama wasn't running when you started, start it and click **Rewrite script with AI**: ClipForge now tries again instead of staying in basic mode until you restart.

**Projects**
- **Projects…** (bottom left) lists all your projects: name, video, topic, current step, last change and status. From there you can open one, start a new one, rename it or delete it.
- When you delete a project you choose whether its downloaded video and analysis go too. They're kept automatically if another project uses the same video. Exported Shorts, settings, AI models and other projects are never touched.
- Projects save automatically whenever you move between steps, after every task, and shortly after edits.
- Saves are crash-safe: a new save never half-overwrites the old one, and the last 5 versions are kept. A damaged project file is restored from the newest good copy.

**Restart project**
- **Restart project…** (bottom left) starts the open project over from step 1, from any step.
- You can keep the video and its analysis (so finding moments again takes seconds), or start completely from scratch.
- Nothing from before reappears, and your settings, models and other projects are untouched.

**Cancel anything, see what's happening**
- A status bar at the bottom shows what ClipForge is doing (Downloading, Analysing, Generating, Rendering, Exporting, Cancelling, Finished, Error) and which step it's on.
- It shows a percentage only when one can really be measured; otherwise it shows a moving "working" bar. It estimates the time left once it can.
- **Cancel** stops any task within a few seconds and leaves the project as it was before that step, including language-model answers, voice recording and downloads. A cancelled download has completely stopped writing by the time Cancel finishes, so you can start it again straight away.
- While a task runs, the steps are read-only, so two tasks can't fight over your project.
- No FFmpeg is ever left running in the background, even if ClipForge itself is closed by force.

**No more freezing during "Identifying speakers"**
- The window used to freeze for several seconds at a time while ClipForge worked out who was speaking (worse on long streams). That model now runs in a small helper process, so the window stays responsive, and Cancel stops it instantly. The results are exactly the same.

**Going back to change things**
- ClipForge tracks what each step was made from, and tells you (yellow note) when an earlier change makes a later step out of date.
- It redoes only what's needed: a new hook doesn't re-download clips, new narration doesn't redo the analysis, a caption style only re-renders, and a new topic reuses the video's analysis.
- You're asked before anything that would replace your hand edits.

**Normal PCs**
- New **Performance** setting: Balanced (default), Performance or Low resource. The modes change speed and how much of the PC ClipForge uses, not quality.
  - Balanced leaves CPU
