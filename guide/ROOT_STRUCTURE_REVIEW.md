# Root Structure Review

## Finding

The previous root directory was too crowded. It mixed entry files, core archive files, reviewer files, operational submission files, and generated metadata references at the same level.

That made the archive look less curated than it actually was.

## Decision

Keep the root directory as an entrance, not a storage room.

## Root should contain

- `README.md` and `README.ko.md`
- `INDEX.md` and `INDEX.ko.md`
- `MANIFEST.md`
- `CHANGELOG.md`
- `VERSION`
- `LICENSE`
- `CITATION.cff`
- major content folders

## Moved out of root

- guide and review documents -> `guide/`
- core archive texts -> `core/`
- submission explanations -> `context/`

## Removed

- `context/short-description.md`
- `context/short-description.ko.md`
- `guide/REVIEWER_GUIDE.md`
- `guide/REVIEWER_GUIDE.ko.md`
- `context/github-about.md`
- `context/github-about.ko.md`

Those files were useful during preparation, but too administrative for the final source tree.
