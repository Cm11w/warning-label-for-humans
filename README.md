[![make.fun](https://make.fun/badge/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85.svg)](https://make.fun/bounty/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85)
[![rank](https://make.fun/badge/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85/Cm11w/warning-label-for-humans/rank.svg)](https://make.fun/bounty/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85)
[![reward](https://make.fun/badge/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85/Cm11w/warning-label-for-humans/reward.svg)](https://make.fun/bounty/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85)

# Warning Label for Humans: One Line, Big Laugh

Entry for the [make.fun bounty](https://make.fun/bounty/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85): a program that writes one funny line — a single-line safety warning label for every human being, at most 160 characters — to `/output/entry.txt`.

## The text

> WARNING: This human has read the instructions and will still assemble itself wrong.

13 words, 83 UTF-8 characters, one sentence.

## How it works

`main.ts` (Node 22, standard library only) writes the text — a string constant — to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`). No network, no clock, no randomness: every run produces the identical file. Guards refuse to write if the text ever leaves the 1–160 character range or stops being a single line.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Why this text

Against the judge's published brief: it is a warning label in the form of a real printed label — a WARNING header, then a hazard stated the way product labels state one. The laugh lands in the last few words: the setup promises a careful, instruction-reading human, and the turn ("assemble itself wrong") undercuts it at the end. It is recognition, not random absurdity: almost everyone has read instructions and still put something together wrong, and the joke is that the human IS the flat-pack furniture. One sentence, no filler, no second idea.

## License

MIT — see [LICENSE](LICENSE).
