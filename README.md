# Hockey Bet — Ice Derby

A 90s-style pixel art betting race for events at an ice hockey venue. Six hockey players skate across the rink, and guests bet on who scores first. It works like a classic horse race game, on ice.

**Play it:** https://hsztheater.github.io/hockey-bet/

## How it works

- Six players, each with their own jersey colour and number:
  1 Red · 2 Blue · 3 Green · 4 Yellow · 5 Orange · 6 Purple
- Every race lasts exactly **25 seconds**.
- Speeds change during the race (bursts, slow patches, lead changes), but there is always **one single winner** and never a tie.
- Each player has a true 1 in 6 chance. The winner is drawn at the start with the browser's secure random generator, and the race is then shaped around that result.
- The winner shoots into the net, the goal horn sounds and the lamp lights up. The other players cross the goal line afterwards, and their finishing place is shown next to the net.

Bets are taken outside the game, for example on paper tickets or out loud.

## Running a race

1. Open the game. The betting screen shows the six players and their colours.
2. Press **Space** (or click) to start the 3-2-1 countdown.
3. Watch the race. The current leader is shown at the bottom of the screen.
4. When the winner is announced, press **Space** to go back to the betting screen for the next race.

## Controls

| Key | Action |
| --- | --- |
| Space / click | Start the race, or go to the next race |
| Esc | Cancel the current race and go back to the betting screen |
| F | Fullscreen |
| M | Sound on / off |
| S | Settings: change the title ("OILERS") and subtitle ("ICE DERBY") |

The settings are saved in the browser you use.

## Offline use

The whole game is one file, `index.html`. Graphics, the pixel font and all sounds are generated in code, with no images, fonts or libraries loaded from the internet.

To use it without a network, download `index.html` (or clone the repository) and open it in any modern browser, from a USB stick for example.

## Customising

- **Title and subtitle:** press **S** in the game.
- **Jersey colours and names:** edit the `PLAYERS` list at the top of the script in `index.html`.
- **Race length:** change `RACE_T` (in seconds) in the same place.
