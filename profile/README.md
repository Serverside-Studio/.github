## Serverside

**[serversidedev.com](https://serversidedev.com)**  ·  serversidestudio@gmail.com

FiveM deployment and server work — on live servers, with real players logged in.

---

### 🔧 Free tools, no signup

**[Why did my FiveM server crash?](https://serversidedev.com/check)** — paste your console log.
34 diagnostic rules read it and name the cause: pool exhaustion, a resource ensured but never
installed, two scripts fighting over the same command. Nothing is stored.

| repo | what it does |
|---|---|
| 🐕 **[fivem-watchdog](https://github.com/Serverside-Studio/fivem-watchdog)** | Crash diagnosis in your Discord. txAdmin tells you the server went down; this tells you **why**, in plain English. Three Lua files, server-side only, nothing client-side — read the whole thing in five minutes before you install it. |
| 🔍 **[fivem-vendor-config-diff](https://github.com/Serverside-Studio/fivem-vendor-config-diff)** | What a vendor update would **reset** in your tuned config, before you copy the file over. Matches list entries by identity, so a reordered shop list is not two hundred false changes. |
| 📊 **[fivem-fleet-texture-audit](https://github.com/Serverside-Studio/fivem-fleet-texture-audit)** | What a vehicle fleet costs in texture memory, and how much is waste. On a real 203-car fleet: 17.6 GB of textures, **37% recoverable by compression alone**. |
| ⚔️ **[wow-transmog-index](https://github.com/Serverside-Studio/wow-transmog-index)** | Reverse-indexes WoW item sources from Blizzard's API — item to boss, profession and transmog set. 19,065 items in about 120 KB. |

All MIT. All run offline and none of them touch your server.

---

### What we do

| | |
|---|---|
| **Script installs** | $50 for one · $40 each for two or more in one order |
| **Crash diagnosis** | $95, and the diagnosis is credited toward the fix |
| **Server bundles** | Starter $250 · Full Build $500 · Launch Package $750+ |
| **Care plans** | Basic $75/mo · Pro $150/mo · Studio $300/mo — **Watchdog free on every plan** |
| **Vehicle & weapon packs** | ingest, dedupe, collision-check, deploy |
| **Malware scanning** | every third-party pack read before it touches a live server |

**[Every service with its price →](https://serversidedev.com/services/)**

Escrow-aware. Backup before overwrite. And we check the console says a resource actually
**started** before telling anyone it's live.

---

### Some things we found

**A popular carry script was a Discord token stealer.** Circulating widely, caught in a
pre-deploy scan before it reached a live server.

**A server nobody could join, and it wasn't the car.** Players crashed on connect and on
mounting vehicles. The obvious suspect was pulled twice and changed nothing — the actual
cause was the engine's texture pool ceiling, a hard clamp that ignores what `gameconfig.xml`
asks for.

**[39 more write-ups →](https://serversidedev.com/work/)** — the real problem each time, and
what the fix turned out to be.

---

### 💬 [Join the Discord](https://discord.gg/pcPqdeqxcY)

Free advice, install quotes, and Watchdog keys.
