# Grayson's Lugia Game

Side-scrolling Pokemon-themed shooter for Grayson (Colin's 5yo nephew). Mobile web game hosted on GitHub Pages.

## Game Design
- Player rides Lugia, uses up/down arrow buttons to move
- Lugia auto-shoots Aeroblast (swirling blue energy beam)
- 3 levels: Route 1, Whirl Islands, Mt. Silver
- Boss fight at end of level 3 (burst/pause attack pattern)
- 3 lives, smart adaptive difficulty (eases up if dying frequently, ramps back if cruising)
- Poke Ball collectibles, power-ups (rapid fire, shield, big shot, extra life)
- Pokemon battle theme chiptune BGM
- Googly eyes on enemies, fire explosions, screen shake, parallax backgrounds
- Tutorial on first play, landscape lock prompt
- Celebratory win/game over screens

## Tech
- Single HTML file with inline CSS/JS using HTML5 Canvas
- All sounds generated programmatically (Web Audio API)
- Touch controls: D-pad arrow buttons (bottom-left)
- Hosted on GitHub Pages (colin1201 account)
- Player sprite: grayson-lugia.png (transparent background, facing right)

## Repo
- GitHub: https://github.com/colin1201/graysons-lugia
- Live: https://colin1201.github.io/graysons-lugia/

## Key Design Decisions
- Hitbox is 55% width x 65% height of image (transparent pixels excluded)
- Boss uses burst pattern (3 shots then 2s pause) so player can dodge
- Adaptive difficulty is invisible — no UI indicator, just feels easier when struggling
- Tutorial stored in localStorage, only shows once
- Power-up hearts only spawn when below 3 lives
