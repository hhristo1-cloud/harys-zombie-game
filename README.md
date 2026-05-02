# Hary's Zombie Survivor

Browser-based zombie horde survivor game in the vein of *Vampire Survivors* / *20 Minutes Till Dawn*. Top-down arena, hordes of zombies, auto-firing weapons, level-up upgrade picker. Built mobile-first as a single HTML file using the Canvas 2D API — no build step, no framework.

## Status

**v0.2 — Step 1 (Foundation) complete.**
- Top-down 2D Canvas, camera follows player
- WASD on desktop, virtual joystick on touch devices (analog)
- Zombies spawn from off-screen and walk at the player
- Auto-firing pistol locks onto the nearest zombie
- HP bar, contact damage with brief invulnerability
- Death overlay with kills + time + restart
- DPI-aware canvas, safe-area-aware UI, locked viewport

## Mobile-first

Mobile (especially phones) is the primary target. Every step of the roadmap must work and feel good with one thumb on a phone. Touch joystick + auto-fire keeps controls minimal. UI uses `clamp()` and safe-area insets so it works on notched screens. Performance budget: 60fps on mid-tier phones with 200+ on-screen zombies.

## Roadmap to v1.0

1. **Foundation** — WASD + touch joystick, zombies that walk at you, auto-firing pistol, HP, death/restart ✅
2. **Juice** — hit flash, blood, gibs, screen shake, hit-stop on kill, kill thuds
3. **XP + Leveling** — gem drops, level-up freeze, 3-card upgrade picker
4. **5 Weapons** — pistol, shotgun, fire ring, lightning chain, bouncing knives — 5 upgrade tiers each
5. **Enemy Variety** — fast runners, fat tanks, exploders, ranged spitters
6. **Bosses** — every 5 min, big zombie + treasure chest
7. **Real Audio** — proper SFX, ambient horror loop, level-up sting
8. **Meta-Progression** — gold persists between runs → permanent upgrades shop
9. **3 Maps + 3 Characters** — graveyard, sewer, ruins; characters with starting perks
10. **Polish** — difficulty modes, achievements, leaderboard, settings, accessibility

## Play

Open `index.html` in a browser, or visit the deployed URL: https://harys-zombie-game.vercel.app

## Dev

Single `index.html`, no build step. Vanilla JS + Canvas 2D. Push to `main` → Vercel auto-deploys.
