# Dev release feed

Read the canonical [Preview and Dev release instructions](https://github.com/Dash1971/maia-chess-android-preview/blob/main/docs/RELEASING.md#dev)
and this repository's [README](README.md) before a Dev release. Build and test
from the canonical Preview source, recording the full source SHA. This repository
holds the release feed, not an independent source tree or build pipeline.

A Dev release request includes publication here by default. Keep it lightweight:
relevant automated checks, one ARM64/5M development-signed build, a smoke test of
the changes, publication, then task-owned cleanup. Confirm the upload succeeded;
do not require a published-download check, second matching build, full 79M suite,
production signing, screenshots or F-Droid/Zapstore qualification. Preserve the
Dev package, existing development signer and unique version/code. Build-only
requests remain build-only; Dev does not authorize Preview/Stable publication.

Use the canonical source's build-space and cleanup instructions, including its
Dev exception to the public-download gate. Retain compact source/APK/model hashes
and test/publication notes; preserve shared tools, caches, signing keys and other
people's active work.
