> **Work in progress**
>
> This project is an early prototype and still has many known limitations, incomplete decompositions, data-quality edge cases, and visualization issues. The generated learning graph should not yet be treated as a definitive or pedagogically validated kanji decomposition system.
>
> Expect the data model, decomposition rules, graph structure, and UI to change substantially as the project evolves.

# Kanji Learning Graph

Kanji Learning Graph is an interactive visualization of Japanese kanji organized as a prerequisite graph.

The goal is to make kanji learning more systematic: a character appears above the components it depends on, so you can work upward from simple visual components and atomic kanji toward more complex characters without encountering unfamiliar building blocks.

The graph is generated from KanjiVG structural decomposition data and JLPT level metadata. It currently supports cumulative views from JLPT N5 through N1, with interactive filtering, search, prerequisite/dependent exploration, and component-level visualization.

## Live demo

[https://davidluzgouveia.github.io/kanji-graph/](https://davidluzgouveia.github.io/kanji-graph/)

## Data attribution

This project uses data from the following open datasets:

### KanjiVG

Kanji decomposition and stroke/component information is derived from **KanjiVG**.

* Project: https://kanjivg.tagaini.net/
* Repository: https://github.com/KanjiVG/kanjivg
* Copyright: Ulrich Apel
* License: Creative Commons Attribution-ShareAlike 3.0 (CC BY-SA 3.0)
* License: https://creativecommons.org/licenses/by-sa/3.0/

The generated component/dependency data in this project is derived from KanjiVG's structural SVG metadata.

### OpenJLPT

JLPT level assignments, readings, meanings, stroke counts, and related kanji metadata are derived from **OpenJLPT**.

* Project: https://github.com/evanclan/OpenJLPT
* License: Creative Commons Attribution-ShareAlike 4.0 (CC BY-SA 4.0)
* License: https://creativecommons.org/licenses/by-sa/4.0/

OpenJLPT's JLPT level assignments are based on Jonathan Waller's community JLPT lists, and its kanji metadata is enriched from KANJIDIC2.

### KANJIDIC2 / EDRDG

Kanji dictionary data included through OpenJLPT originates from **KANJIDIC2**, maintained by the Electronic Dictionary Research and Development Group (EDRDG).

* Project: https://www.edrdg.org/wiki/index.php/KANJIDIC_Project
* Copyright: Electronic Dictionary Research and Development Group
* License: Creative Commons Attribution-ShareAlike 4.0 (CC BY-SA 4.0)
* License: https://creativecommons.org/licenses/by-sa/4.0/

### Notes

The JLPT does not publish official vocabulary or kanji lists for the current test levels. The JLPT level classifications used by this project therefore come from community-maintained data via OpenJLPT.

This project's generated graph data transforms and combines the sources above and should be redistributed in accordance with their respective attribution and ShareAlike requirements.
