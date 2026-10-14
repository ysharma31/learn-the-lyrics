# Learn the Lyrics (Lyric Stand)

A single-page app for learning to sing a song's lyrics.

- **Find songs on the internet.** Search by title (with an optional artist), or type or say a line you remember and the app works out which song it is. If several songs share the title, it asks which one you mean.
- **Autofill.** Picking a song fills in the lyrics, artist, singer(s), album or film, and year. Lyrics come from [LRCLIB](https://lrclib.net), year and credits from [MusicBrainz](https://musicbrainz.org), and on claude.ai Claude recognises songs from a line and fills in singers. Check the details before saving.
- **Or add songs yourself** by pasting lyrics, or dropping a `.txt` / `.lrc` file.
- **Numbered lines.** Lines in brackets, such as `[Chorus]` or `[मुखड़ा]`, become section labels and don't get a number.
- **Auto-scroll on or off.** With it on, the current line stays in the middle and moves on at your pace (seconds per line, adjusted for line length). With it off, you scroll yourself and tap a line to mark it.
- **Restart** with a 3-2-1 countdown (button or `R`). Space plays and pauses; ↑/↓ move between lines.
- **Ask box.** Type commands like `restart`, `start from line 9`, `revise lines 5-8`, `revise the chorus`, `go to verse 2`, `slower`, `test me`. When the page is opened on claude.ai, anything else (meaning, pronunciation, Hindi transliteration) goes to Claude, which can also control playback.
- **Practise modes:** Full, First letters, Hidden (tap a line to peek).
- **Languages:** English and Hindi (Devanagari is detected automatically). To add a language, add an entry to `LANGS` in `index.html`.

Songs are saved to your Claude account when the page is opened as a claude.ai artifact, or otherwise in your browser.

## Where each feature works

| | Opened as a normal web page (GitHub Pages, or the file) | Opened on claude.ai |
|---|---|---|
| Lyrics search by title | Yes | No: the page can't go online there. You get song details and a web-search link |
| Find a song from a line | Keyword search only | Yes, Claude recognises the song |
| Say a line out loud | Yes, in Chrome, Edge or Safari | No microphone access |
| Ask box questions | Commands only | Commands and free-form questions |
| Saving songs | In this browser | In your Claude account |

Open `index.html` in a browser to use it locally.
