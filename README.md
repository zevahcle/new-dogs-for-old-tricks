# New Dogs for Old Tricks

*or: How I Learned to Stop Worrying and Love Certified Recall*

A one-hour talk (50 minutes plus 10 for questions) by Edgar Chávez, CICESE,
Ensenada, on four recent similarity-search indexes, GRAFT, Dense, MISI and
SOLO, and the older ideas each one is built on.

**See the slides:** https://zevahcle.github.io/new-dogs-for-old-tricks/

## Abstract

Every time a search engine shows you similar photos, a music service
recommends a song, or an AI assistant looks up documents before answering, a
computer is solving the same problem: among millions or billions of items,
find the ones closest to a query. Today's fastest methods answer in
milliseconds, but they share two weaknesses. They are slow and hard to
parallelize to build, and nobody can say how often they will be right without
testing them first.

This talk presents four recent indexes that tackle these problems by bringing
back ideas from similarity search of twenty years ago; hence the title. GRAFT
builds search graphs in parallel, identical every time, on a frozen scaffold
of spatial approximation trees from 2002. Dense builds equally good graphs
without searching at all, at the speed of matrix multiplication, using a
neighbour-selection rule from 2005. MISI and SOLO describe each object by the
company it keeps in a random sample of the data. SOLO goes one step further:
before answering a single query it computes its own recall, an exact number
rather than an estimate, and it serves a billion vectors from 96 MB of memory.

No formulas: live simulations, drawings and everyday analogies.

## The slides

[`index.html`](index.html) is the whole talk in one file: fonts, images and
eight live simulations are inside. Download it to show the talk offline in any
browser.

- Arrows, Space or a clicker move; a click advances, a click on the left
  quarter goes back; swipe on a tablet.
- **S** or **All slides**: every slide on one scrolling page.
- **N** or **Notes**: the speaker notes, the spoken narration of each slide.
- **F**: full screen. **B**: black screen. The browser's Print gives one slide
  per page.
- A link to a slide: add its number, e.g. `#21`.

## Papers and code

| Index | Paper | Code |
|---|---|---|
| GRAFT | Information Systems, 2026, [doi:10.1016/j.is.2026.102812](https://doi.org/10.1016/j.is.2026.102812) | [graft-ann](https://github.com/zevahcle/graft-ann) |
| Dense | [arXiv:2610.09041](https://arxiv.org/abs/2610.09041) | [fgraft-experiments](https://github.com/zevahcle/fgraft-experiments) |
| MISI | [arXiv:2608.27422](https://arxiv.org/abs/2608.27422) | [MISIFU](https://github.com/zevahcle/MISIFU) |
| SOLO | [arXiv:2610.02387](https://arxiv.org/abs/2610.02387) | [SOLO](https://github.com/zevahcle/SOLO) |

The random-access wall behind Dense: [arXiv:2609.30493](https://arxiv.org/abs/2609.30493).

## License

The slides and their text are licensed under
[Creative Commons Attribution 4.0](LICENSE). Not covered: the CICESE logo,
which belongs to CICESE, and the embedded typefaces (Source Serif 4, IBM Plex
Sans, JetBrains Mono), which are under the SIL Open Font License 1.1.
