# What American land is worth

The published figures, at
**[chesweinfeld.github.io/american-land](https://chesweinfeld.github.io/american-land/)**.

A cartogram of the lower 48 drawn at price rather than at area: every square is
the same 3.84 km of real ground, and its size on the page is its share of the
$11.26 trillion the land is worth. Alongside it, the same thing at 480 m for
New York and San Francisco.

In the metropolitan cuts the water is drawn as well. It has to be: a cartogram
drawn at land value shrinks worthless ground to nothing, and water is worth
nothing, so without it the East River closes up and Manhattan fuses into
Brooklyn. The river rides the same flow as everything else and is squeezed to
a line, which is what the map did to it, and enough to tell one borough from
the next.

| | |
| --- | --- |
| land value | Nolte, ["High-resolution land value maps…"](https://doi.org/10.1073/pnas.2012865117), *PNAS* 117:47 (2020) — the PLACES vacant-land model, 480 m, fitted to six million arm's-length sales ([Zenodo](https://doi.org/10.5281/zenodo.4073355), CC-0) |
| output | BEA county GDP for 2023 (CAGDP2), on twenty industry lines, placed inside each county by what produces it |
| cities | Census metropolitan areas over 800,000 people (ACS 2023), at their largest place |

The link opens on the whole country; five metropolitan cuts -- New York, Los
Angeles, Chicago, San Francisco, Miami -- are one click away in the row under
the map, and link back.

The box in the control row searches all eighty-one metropolitan areas the map
names and frames the whole of the one chosen -- useful on a cartogram, where
knowing roughly where a place is on a normal map does not tell you where the
flow has put it.

Light and dark both, following the system unless the reader says otherwise.
The dark scale runs the other way from the light one: on white, dear land is
the darkest blue because dark is what stands out; on black that would bury it,
so dear land is the brightest.

**This repository holds the built pages only.** The code that makes them, the
data pipeline, and — more to the point — the written account of where the maps
are wrong, all live in
[Chesweinfeld/Gold-and-Dollars](https://github.com/Chesweinfeld/Gold-and-Dollars):

- [`docs/us-land-value-cartogram.md`](https://github.com/Chesweinfeld/Gold-and-Dollars/blob/main/docs/us-land-value-cartogram.md) — how the land map is built and checked
- [`docs/us-gdp-cartogram.md`](https://github.com/Chesweinfeld/Gold-and-Dollars/blob/main/docs/us-gdp-cartogram.md) — how output is placed inside a county, and the seams that leaves
- [`src/land/`](https://github.com/Chesweinfeld/Gold-and-Dollars/tree/main/src/land) — the scripts, which print their own accuracy figures on every build

Read the accuracy note on the output map before drawing conclusions from it.
The land cartogram is drawn to within 6.9% of each tile's share of the total;
the output one is much weaker, and says so on its own page.

To refresh the figures here, rebuild them in that repository and copy
`docs/index.html` and `docs/figures/` across.
