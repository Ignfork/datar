# DATAR ($DATAR)

A Solana launchpad site set in a pixel DEFCON 5 operations room, with a 2000s internet look: Win98-style windows, a marquee, a hit counter and 88x31 badges.

## Deploy
The site is a single `index.html` with no folders and no build step. Drop it into a GitHub repo or Vercel.

## Settings
Open `index.html` and find `CONFIG` near the top of the script:

```js
var CONFIG={xUrl:'',ca:'',buyUrl:'',chartUrl:'',launchUrl:''};
```

- `xUrl`: your X profile link
- `ca`: the $DATAR contract address. Until it's set, the page says "CA drops on X at launch".
- `buyUrl` / `chartUrl`: your buy page and chart link
- `launchUrl`: optional. When set, the wizard's final "Transmit" step opens this real launch app instead of the demo.

## What's on the page
- **Ops room hero:** a pixel canvas with a global launch map, radar scope, DEFCON board (lit at 5, "ALL QUIET"), world clocks, CRT consoles and empty chairs. Parts of the room are clickable.
- **Hot coins:** ranked by 24h volume, market cap or newest. Each coin opens a dossier showing its chart, pair, tax and fee routing.
- **Holder payout timer:** runs every 10 minutes, synced to the real clock, with a payout curve and a bonding-curve view.
- **Radar sweep:** every coin is a blip, and closer to the centre means more volume. Tap a blip to lock on.
- **Platform volume:** 7D and 30D views, plus a split of coins and fees by pair (SOL, stables, stocks, tokens).
- **Holder rewards:** total paid, latest rounds and the minimum hold.
- **Marketing tank:** trading fees fill up boost tiers, which are bought automatically when full.
- **Live trades and an onchain activity log.**
- **Launch wizard (8 steps):** Details, Socials, Pair, Tax, Fees, Holders, Marketing and Review. In demo mode the brief is saved on the visitor's device and their coin appears on the radar as a draft. No transaction is sent.
- **Search:** opens with Ctrl/⌘ K.
- **Start menu and taskbar.**

All coins, trades and payouts are a clearly labelled simulated sample feed until the token is live.
