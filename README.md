# MTG-Playmat

This table for playing magic the gathering automates a ton of the work playing magic on TTS. 

## Features

- Automatically resizes table as players join
- Start and mulligan buttons
- Untap, draw, scry, and reset buttons
- Upkeep button (Untap + draw in one click)
- Life counter
- CMDR damage counter
- Automatic hand size counter
- Selectable playmat background via import module

## Usage

### Gameplay Controller
The board with buttons to the bottom right of your playmat is used to automate some actions in the game.

The Start button will draw you 7 cards if you have no cards in hand.
The Mulligan button will return your hand to the deck, shuffle, and draw 7 new cards.
Untap and Draw are straight forward, Upkeep is just a combination of the two.
Scry will hover the card above your playmat (hidden so only you can see) with buttons to move it to other locations, this also works for surveilling and other similar abilities.
Reset moves all cards from your field, hand, graveyard, and exile to your library and sets all counters to their default value.

If turns are enabled: after hitting upkeep, it will be replaced by a pass button. The pass button then disappears and is replaced at the start of your next turn by the Upkeep button. Your turn will also be skipped if your controller is in the start/ mulligan phases or your life total is < 0

### Settings Module

The module to the left of your hand is for settings and personalization.

The module will only have autoupkeep as a setting by default, this can be toggled on or off. When autoupkeep is on, the Upkeep button is pressed for you at the beginning of your turn.

If you hit the Importer button, a little white pedestal will appear. You can place a figure on that to load custom data onto. At this time there is no easy way to generate custom data, but there are a few example modules to play with for now. Once data is loaded from the figure, a Change Playmat button will appear in the settings menu, you can use this to switch your playmat with any of the mats provided by the figure.

### Counters

The counters that line the top of your playmat are used for keeping track of various things
- Commander damage
- Life total
- Commander tax
- Hand size

All counters except hand size are manually incremented. Left click will increase the value by 1 while right click decreases it. There are also individual reset buttons on each counter.

## Wish list
These are just a few ideas I have for improving the mats in the future. Suggestions are welcome.

- Experience Counter
- Turn Timer
- Player Infect Counter
- Card Encoding
  - Reset Commander to command zone
  - Move tokens off board on reset
- Alternate playmode
  - Standard / Modern (Life starts at 20, dont spawn commander related stuff)
- Discard reminder on turn pass
