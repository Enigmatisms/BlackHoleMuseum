# Black Hole Museum

[中文说明](./README.zh-CN.md)

An interactive WebGL2 black-hole observatory.

Choose a curated scene or switch to the editor and build your own view. The page runs entirely in the browser.

## Screenshots

![English interface — NGC 4258](./images/observatory-en.png)

![Chinese interface — Gargantua](./images/observatory-zh.png)

## Features

- Schwarzschild gravitational lensing
- Continuous volumetric accretion discs
- Thermal blackbody, artistic palette, and power-law false-colour modes
- Doppler shift and relativistic beaming controls
- Curated observed, fictional, and artistic scenes
- Full editing of camera, disc geometry, density, turbulence, radiation, colours, gradients, timing, and star field
- Mouse, touch, keyboard, and WASD camera controls
- Horizon-distance, time-dilation, clock, and model-temperature readouts
- JSON import/export and local workspace saving

## Model

The renderer uses a non-rotating Schwarzschild spacetime. Gas, opacity, temperature, colour, and scene shape are procedural parameters. This is not a Kerr, GRMHD, synchrotron, or observational-data reconstruction.

Temperature values are area-weighted model colour temperatures for thermal scenes. False-colour scenes do not represent measured gas temperatures.

## Run locally

Serve this directory with any static HTTP server.

```bash
python -m http.server 8000
```

Then open `http://127.0.0.1:8000/`.

## License

The observatory is licensed under **AGPL-3.0-only**. See [`LICENSE`](./LICENSE), [`NOTICE`](./NOTICE), and [`source.html`](./source.html).

Third-party licenses are in [`licenses/`](./licenses/).
