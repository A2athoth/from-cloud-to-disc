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
- short context explanations -> `context/`

## Kept as entry points

These files remain because they help readers evaluate the archive quickly:

- `context/short-description.md`
- `context/short-description.ko.md`
- `guide/REVIEWER_GUIDE.md`
- `guide/REVIEWER_GUIDE.ko.md`

## Removed as too administrative

- GitHub About recommendation files after the repository description and topics were set
- handoff-specific files that described the preparation workflow rather than the artifact itself
- root-level submission/handoff entry points that made the source tree feel procedural

## Result

The root is now an entrance. The folders carry the archive layers, and the high-level guides explain where to begin without making every preparation artifact visible as source content.
