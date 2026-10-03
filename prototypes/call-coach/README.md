# Call Coach – weekly coaching loop (design prototype)

Clickable prototype for the Call Coach app (calls.alpharetta.fit/v2):
one card per rep per week, sent by text or email, a no-login rep link
to listen and commit, and a manager view that closes the loop.

Live canvas: https://claude.ai/artifact/QKbsXDWmzjc1puAjv64Mgy

These are Design canvas artboards (`.dc.html`), not production code.
The Call Coach front end is not in this repository, so the visual
language was rebuilt from screenshots of the current /v2 pages.

| File | Screen | Route |
| --- | --- | --- |
| `RepText.dc.html` | Text message the rep receives | SMS |
| `RepAudio.dc.html` | Rep link, variant A (leads with audio) | new public `/r/:token` |
| `RepLine.dc.html` | Rep link, variant B (leads with the line) | new public `/r/:token` |
| `RepExpired.dc.html` | Expired link | `/r/:token` |
| `Main.dc.html` | This week (replaces Team) | `/v2/team` → This week |
| `Progress.dc.html` | Rep progress (Makenzie) | new, under This week |
| `Loop.dc.html` | Closing-the-loop card states | component |
| `Coach.dc.html` | Coach, with Discovery category | `/v2/` |
| `Calls.dc.html` | Calls list, with discovery column | `/v2/calls` |
| `CallDetail.dc.html` | Call detail, with discovery breakdown | `/v2/call/:id` |
| `Backend.dc.html` | Backend changes needed | notes |

`canvas.json` is the canvas index (artboard positions and sizes).
