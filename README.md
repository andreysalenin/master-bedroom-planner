# Master Bedroom Planner

A 3D planner for the master bedroom: the room, the AAGL-J robe from the Master Robe Builder, the Castlery Seb bed and bedside tables, and the hamper rails in the entrance corner, with load and clearance checks.

The page is locked with a passphrase. Everything except the lock screen, three.js (loaded from a CDN) and the generic shoe models in `shoes/` is encrypted inside `index.html`: AES-256-GCM, with a key derived from the passphrase by PBKDF2-SHA-256 (600,000 iterations). Without the passphrase the page shows only the lock screen.

## Opening it

Serve the folder over https (for example with GitHub Pages: Settings → Pages → Deploy from a branch → `main`, `/ (root)`), open `index.html` and enter the passphrase. Tick "Remember on this device" to skip the prompt next time on that browser.
