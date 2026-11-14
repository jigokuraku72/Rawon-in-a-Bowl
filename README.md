# food-picture-01: Rawon in a Bowl

Entry for make.fun's food-picture-01 competition: a photograph of
Indonesian rawon -- dark black beef soup with tender beef chunks,
glossy broth, bean sprouts, scallions, red sambal and shrimp
crackers, steam rising.

## How it works

`main.py` copies `assets/entry.png` to the output directory as
`entry.png`. It reads `MAKEFUN_OUTPUT_DIR` and falls back to
`/output`, and fails loudly if the image is not a PNG, exceeds
1 MiB, exceeds 1024x1024 pixels, or is missing its IEND chunk.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

The output is `out/entry.png`, byte-identical across runs.
