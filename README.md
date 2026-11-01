# Learn the Lyrics (Lyric Stand)

A single-page app for learning to sing a song's lyrics.

- **Find songs on the internet, no pasting.** Search by title, type or say a line you remember, or paste a YouTube, Spotify or lyrics-site link. Pick the song and it's added to your library with the lyrics already loaded. If several songs share the title, the app asks which one you mean.
- **Autofill.** The artist, singer(s), album or film, and year are filled in too. Lyrics come from [LRCLIB](https://lrclib.net), year and credits from [MusicBrainz](https://musicbrainz.org), and links are read through [noembed](https://noembed.com). On claude.ai, Claude recognises songs from a line and fills in singers. Press Edit on a song to check or change the details.
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
| Lyrics load by themselves (title, line or link) | Yes | No: the page can't go online there. It links to the full app |
| Find a song from a line | Yes, when the line contains part of the title (choruses usually do) | Yes, Claude recognises the song from any line |
| Say a line out loud | Yes, in Chrome, Edge or Safari | No microphone access |
| Ask box questions | Commands only | Commands and free-form questions |
| Saving songs | In this browser | In your Claude account |

Open `index.html` in a browser to use it locally.
