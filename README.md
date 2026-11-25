# What the Dust Keeps · ما يحفظه الغبار

A three.js open-world survival game drawn in a sepia pencil style. A child moves through a ruined Gaza Strip, built from its real outline, towns and roads. He scavenges for the camp, avoids patrols, crosses the strip through tunnels, queues at food distributions and makes it through seven days.

The child never fights. Being caught or collapsing fades out, and he wakes back at camp.

## Play

It is a single file. Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8765
```

Then open http://localhost:8765. three.js and the fonts load from CDNs, so it needs an internet connection.

**Desktop:** W/S walk, A/D turn, mouse to look, Shift run, C crouch, Space jump, E interact, F lantern, G shout, 1/2/3 eat/drink/heal, M map.

**Phone and tablet:** touch controls turn on automatically: a left thumbstick to walk and turn, drag to look, and on-screen buttons. Add `?touch` to the URL to force them on.

## Tuning

Balance settings are plain objects near the code they control in `index.html`:

| Object | Controls |
|---|---|
| `UB` | Underground: lantern drain, hunger, darkness, supplies |
| `AS` | Air strikes: frequency, warning time, damage radius |
| `DC` | Food distribution: hours, queue speed, stock, scramble |
| `RC` | Night looters: how strong shouting, light and the pot are |
| `KC` | Donkey cart: how often, speed, hours |
| `SLOGANS` | Graffiti text |

## Credits

- Map data © [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors, available under the ODbL.
- Administrative boundaries from [geoBoundaries](https://www.geoboundaries.org/) (CC BY 4.0).
- Scale is 1 game metre to 32 real metres. Roads are simplified. Tunnels, camps, distribution centres and patrols are fictional.
- Rendering by [three.js](https://threejs.org/). Fonts are Gaegu and Aref Ruqaa from Google Fonts.
