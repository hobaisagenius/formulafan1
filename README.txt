THE GRID — F1 DRIVER EDITORIAL / VERSION 2

Changes:
- Direct Formula 1 media CDN URLs requested at a much larger image size.
- Team cards show team logos instead of driver portraits.
- Opening a team gives exactly three choices: Team history, Drivers, 2026 season.
- Team history includes origins/context and GP entries, wins, podiums, poles and championships.
- Driver dossiers include starts, wins, podiums, poles, championships, career points, highest finish and DNFs, plus 2026 season stats.
- Smooth transitions and responsive layout retained.

NETLIFY:
Extract the ZIP and drag the folder containing index.html, style.css and app.js into Netlify Drop. index.html must be at the deployment root.

DATA:
Current 2026 line-ups and statistics were checked against official Formula 1 team/driver pages on 8 September 2026. Images/logos are loaded from Formula 1's media CDN. Check Formula 1's brand/media guidelines before public or commercial redistribution.

PRIVATE v4 STABILITY FIX
------------------------
- Fixes archive menu text bleeding/overlap: the closed full-screen menu is now
  visibility:hidden + pointer-events:none + overflow-contained, not just translated.
- Team cards use side-profile 2026 car renders in a contained center stage rather
  than full rectangular photography. White/light render backgrounds are blended
  into the team color with multiply + edge masking.
- Ferrari uses a clean wordmark treatment if the crest asset is unsuitable.
- Archive card -> detail transitions are DOM-safe fades: the previous page is
  replaced before the new page enters; no cloned or fixed ghost cards are used.
- CSS/JS have ?v=4.1 cache-busting in index.html for Netlify/Brave redeploys.
