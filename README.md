# gta-cheats-data

The cheat list read by the "Unofficial Cheats for GTA 6" Android app. Edit `cheats.json` here and phones pick
up the change within about 3 hours, or right away when someone pulls down on the Cheats tab.

## How to add a cheat

1. Open `cheats.json` on GitHub and click the pencil (Edit).
2. Find the game (for GTA 6 it is the block with `"id": "gta6"`).
3. Add an entry inside its `"cheats": [ ... ]` list, separated from the others by a comma:

```json
{
  "name": "Max health and armor",
  "category": "Player",
  "codes": {
    "ps": "Circle, L1, Triangle, R2, X, Square",
    "xbox": "B, LB, Y, RT, A, X",
    "pc": "TURTLE",
    "phone": "1-999-887-853"
  },
  "note": "Optional extra line shown under the code."
}
```

4. Click "Commit changes".

Rules:
- Platform keys: `ps`, `xbox`, `pc`, `phone`, `psp`, `ds`, `switch`, `mobile`. Leave out any the cheat does not have.
- Button combos are comma separated. `Up`, `Down`, `Left`, `Right`, `Triangle`, `Circle`, `Square` and `X` are shown as symbols on PlayStation.
- Categories in use: `Player`, `Weapons`, `Wanted level`, `Vehicles`, `World` (these are translated in the app; new ones show as typed).
- A game with an empty `"cheats": []` list shows "Coming soon". Once it has cheats, the badge goes away by itself.

If an edit breaks the JSON (a missing comma, for example), the app ignores it and keeps the last good list.
Check with https://jsonlint.com before committing if unsure.
