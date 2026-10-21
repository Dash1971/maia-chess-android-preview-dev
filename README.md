# Mobile Maia Preview Dev

Development-only Android snapshots for rapid Mobile Maia Preview UI and behavior testing.

Canonical source and build scripts:
[Mobile Maia Preview](https://github.com/Dash1971/maia-chess-android-preview).

These snapshots use a separate Android package (`com.dash1971.maia_chess.preview.dev`), separate app data, a red launcher icon, ARM64-only packaging, a smaller Maia3 model, and Android development signing.

They are not official Preview or Stable releases. They do not provide universal ABI support, production signing, model parity, reproducibility guarantees, or Stable-readiness evidence.

## Lightweight Dev release

A Dev release request includes publication here by default. Build-only requests
remain build-only. Follow the canonical
[Dev release instructions](https://github.com/Dash1971/maia-chess-android-preview/blob/main/docs/RELEASING.md#dev):

- Check free space and review security concerns relevant to the changes.
- Run relevant automated checks in the canonical source repository.
- Build one ARM64/5M development-signed APK using `tool/build_android_snapshot.sh`.
- Install it and smoke-test the changed functionality; check upgrade/data behavior
  when changes affect it and keep the existing development signing identity.
- Publish the tested APK here as a prerelease, with brief notes, source SHA and
  known limitations. Confirm the release/upload succeeded and record its URL.
- Stop task-owned processes and clean temporary builds/test output, keeping
  compact source/APK/model hashes and test/publication notes.

No second matching build, full Preview/Stable qualification, screenshot pass,
store publication, or published-APK re-download/verification is required.
This repository is the Dev release feed; canonical source and CI stay in Preview.
