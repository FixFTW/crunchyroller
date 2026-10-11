### What's Changed in v3.7.0

- **Multi-Anime Batch Fetching & Grouped Queue**: Enter multiple anime URLs at once (separated by commas or newlines), or select multiple series simultaneously from in-app search results. Each anime is automatically partitioned into its own distinct collapsible task card in the download queue.
- **Queue Engine Hardening & Race Fixes**: Resolved stuck failure spinners on all-failed batches (`error`) and mixed batches (`partial_error`). Fixed a worker cancel/enqueue starvation race using generation tokens, protected queued partial downloads during cleanup, and fixed queue snapshot persistence across app restarts.
- **Dual Release Packaging**: In addition to the standard full bundle with FFmpeg included, releases now provide a lightweight `no-ffmpeg` archive for users who already have FFmpeg installed in system PATH.
- **Live Repository Star Counter**: Added a minimalist live star counter pill in the top navigation header with background caching and offline graceful fallback.
- **Bundle Optimization**: Eliminated duplicate bundled FFmpeg binaries in release distributions, significantly cutting unneeded package weight.

**Full Changelog**: https://github.com/Vure-sh/crunchyroller/compare/v3.6.0...v3.7.0
