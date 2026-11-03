# Idrelyan

Website for **Idrelyan** — one house in Idre with two rentable apartments, 18 beds in total: *Stora lyan* (ca 160 m², 12 beds) and *Lilla lyan* (ca 60 m², 6 beds).

A single-page static site (`index.html`) built with Tailwind CSS (via CDN), featuring photo galleries for both apartments and a looping drone video.

## Local preview

Open `index.html` directly in a browser, or serve the folder with any static server.

If you have Node installed, `node serve.mjs` starts one on http://localhost:3000.
It has no dependencies, and unlike some simple servers it sends the correct MIME
type for `.mp4` and supports byte-range requests — both required for the drone
video to play on iOS. `serve.mjs` is only for local preview; it does not need to
be uploaded to the web host.

There is no build step — editing `index.html` and the files in `Bilder Idrelyan/` is all that's needed. Note that the folder name contains a space (referenced as `Bilder%20Idrelyan/`), and that `IMG_1317.JPG` has an uppercase extension; both matter on case-sensitive (Linux) hosting.

## Deployment

Static hosting — upload `index.html`, `favicon.svg` and the `Bilder Idrelyan/` folder to the web root. The server must serve `.mp4` with byte-range support, or the drone video will not play on iOS.

## Contact

Johan 0705-560023 · Stefan 0708-340043 · info@idrelyan.se
