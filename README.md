# Learn the Lyrics (Lyric Stand)

A single-page app for learning to sing a song's lyrics.

- **Add songs** by pasting lyrics, or dropping a `.txt` / `.lrc` file. You can save a link to the lyrics with each song so you can open it again.
- **Numbered lines.** Lines in brackets, such as `[Chorus]` or `[मुखड़ा]`, become section labels and don't get a number.
- **Auto-scroll on or off.** With it on, the current line stays in the middle and moves on at your pace (seconds per line, adjusted for line length). With it off, you scroll yourself and tap a line to mark it.
- **Restart** with a 3-2-1 countdown (button or `R`). Space plays and pauses; ↑/↓ move between lines.
- **Ask box.** Type commands like `restart`, `start from line 9`, `revise lines 5-8`, `revise the chorus`, `go to verse 2`, `slower`, `test me`. When the page is opened on claude.ai, anything else (meaning, pronunciation, Hindi transliteration) goes to Claude, which can also control playback.
- **Practise modes:** Full, First letters, Hidden (tap a line to peek).
- **Languages:** English and Hindi (Devanagari is detected automatically). To add a language, add an entry to `LANGS` in `index.html`.

Songs are saved to your Claude account when the page is opened as a claude.ai artifact, or otherwise in your browser.

Open `index.html` in a browser to use it locally.
