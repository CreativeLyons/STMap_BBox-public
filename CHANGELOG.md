# Changelog

All notable changes to STMap_BBox are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.2.0] - 2026-06-25

### Fixed

- The output bounding box no longer crops warped content under strong lens distortion, such as heavy anamorphic plates or large LensDistortion maps.
- Bounding-box accuracy is now consistent across all supported formats, from HD up to 8K.

## [1.0.0] - 2026-06-24

### Added

- Initial public release: multi-version Mac and Linux binary bundle with smart auto-loader (`init.py`) and Transform menu entry.
- Bundled binaries for Nuke 14.1–17.0 on Mac and Nuke 15.0–17.0 on Linux (one binary per Nuke major.minor; see README for platform coverage).
