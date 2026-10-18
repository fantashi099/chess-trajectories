# Chess trajectories

[Explore the 20 recorded games](https://fantashi099.github.io/chess-trajectories/)

A static chess trajectory explorer with a synchronized timeline, board playback,
and recorded model/tool evidence. Select Stockfish **1500** or **2000** Elo and one of **10 games** at each Elo.
The viewer shows only LLM-agent games; there is no mode selector or comparison strip.

Only sanitized recordings and browser assets are published. The site runs no
models, chess engines or backend. Recorded rationales are model claims, and
missing reasoning is never reconstructed. These games do not demonstrate
Reflexion or learning between games.

The 2000 Elo LLM + Tools collection was retrospectively selected by outcome
across three source runs; it is a case-study collection, not a representative
win-rate estimate. Its selection provenance remains in the run manifest.
Individual game labels retain their recorded completion status.

## Hosting

GitHub Pages serves the root of `main`. `.nojekyll` disables Jekyll processing;
there is no build step or dependency installation. Relative asset and data URLs
support the `/chess-trajectories/` project path and bookmarked event hashes.

To preview locally, serve this directory with an HTTP server. To update the
site, replace browser assets and sanitized data, then push to `main`.

The importer and viewer source are maintained in
[the chess-agent project](https://github.com/fantashi099/harness-chess-agent)
on branch `feat/chess-trajectories`. Unused generated search indexes and the
unfinished blog are excluded from this publication.
