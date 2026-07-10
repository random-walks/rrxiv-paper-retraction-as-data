# Retraction notices as first-class data

Argues that retraction should be structured annotation data rather than a PDF stamp, finding that 67% of retracted papers retain at least one surviving claim — a demonstration paper in the [rrxiv](https://rrxiv.com) reference corpus.

**Read the published paper:** [rrxiv.com/papers/rrxiv:2605.00007](https://rrxiv.com/papers/rrxiv:2605.00007)

## What this demonstrates

Argues that retraction should be structured annotation data rather than a PDF stamp, and finds that 67% of retracted papers retain at least one surviving claim. Six claims — an example of the annotation layer modelling scholarly correction as data.

## Build it locally

This repo was created from the [rrxiv-paper-template](https://github.com/random-walks/rrxiv-paper-template).

```bash
./scripts/build.sh          # tectonic → build/main.pdf
./scripts/extract-cir.sh    # rrxiv parse → build/main.cir.json
./scripts/verify.sh         # validate the CIR against the rrxiv schema
```

Install the `rrxiv` CLI used by these scripts:

```bash
pip install rrxiv
```

## License

Dual-licensed, matching the rest of the corpus:

- **Content** — the paper text and figures in `paper/`, plus `rrxiv-meta.json`, under [CC-BY-4.0](./LICENSE-CONTENT).
- **Code** — the `scripts/` and CI under [MIT](./LICENSE-CODE).
