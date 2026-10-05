# Super Castlevania IV Password Generator

A password generator for Super Castlevania IV (SNES, US version) that runs in any web browser. Type the player name you entered in the game, choose first or second quest, and it shows the password for every level.

**Use it online:** https://codekonga.github.io/Super-Castlevania-IV-Password-Generator/

It's a single HTML file with nothing to install. You can also download `index.html` and open it in any browser, including offline.

## Features

- Passwords for all 15 password checkpoints, shown as the game's 4×4 icon grid (axe, holy water, heart, empty)
- First quest and second quest passwords (second quest is the harder replay after the ending)
- Spaces anywhere in the name: at the start, in the middle, or at the end, matching what the game's name screen allows
- Correct passwords for 8-character names
- Characters the name screen doesn't have (0, punctuation and so on) give blank results

## Credits

Based on TFG's `scv4pg` password generator, whose reverse-engineering of the password algorithm this builds on.

Second quest support comes from the game's own password check (`$03:82EA` in the US ROM). The decoded second byte goes into `$88`, the game's second-quest flag, and is also added to the checksum.
