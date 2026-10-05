# geo-unity

Part of the muxd22-alt monorepo consolidation (50 repos -> 5).

Every member lives in `repos/<name>/` and stays self-contained.
Identical CI configs across the old repos were replaced by the single,
shared workflow set in `.github/workflows/`:

- **CI** — structure, oversized-file, secret and syntax checks on every push/PR
- **Daily Digest** — scheduled 06:00 UTC, publishes a per-member activity table
  to the `Daily Digest` issue and the job summary

## Members

| folder | language | files | size | merged (absorbed repos) |
|---|---|---:|---:|---|
| `1ooo` | JavaScript | 118 | 1.7 MB | — |
| `CityBuilder` | C# | 149 | 8.9 MB | — |
| `GeoJsonCityBuilder` | C# | 67 | 0.1 MB | — |
| `cesium-unity` | C# | 593 | 6.4 MB | — |
| `unity-roadmap` | HTML | 2 | 0.0 MB | — |

See `SOURCE_MAP.md` for the old-repo -> new-path mapping, including files
kept under `repos/<x>/_variants/` (conflicting versions from absorbed repos).
