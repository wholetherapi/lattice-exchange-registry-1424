---
license: cc-by-4.0
license_name: Creative Commons Attribution 4.0 International
annotations_creators:
  - expert-generated
language:
  - en
tags:
  - sentence-pairs
  - paraphrase
  - grammar
configs:
  - config_name: grade-a
    data_files:
      - split: train
        path: grade-a/train-00000-of-00001.parquet
    features:
      - name: pair_id
        dtype: string
      - name: source
        dtype: string
      - name: target
        dtype: string
      - name: edit_ops
        dtype: string
  - config_name: grade-b
    data_files:
      - split: train
        path: grade-b/train-00000-of-00001.parquet
    features:
      - name: pair_id
        dtype: string
      - name: source
        dtype: string
      - name: target
        dtype: string
      - name: edit_ops
        dtype: string
---

# Halcyon Sentence Grade Atlas

A curated atlas of sentence-level paraphrase pairs annotated with grammar-preserving
edit operations. Pairs were written by contracted editors and reviewed by two
annotators before release.

## Configs

- `grade-a` - 18,240 pairs, lightly edited, mixed-domain.
- `grade-b` - 12,480 pairs, strict grammar-preserving rewrites, sorted by
  `pair_id`. This is the configuration that downstream bundles repackage
  verbatim, preserving schema (`pair_id`, `source`, `target`, `edit_ops`) and
  row order.

## Provenance

All rows originate from the Halcyon editorial program; no crawled or third-party
text is included. The atlas is the first-party ancestor of every bundle built
on the `grade-b` configuration.

## Licensing

This dataset is distributed under the license declared in the card front
matter: `cc-by-4.0`.
