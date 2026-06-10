# ढोल पाठशाळा · Dhol Pathshala

An interactive, single-page web app for learning the traditional **Maharashtrian dhol** — the heartbeat of every dhol-tasha pathak. An animated player in a nauwari saree performs each rhythm (haat) on a steel pathak dhol while the bols light up in time, so you can see, hear, and read the rhythm all at once.

**▶ Live demo:** enable GitHub Pages on this repo and the app runs at your Pages URL — it's a single self-contained `index.html` with all audio embedded.

## The instrument

The dhol is played with both hands at once:

| Bol | Hand | Strike |
|-----|------|--------|
| **ता · Ta** | Left | *Thapi* — the open palm on the drum skin |
| **धिन · Dhin** | Right | *Thoka* — a straight wooden stick with a round knob at the tip |

## Features

- **Five traditional haats** (hands/patterns), from the beginner's *Ta Dhin Dhin* to compound phrases with quick strokes and pauses
- **Animated performance** — the player's arms strike in sync with the audio; bol words (ता / धिन) fly out of the drumheads with pulse rings on every hit
- **Two sound modes** — 🥁 *Dhol* (real recorded thoka + synthesized thapi) and 🗣 *Bol* (a synthesized voice reciting the bols, the way a guru calls the theka)
- **Tempo control** (50–160 bpm) and tap-to-practice buttons (keyboard: `T` = ta, `D` = dhin, `Space` = play/stop)
- **Write your own haat** — a built-in notation editor parses your bols and plays them instantly

## Notation grammar

Write bols separated by spaces in the custom haat editor:

| Notation | Meaning |
|----------|---------|
| `ta` / `dhin` | Full-beat strokes |
| `pause` | A half-beat rest |
| `dhindhin`, `dhinta`, `tadhindhin` | Joined bols = quick half-beat strokes with no gap |
| `ta^` | Ta with the left hand raised high first (the haat ५ flourish) |

Example — the fourth haat:

```
ta dhin dhin dhin tadhindhin pause dhin
```

## Running locally

No build, no dependencies. Just open `index.html` in any modern browser. All artwork is inline SVG and all audio is embedded, so the file works offline too.

## Tech

Vanilla HTML/CSS/JS in one file. Web Audio API for sample playback and synthesis (including formant-synthesized spoken bols), CSS-animated SVG for the scene, and a small duration-aware sequencer driving sound, animation, and bol highlighting from a single clock.

---

*A tribute to the dhol-tasha pathaks of Maharashtra. हर हर महादेव!*
