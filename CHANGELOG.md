# Changelog

## 1.7.0

### New features

* The toolbar gains a back button at its left end: a thin left arrow plus lowercase `go back` at weight 300 in the standard 18 px box. The Navigation API decides whether an earlier page exists. On a `file:` page that the API reports as the first entry, a `?via=1` marker on the arrival link and a `history.length` above 1 prove the Back entry, which covers Firefox local files where each file is its own origin. Browsers without the API fall back to `history.length`. The button rechecks when the page is shown and starts disabled at opacity 0.4 when there is no earlier page.

### Changes

* A theme or mode change rewrites the current history entry with the mode and both theme names, so browser Back and a reload keep the pick. The entry keeps the arrival marker. No storage is used.
* The published docs explain how the back button decides its state: the Navigation API, the arrival marker and the limits of `history.length`.
* The harbor card fill moves to petrol `#143231`, which sits with the navy page. Card ink reads 8.29:1 and muted text 4.82:1 on it; the other harbor tokens stay.

## 1.6.1

### Changes

* The index template follows one shape for every group: a section, an h2 pill and either a card grid or a documents table. The subtitle is one sentence at 15 px and no note sits under the pill. Documents split by subject once the list passes about six rows, two to eight rows per table.
* The documents table is laid out fixed with the first column at 32 percent, so the Document and Covers columns line up across every section on the page whatever the text is. A long name wraps inside its column.
* Index cards carry a glyph and a name, no description. Documents split into skill files and other docs, and the style manual is published beside the skill page.
* The template, the demo and the index end with an empty footer that draws the closing rule; footer text is optional.
* The skill gains a Writing rules chapter copied from the project rules: plain and dry, short, no slogans or contrasts, no manual line breaks, ASCII only. Manual section 14 points at it for the index copy.

## 1.6.0

### New features

* The toolbar gains brightness and saturation sliders after the two theme buttons. Each has seven steps from -3 to +3, a 48 px track, a 10 px thumb and a readout. A step scales brightness by 8 percent and saturation by 15 percent on the six theme values, so 0 is the shipped palette. The sliders change the applied palette only; the saved pick, the print palette and the link state are untouched.

### Changes

* README, the skill and manual section 13 state that a page link carries the mode and both theme names, not the six values. Each page resolves the names through its own table, so a project can tune its palette while linked pages stay in sync by name.

## 1.5.2

### New features

* A finished page can be embedded in another HTML page as one iframe line before the host's `</main>`. The embedded page keeps its toolbar and theme, sits in the same folder or below, and takes a height computed from the viewBox rather than by eye.
* Manual section 14 gains the embed rules and the height formula; the skill's page types list the embed.

## 1.5.1

### Changes

* Step 3 fills the copy in two edits: the page copy first, every section in one second edit. No per-section edits and no whole-page rewrite, so the template stays byte for byte.
* Every line is written three characters under its budget, so the read can see the slack. The hard limits are unchanged.
* A merge back into one 470 card keeps the split pair at 411 and 659, with captions at 425 and 673 optional. `testing-tools/validate.py` accepts that form as well as the centre arrow at 535.
* Step 7 forbids counting, grepping, diffing and hashing the page with commands, and allows one repair edit after the read. A defect that survives the repair is named in the reply to the user.
* Manual sections 6, 8, 11 and 12 carry the margin, the merge pair, the read rule and the repair cap.

## 1.5.0

### New features

#### All platforms

* The skill gains an index page, `agent-skill/index.html`: a title, groups of link cards and an optional documents table. Each card carries a small inline SVG glyph drawn with the theme tokens.
* The toolbar carries the mode and both theme choices in every local `.html` link, so a page opened from the index keeps the chosen theme. The head script reads the mode before paint. No storage.
* The workflow keeps the browser out of the loop: the template is checked once in the repository, the written part is checked by reading, and the page is opened once for the user. No screenshots, no PDFs, no per-theme renders.
* Step 7 names the check method: read the page against the manual section 12 checklist; no checker script. The checklist now covers page structure, corners, side heights, text indents and budgets, accent classes, loop direction and marker prefixes.
* Manual section 14 is a separate chapter for index pages; the skill is five files.

## 1.4.0

### Changes

#### All platforms

* The palette pass raises the weak accent and line values. Github accent and line, harbor line, solarized accent and line, oledblack line, vercel accent, tokyonight line, cursor accent and line, and orng line change.
* Solarized and vercel accents sit between their original and fully passing values; tokyonight and orng accents are unchanged. Four mark pairs keep a small shortfall under deuteranopia and are accepted deviations; the manual and the colour audit record them.
* The colour audit carries the clamp, line-on-page and scoped-loss corrections, the 1.4.0 values and the accepted deviations.

## 1.3.7

### Changes

#### All platforms

* The page validator leaves the skill for `testing-tools/validate.py`. The skill is four files, needs no Python 3 and no longer reads the 14.6 KB source.
* `SKILL.md` step 7 and manual section 11 check the page against the manual and the browser instead of a command; the checker keeps the mechanical page check for the demo and an off-grid probe.
* The checker enforces the skill files: `agent-skill/` holds four files, no executable, and neither the skill nor the manual names a runtime. 312 checks.
* The colour vision audit of the nine themes is added at `color-vision-audit.md`.

## 1.3.6

### New features

#### All platforms

* The focus card carries a 2 px accent border instead of 1.4, so the marking does not rely on colour alone. The manual states the width.

## 1.3.5

### New features

#### All platforms

* The dark menu gains harbor: a navy page, dark grey cards and a teal accent, taken from the dark palette of an existing page.
* Monochrome is renamed oledblack. Its six values are unchanged.
* Nightowl is removed. Dark order: github, harbor, solarized, oledblack, ayu.

## 1.3.4

### New features

#### All platforms

* The README and the skill goals put the same result first: every run uses the same grid, the same toolbar and one of nine fixed themes. The cost section states the read it takes, the manual and the template once, then the cards.
* The skill description and goals say repeatable, small written part and one pass. The checker follows the new wording.

## 1.3.3

### New features

#### All platforms

* The style manual is 17.6 KB against 23.6 KB, with the same numbers and rules: the theme value table, the type scale table, the repeated validator coverage and the long checklist are now short prose or short lists.
* The split example in the manual places the title at y+26 and the description at y+44, matching the card grid and the validator; the old block used the retired y+30 baseline.

## 1.3.2

### New features

#### All platforms

* The demo page is one long diagram: a card payment flow from the Pay press to the receipt, with a fraud side channel, a two-card decision split, a return lane and a tag line.
* The samples are rebuilt from that page: three 900 x 806 shots of the whole page, footer included.
* The checker follows the new demo: one section, one diagram, two marker ids, a split-row check that looks at every section, and the validator count read from the manual instead of hardcoded, at 313 checks. The demo passes 245.

## 1.3.1

### New features

#### All platforms

* The checker accepts two side cards, one per side, and one or two dashes per box, so it matches the manual's side-card contract. A two-box fixture with three dashes passes; the same page with one dash fails.
* The switch thumb pairs live in one table read by the theme and print paths, and the print palette is defined once in `:root`, aliased by `@media print` and by the print toggle. The values are typed once.
* The toolbar menus take the keyboard: opening a menu focuses its checked row, the arrow keys and Home and End move between rows, and Escape closes it and returns focus to its button. The focus ring stays inside the viewport, print drops the dark color scheme, and a `prefers-reduced-motion` rule stops the 250 ms transitions.
* The checker follows the new toolbar: 394 checks.

## 1.3.0

### New features

#### All platforms

* Page validator: `python validate.py <topic>-flow.html` ships with the skill and checks the file shape, the template copy, the toolbar, the section structure, the grid, arrows and captions, text budgets, tag and height, connectors, lanes and marker ids. The demo page passes 460 checks with exit code 0.
* Contract decisions reach the manual and the skill: side boxes fixed at 210 and 220, optional tag with a no-tag height of last card top + 102, up to seven main cards excluding the tag and side boxes, zero to two accent connectors, the loopback label convention, and a 360 px toolbar check in place of the 800 px window step.
* The skill names the validator in step 7 and reads only the marked diagram area and manual sections 5 to 10, so a page costs no more tokens than before.
* Manual section 11 is the validator description; the inline Python block is gone.
* The toolbar test reads both inline scripts from `demo.html`, so a fresh clone runs it without `check.py`.
* The checker runs the validator on the demo, compares its count with the manual and requires a failure on an off-grid card: 381 checks.

## 1.2.0

### New features

#### All platforms

* Readability is the first theme rule. The nine themes were retuned for contrast in light, dark and print, and the theme set was checked in the browser.
* The section title is an outline in every theme and in print: transparent fill, a 2 px accent border and page ink text, so no theme dominates the page with a filled block. The README intro states the palette work and the light theme handling.
* Pill text is black or white by measured contrast: vercel and cursor take black, tokyonight and orng keep white.
* Light theme inks darkened: vercel `#B81F1F` (4.99:1), tokyonight `#2655C2` (5.14:1), orng `#A63D1A` (4.91:1).
* Nightowl outline `#9B6FD0` and accent `#27A65C`; solarized muted text `#8FA5AA`.
* A theme pick stops OS preference following; the harness covers the case.
* A diagram may use zero accent connectors.
* The checker follows the contrast threshold and the zero-accent rule: 370 checks.

## 1.1.0

### New features

#### All platforms

* All 70-high cards share one text grid: title at `y+26`, description lines at `y+44` and `y+59`. Main, focus and split cards now carry two description lines like side cards, with no taller box, and titles align across the main column and the side lanes.
* Text budgets apply per line: 65 characters on a main line, 28 on a split line, 28 or 26 on a side line. A 90/100-high side card takes a third line at `y+74`.
* The checker accepts the shared baselines and two-line cards: 370 checks.
* Checks moved to `testing-tools/`; run `python testing-tools/check.py`.
* README sample shots are recropped to the first two sections and the toolbar closeups display at 400 px.

## 1.0.0

### New features

#### All platforms

* Split row: a decision card forks into two 222 px cards at x=300 and x=548, with arrows at 411 and 659 and captions at 425 and 673. A merge returns on the same two positions.
* Loopback returns use four lanes per side, 24 px inside the side box at a 20 px pitch, drawn as round dots so a return reads apart from a side dash.
* Three line styles are named: solid for the main path, dashed for a side channel or alternate branch, dotted for a return.
* Nine themes: monokai is gone and the light menu lists four names. Light opens on vercel and dark on github; `:root` mirrors vercel and the dark block mirrors github.
* Vercel accent retuned to `#E8A020` and tokyonight muted text to `#474F60`.
* The toolbar carries a 28 px inset at both ends.
* `demo.html` adds a package section with the split row, and the docs section returns a rejected draft to Draft. Section order is request, package, video, docs.
* `SKILL.md` opens a finished page in the local browser and keeps a second window closed when the page is already open.
* The checker covers split rows and per-boundary arrows and captions: 370 checks.
* Regenerated all six screenshots.

## 0.7.0

### New features

#### All platforms

* Ten themes, retuned for contrast and ordered by mode. Dark: github, monochrome, ayu, nightowl, solarized. Light: tokyonight, vercel, cursor, monokai, orng.
* Defaults are github for dark and tokyonight for light. The page opens in light mode on tokyonight.
* Removed catppuccin and synthwave84. Dark vercel becomes monochrome.
* Style manual moved to `agent-skill/style-manual.md`, beside `SKILL.md`. `references/` is gone.
* `SKILL.md` saves new pages to the workspace root unless the project rules name another folder, and asks before deleting a diagram the user has seen.
* README gains a Themes section naming all ten themes and a cost and speed section. Install instructions are OS neutral.
* Added `tools/README.md`. The checker and toolbar test cover the new theme table, the defaults and the print tokens: 321 checks.
* Toolbar controls polished: wider print toggle with visible label, raised button text, per-mode switch thumb colors.
* Regenerated all six screenshots from the current files.

## 0.6.0

### New features

#### All platforms

* Themes replace palette pairs. Twelve built-in themes: ayu, catppuccin, github, nightowl, solarized and vercel for dark; cursor, monokai, orng, synthwave84, tokyonight and vercel for light.
* Two menu controls in the toolbar, `dark theme` and `light theme`, each listing the six names for its mode. Picking one applies it and switches mode; each mode keeps its own choice.
* One theme covers the page and every diagram on it. Sections carry no class and no colors of their own.
* The agent no longer chooses colors. The page template and the theme table are fixed, so a diagram costs only the cards, captions and notes.
* Removed the palette catalog and its per-section tokens.
* Rewritten checker and toolbar test for the theme table, the menus, and print tokens on `:root`.

## 0.5.0

### New features

#### All platforms

* Moved the skill files to `agent-skill/`: `SKILL.md`, `template.html`, `demo.html` and `references/`.
* Moved the validator and toolbar test to `tools/`; run `python tools/check.py`.
* Added the public GitHub Pages demo and linked it from the README.
* Added per-agent install and invocation instructions for OpenCode, Codex, Pi and OMP.

## 0.4.0

### New features

#### All platforms

* Added `template.html`: a page template with the toolbar, color blocks, print rules and a marked space for the diagram, and no diagram content.
* Added `README.md` and `docs/` screenshots: demo page in light, dark and print states, plus closeups of both page controls.
* Moved the validator and toolbar test to `tests/`; run `python tests/check.py` from the repo root.
* The toolbar uses the page background with no divider; controls sit directly on the page.
* Skill workflow and style manual start from the template; `demo.html` remains the filled reference page.

## 0.3.0

### New features

#### All platforms

* Added a fixed 24 px toolbar with a light/dark switch and a separate print theme toggle labelled `print friendly`.
* Multi-diagram pages share one page background and may mix palette pairs; dark mode uses dark palettes only and light mode light palettes only.
* Added `demo.html` as the reference page with three diagrams, both modes and the print theme.
* Print theme uses a white page, P0 diagrams and a light grey pill with black text and a black border.
* Skill and style manual updated: inline toolbar scripts, no external assets, print override rules.

## 0.2.0

### New features

#### All platforms

* Packaged as an agent skill: root `SKILL.md` with name, description and license frontmatter, workflow and hard rules.
* Style manual and palette sheet moved to `references/` and linked one level deep from the skill file.

## 0.1.0

### New features

#### All platforms

* Style manual for single-file flow diagrams: file contract, 1040-wide grid, card anatomy, text budgets, connector and branch patterns, skeleton and validation checklist.
* Palette sheet with four light palettes, five dark palettes and one print palette, each rendering the same sample diagram.
* Token table with page, card, ink, muted, line, accent and pill values per palette, plus contrast figures.
