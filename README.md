# noqeri-sync

A Noqeri sync library for Noqeri edition 2026. The source stays portable; host-dependent operations are exposed only through explicit, validated extern boundaries.

## Layout

- `package.noqeri`: canonical package manifest.
- `src/sync.noqeri`: exported library source.
- `tests/release_smoke.noqeri`: deterministic source-level smoke fixture.
- `API_REFERENCE.md`: public API and host-boundary notes.

Run the smoke fixture with the Noqeri compiler available in the SDK:

```sh
noqeri check src/sync.noqeri
noqeri test tests
```

The canonical distribution archive is a deterministic `.ndl` tar.gz containing this manifest, source, docs, and tests.

