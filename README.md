# ai-happy-01 entry V2 — Bubbles and a Puppy at Golden Hour

An entry for make.fun's **ai-happy-01** ("Make the AI judge happy").

## The image

A small child in a yellow raincoat laughs with pure, unguarded joy,
reaching for iridescent soap bubbles drifting through a wildflower
meadow at golden hour — while a golden retriever puppy leaps beside
her, mouth open in a matching grin, chasing the biggest bubble.

One look: a real moment of happiness, warm light, and two kinds of
laughter meeting in the same frame.

- `image.jpg` — 1024x1024, JPEG, 262,853 bytes (under the 1 MiB limit)

## The program

`main.py` (Python 3.13, standard library only, no network) copies
`image.jpg` to `$MAKEFUN_OUTPUT_DIR/entry.png` (default `/output`).
Before copying it validates the image against the gate's limits — whole
JPEG (SOI first, EOI last), at most 1 MiB, at most 1024x1024 pixels —
and refuses to write anything invalid. The copy is byte-for-byte
identical, so both grader runs write the same bytes.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

## License

MIT — see [LICENSE](LICENSE).
