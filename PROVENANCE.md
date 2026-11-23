# Provenance

## Voice
- Model: **Kokoro-82M v1.0** by hexgrad (https://huggingface.co/hexgrad/Kokoro-82M), **Apache License 2.0**, which allows commercial use. Its model card says it was trained only on permissive or non-copyrighted audio.
- Voice: **am_michael** (American English, male), from the same Apache 2.0 repository.
- Run locally on our own computer with kokoro-onnx (MIT) and onnxruntime. No paid or cloud speech service was used. The voice is computer generated, not a human reader.
- Settings: speed 0.9; each verse made separately and joined with 0.45 s of silence; each chapter starts with "<Book>, chapter <n>." Encoded as Opus 16 kbps mono (WebM) from a 24 kHz original. Same settings as https://github.com/Nloperena/ethiopian-bible-audio
- Text cleanup before reading: translators' square brackets and editorial marks removed; LORD and GOD read as Lord and God.

## Texts read
| Books | Source | License |
|---|---|---|
| 1 Maccabees, 2 Maccabees, Prayer of Manasseh, 2 Esdras (except 7:36-105) | King James Version with Apocrypha, 1769 standard text, eBible.org `eng-kjv` (https://ebible.org/Scriptures/eng-kjv_vpl.zip) | Public domain (https://ebible.org/eng-kjv/copyright.htm). In the UK, Crown letters patent restrict printing; this has no effect elsewhere. |
| 3 Maccabees, 4 Maccabees, 2 Esdras 7:36-105 | World English Bible, eBible.org `eng-web` (https://ebible.org/Scriptures/eng-web_vpl.zip) | Public domain dedication (https://ebible.org/eng-web/copyright.htm). "World English Bible" is a trademark of eBible.org; the text is read unchanged. |

The KJV lacks 2 Esdras 7:36-105. That passage is read from the World English Bible, and the KJV verses after it are numbered 106-140, as in modern editions.

## License of these audio files
- **Recordings** (`.webm`), timing files (`.json`) and `index.json`: **CC BY-SA 4.0**. Legal code in [LICENSE](LICENSE). Credit: **Nexrena LLC Bible app**.
- **Texts**: public domain, as listed above. CC BY-SA 4.0 covers only the recordings.
- **Voice model**: Kokoro-82M v1.0 and the am_michael voice are under the **Apache License 2.0** by their authors. Not covered by CC BY-SA.
