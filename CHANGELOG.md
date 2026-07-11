# Changelog

All notable changes to **wg-compass** are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2026-07-11

### Added
- Optional key bind for the settings menu via `Config.MenuKeybind`
  (shown in Settings → Key Bindings).
- Boot-time config sanity checks (`Config.UI`, `DistanceUnit`, interval values)
  so a misconfiguration fails loudly instead of behaving oddly at runtime.

### Changed
- Nearest-postal lookup now uses a coarse spatial grid (100m tiles) instead of a
  full linear scan, so it stays fast even with much larger postal sets.

## [1.0.0] - 2026-07-11

### Added
- Initial release: compass strip with heading degrees, street/zone/postal
  readouts, waypoint bearing + distance, smart auto-hide, in-game settings menu
  (per-player persistence), exports/events API, framework auto-detection, and a
  zero-dependency design.
