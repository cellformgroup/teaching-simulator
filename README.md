# Cellform Teaching Simulator

Scenario-based training for new STEM teachers. Read a real classroom moment,
choose a response, see what actually happens, learn the principle. No score —
wrong turns teach as much as right ones.

Sibling project of the Cellform game platform (game-platform repo),
same stack and design language.

## Run it

Open `index.html` in a browser. Single HTML file, React via CDN, no build step.
Scenarios currently live as plain objects at the top of the file; they move to
a database (Supabase) as the project grows, same pattern as the game platform.

## Add a scenario

A scenario is a graph of steps: decision steps (a prompt and options) and
feedback steps (what happens, the principle, optionally a follow-up decision).
See the format comment at the top of `index.html`. Content rules: real teaching
situations only, all options plausible, consequences honest, calm copy.
Scenarios carry a draft/verified status — only verified content ships to teachers.

## Design rules

Editorial + pixel: Georgia serif for content, Courier mono for labels, pixel
details carry the identity, color carries meaning (move quality), spacing in
multiples of 8. Keep it.
