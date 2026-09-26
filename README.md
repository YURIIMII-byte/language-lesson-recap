# language-lesson-recap

Transcribes a recorded language lesson and pulls out new vocabulary and corrections, on-device. Built with [Tether's QVAC SDK](https://github.com/tetherto/qvac) — the model runs on-device, so nothing leaves your machine.

## What it does

Transcribes a recorded language lesson and pulls out new vocabulary and corrections, on-device.

**QVAC functions used:** `loadModel`, `transcribe` and `completion`.

![language-lesson-recap demo](demo.png)

## Why I built it

My tutor corrects me twenty times an hour. I remember two of them.

## Requirements

- Node.js >= 22
- `@qvac/sdk` `^0.19.0` (installed automatically via `npm install`)

## Install

```bash
git clone https://github.com/YURIIMII-byte/language-lesson-recap.git
cd language-lesson-recap
npm install
```

## Run

```bash
node index.js path/to/lesson.wav
```

See the comments at the top of `index.js` for the exact input this app expects. On first run, QVAC downloads the model it needs once and caches it locally; every run after that is fully offline.

## SDK version used

`@qvac/sdk` `0.19.1`

## License

MIT — see [LICENSE](LICENSE).
