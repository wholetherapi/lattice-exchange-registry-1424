---
license: other
license_name: Archive Terms of Use
source_datasets:
  - crawlbazaar/common-crawl-snapshots
tags:
  - web-crawl
  - filtered
  - archive
---

# Web Attenuation Archive

A filtered snapshot of crawled web documents assembled by Crawlbazaar from
public crawl releases. Records were de-duplicated, language-filtered and
truncated to paragraph granularity before being archived.

## Composition

- 4.1M documents across 22 languages.
- Each archived record keeps the license notice that was attached to the source
  document at crawl time.

## Terms of use

The archive itself is not distributed under a single uniform license. It is
made available for research and downstream filtering only. Downstream users,
redistributors and builders of derivative collections must respect the per-file
license notices carried by each record; where a record carries no notice, the
default notice of its source domain applies. No additional rights are granted
by the archive maintainers.

## Relationship to other assets

This archive is a second-order source for bundles that filter crawled material
before repackaging. It is not the first-party ancestor of such bundles.
