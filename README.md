**English** | [简体中文](README.zh-CN.md)

# Daily Original Games

Work starts daily at **12:00 Beijing time (Asia/Shanghai)** to create one original, fully playable HTML game that day.

[Play all games](https://xiangjianan.github.io/daily-original-games/)

## Game index

| Date (Beijing time) | Game | Core mechanic | Play (Pages) | Source |
| --- | --- | --- | --- | --- |
| 2026-09-30 | Moonbalance Dock | Plan torque across four lifting points for precise deliveries | [Play](https://xiangjianan.github.io/daily-original-games/2026-09-30/) | [Source](https://github.com/xiangjianan/daily-original-games/tree/main/2026-09-30) |
| 2026-09-28 | Mossgrid Greenhouse | Plant two-cell pieces and harvest square plots | [Play](https://xiangjianan.github.io/daily-original-games/2026-09-28/) | [Source](https://github.com/xiangjianan/daily-original-games/tree/main/2026-09-28) |
| 2026-09-27 | Star Chart Homecoming | Recall routes in reverse across six stages | [Play](https://xiangjianan.github.io/daily-original-games/2026-09-27/) | [Source](https://github.com/xiangjianan/daily-original-games/tree/main/2026-09-27) |
| 2026-09-26 | Day & Night Post Office | Match day and night with stacking merge chains | [Play](https://xiangjianan.github.io/daily-original-games/2026-09-26/) | [Source](https://github.com/xiangjianan/daily-original-games/tree/main/2026-09-26) |
| 2026-09-25 | Neighbor Numbers Bakery | Pair adjacent numbers and heat neighboring cells | [Play](https://xiangjianan.github.io/daily-original-games/2026-09-25/) | [Source](https://github.com/xiangjianan/daily-original-games/tree/main/2026-09-25) |
| 2026-09-24 | Echo Lights | Linked light pairs, randomized patterns and fewer-move challenges | [Play](https://xiangjianan.github.io/daily-original-games/2026-09-24/) | [Source](https://github.com/xiangjianan/daily-original-games/tree/main/2026-09-24) |
| 2026-09-23 | Stars on the Wind | Use wind direction to plan landing spots and staged deliveries | [Play](https://xiangjianan.github.io/daily-original-games/2026-09-23/) | [Source](https://github.com/xiangjianan/daily-original-games/tree/main/2026-09-23) |
| 2026-09-16 | Three-Color Rain Garden | Collect distinct colors in three pots with previews and rotating dormancy | [Play](https://xiangjianan.github.io/daily-original-games/2026-09-16/) | [Source](https://github.com/xiangjianan/daily-original-games/tree/main/2026-09-16) |

## One repository, organized by date

Since September 30, 2026, past and future games live in `YYYY-MM-DD/` directories at the repository root, with `index.html` as each game's entry point. No separate daily repositories are created. GitHub Pages publishes from the root of `main`. Preserve past games, do not overwrite a completed day's release, and never force-push.

Each dated directory contains the full code, `README.md`, `research.md`, `design.md` and `tests.md`. Before development, check recent casual-game trends and record sources, dates and data coverage. Borrow design principles, combine them originally and avoid repeating earlier games. Each game includes clear controls, a complete gameplay loop, scoring or goals, an ending and restart, sound activated after interaction with a mute option, and link or score sharing, with desktop and mobile support.

Before release, test starting, core gameplay, scoring, ending, restarting, sound and mute, sharing, layout and console errors in a real browser. Verify the remote commit, Pages deployment and live gameplay after pushing. Document replay mechanics and design hypotheses explicitly; do not invent usage or retention findings. Daily reports in the task provide a Chinese mechanic summary, play link and source link.

See the [migration record](migration-2026-09-30.md) for historical repository migration, backups and verification. Historical notes in `games/` are retained. Game interfaces and detailed daily notes are currently in Chinese; the English titles above are descriptive translations. Keep the English and Chinese root READMEs in sync when adding games.
