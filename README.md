# MoodWave

A single-file binaural-beat mood synthesizer with a retro, neon Windows Media Player–style visualizer. Built with React 18 (via esm.sh + htm, no build step), Tailwind CSS, and the native Web Audio API.

## Moods

| Mood | Left | Right | Beat |
|------|------|-------|------|
| Sleep | 150 Hz | 153 Hz | 3 Hz Delta |
| Relax | 150 Hz | 156 Hz | 6 Hz Theta |
| Study | 150 Hz | 162 Hz | 12 Hz Alpha |
| Amp Up | 150 Hz | 185 Hz | 35 Hz Gamma |
| Intimate | 150 Hz | 157.83 Hz | 7.83 Hz + 528 Hz swell |

Each mood layers a warm detuned pad and filtered pink noise under the binaural pair, and crossfades over 2.5 s.

**Use headphones** — binaural beats only work when each ear gets its own tone.

Keys: `1`–`5` switch moods, `Space` plays/pauses.

## Run locally

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy

Render static site (see `render.yaml`): no build step, publish directory `.`.
