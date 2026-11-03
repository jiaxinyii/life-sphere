# Life Sphere

Your life as a world you can spin.

Every area of your life (academics, athletics, research, friends, whatever matters to you) shapes a 3D world around you. Log what you do, and the areas you invest in grow outward. The shape will never be perfectly round, and that's the point.

## Styles

- **Cinematic**: a sunlit planet. Areas are continents, bigger areas grow mountain ranges, and entries glow as city lights on the night side.
- **Hologram**: a scanned globe with glowing coastlines, elevation contours, and beacons for each entry.
- **Nebula**: no surface at all. Each area is a swirling arm of light, and entries are the bright stars inside it.

## Features

- Add areas and log entries with a year, a size, and an optional note
- Hover any region or entry for details; click to fly the camera there
- Timeline playback that shows your world forming year by year
- A friends view where other people's worlds orbit yours (example data for now)
- Data is saved in your browser's localStorage

## Run it

It's a single static page with no build step. Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Tech

- [three.js](https://threejs.org/) r128 with OrbitControls and UnrealBloom post-processing
- Custom GLSL shaders for terrain, oceans, clouds, atmosphere, and the hologram
- 3D simplex noise, mirrored in JavaScript so entry markers sit exactly on the GPU-generated terrain

## Roadmap

- [ ] Time-lapse export: a shareable "year in review" clip of your world growing
- [ ] Embeddable world for personal sites and portfolios
- [ ] Automatic growth from connected apps (Strava, GitHub, Goodreads, calendar)
- [ ] Accounts and real friends' worlds
- [ ] Port to React + react-three-fiber

## License

MIT. See [LICENSE](LICENSE).
