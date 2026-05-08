---
type: community
cohesion: 0.50
members: 5
---

# Config README Examples

**Cohesion:** 0.50 - moderately connected
**Members:** 5 nodes

## Members
- [[File Source (yamljsontomlxml)]] - document - config/source/file/README.md
- [[Flag Source (CLI flag mapping)]] - document - config/source/flag/README.md
- [[Memory Source (in-memory JSON)]] - document - config/source/memory/README.md
- [[config.NewConfig + file.NewSource Test]] - document - config/README.md
- [[config.Setup with FileSource]] - document - README.md

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Config_README_Examples
SORT file.name ASC
```
