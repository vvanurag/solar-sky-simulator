# Solar Sky Simulator

A browser simulation of the Sun, Moon, planets and their orbits as seen from Earth's surface. It shows a real horizon and landscape, day and night skies, and the Milky Way.

Open `index.html` to run it: it's a single file with no build step and no dependencies.

## Features

- **Time controls.** Spring-loaded knobs for time of day and time of year. Push a knob right to run forward or left to run back; the further you push, the faster time runs. Time runs on across days and years, from 1600 to 2500.
- **Observer latitude.** Choose any latitude from 90°S to 90°N.
- **Keep steady.** Choose what stays fixed on screen:
  - Landscape: the sky turns.
  - Sun: the orbital plane stays level and the horizon turns.
  - Stars: the constellations stay fixed and the horizon turns.
- **Camera views.** 50 mm, 24 mm, naked eye, or fisheye.
- **Planets and orbits.** Positions come from JPL approximate Keplerian elements.
- **Moon.** Drawn with its phase. Its path over the next four weeks can also be shown.
- **The Sun's paths.** The Sun's path through the day, plus the analemma: where the Sun stands at the same clock time on each day of the year.
- **Constellations.** All 13 zodiac constellations (including Ophiuchus), Orion, the Big Dipper and Polaris. Arrows at the screen edges point to constellations that are off-screen.
- **Sky backgrounds.** Earth's atmosphere, with day, twilight and night colours, or an airless sky that shows the Milky Way at all times.
- **Landscapes.** Hills, mountains, beach or grassland.

URL parameters can set up a scene, for example `?t=22:00&d=200&obslat=52&frame=sun&bg=space`.

## Local preview

The photographic Milky Way is drawn with WebGL, so the page has to be served over http(s). If you open the file directly from disk, a drawn Milky Way is used instead. To preview the photographic version locally:

```
python3 -m http.server
```

Then open http://localhost:8000.

## Credits

Star and Milky Way background: NASA/Goddard Space Flight Center Scientific Visualization Studio, *Deep Star Maps 2020*. Gaia DR2: ESA/Gaia/DPAC.
