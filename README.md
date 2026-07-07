# 🏋️ Gym Exercises

A structured library of gym exercises and ready-to-run training programs, organized by experience level — plus a mobile web app you can install on your phone.

## What's inside

```
gym-exercises/
├── index.html            📱 Mobile web app (installable on iPhone)
├── manifest.webmanifest  PWA manifest
├── sw.js                 Service worker (offline support)
├── apple-touch-icon.png  Home-screen icon
├── programs/             Complete weekly programs by level
├── exercises/            Exercise reference by muscle group
├── data/                 Machine-readable exercise database (JSON)
└── docs/                 Progression guide
```

## 📱 Run it on your iPhone

The repo doubles as an installable workout app with three tabs:

- **WEEK** — tracker for your active program: day tabs, tap-to-check exercises, weekly progress bar, auto-resets each Monday
- **LIBRARY** — recommended exercises and sets for every body region (chest, back, shoulders, arms, legs, core), filterable by level
- **AI COACH** — describe your goal, level, days, and equipment, and AI generates a custom routine you can apply as your active week with one tap

1. Enable GitHub Pages: repo **Settings → Pages → Source: Deploy from a branch → main / (root)**
2. Open `https://<your-username>.github.io/gym-exercises/` in **Safari** on your iPhone
3. Tap **Share → Add to Home Screen**

It now launches full-screen like a native app, and your check-offs save on the device.

**AI Coach note:** inside Claude the generator works automatically. Running standalone (GitHub Pages / home screen), it needs an Anthropic API key from console.anthropic.com — pasted once in the app, stored only on your device, usage billed to your key.

## Pick your level

| Level | Experience | Program | Days/week | Focus |
|---|---|---|---|---|
| 🟢 Beginner | 0–6 months | [programs/beginner.md](programs/beginner.md) | 3–5 | Machines, learning movement patterns |
| 🟡 Intermediate | 6–24 months | [programs/intermediate.md](programs/intermediate.md) | 4 | Free-weight compounds, Upper/Lower split |
| 🔴 Advanced | 2+ years | [programs/advanced.md](programs/advanced.md) | 6 | Push/Pull/Legs, higher volume, RPE-based |

## Set & rep cheat sheet

| Level | Compound lifts | Accessory lifts | Rest (compounds) |
|---|---|---|---|
| Beginner | 3×10–12 | 2–3×12–15 | 90 sec |
| Intermediate | 4×6–10 | 3×10–15 | 2–3 min |
| Advanced | 4–5×5–10 (RPE 7–9) | 3–4×10–20 | 2–4 min |

## Using the data

`data/exercises.json` contains every exercise with muscle group, equipment, minimum level, and per-level set/rep recommendations — useful for building apps, scripts, or spreadsheets on top of this library. The bundled app ships with the beginner program as its default week, surfaces this same library in its LIBRARY tab, and can swap in AI-generated routines.

## Disclaimer

This is general fitness information, not medical advice. Learn proper form (ask gym staff or a qualified trainer), start lighter than you think you need, and check with a healthcare professional before starting a new program if you have any health concerns.

## License

MIT — see [LICENSE](LICENSE).
