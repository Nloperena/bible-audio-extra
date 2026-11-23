# Bible audio, extra books

Recorded audio for the free, ad-free Bible app by Nexrena LLC (https://ethiopian-bible-lyart.vercel.app).
This repo holds books that are not in the Ethiopian 81-book set, which lives at https://github.com/Nloperena/ethiopian-bible-audio .
One computer-generated voice reads each chapter. No ads, no tracking, and no account is needed.

Files are served with GitHub Pages at https://nloperena.github.io/bible-audio-extra/

## Books planned here
| id | Book | Text |
|---|---|---|
| 1ma | 1 Maccabees | KJV Apocrypha (1769) |
| 2ma | 2 Maccabees | KJV Apocrypha (1769) |
| 3ma | 3 Maccabees | World English Bible |
| 4ma | 4 Maccabees | World English Bible |
| 2es | 2 Esdras (all 16 chapters) | KJV Apocrypha (1769), with 7:36-105 from the World English Bible |
| man | Prayer of Manasseh | KJV Apocrypha (1769) |

## Layout
Same as the main audio repo.
- `index.json`: every chapter that is ready: `{voice, base, ext, type, ch:{book:[chapters]}, kb:{"book/n":KB}}`
- `<book>/<n>.webm`: chapter audio. Opus, 16 kbps, mono, in WebM.
- `<book>/<n>.json`: timings `{"v":voice,"s":speed,"d":seconds,"t":[[verse or null, start, end], ...]}`, one row per verse.

Chapters are added in batches as they are made. Uploads stop before the site reaches 950 MB, under GitHub Pages' 1 GB limit.

## License
The recordings (`.webm`), their timing files and `index.json` are licensed under the
**Creative Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0)**. Full legal code: [LICENSE](LICENSE),
also at https://creativecommons.org/licenses/by-sa/4.0/legalcode

Credit: **Nexrena LLC Bible app**. Please link to https://github.com/Nloperena/bible-audio-extra and note any changes you make.

The texts keep their own licenses, listed in PROVENANCE.md (all public domain).
The voice model, Kokoro-82M, is licensed separately under the Apache License 2.0.
