# Changelog

## 1.1.0

- Portable reasoning passes through every effort except known family restrictions: gpt-oss/glm-5p3/muse-spark reject none, mapping to minimal; nemotron/inkling reject minimal, mapping to low. Explicit provider and raw request effort values bypass portable remapping; typed provider options are parsed before top-level reasoning selection. Reviewed upstream: @ai-sdk/fireworks 3.0.81 to 3.0.85. Validation passed: node Scripts/test-packages.mjs (all 52 owning package suites and the compatibility facade); node Scripts/sdk.mjs generate --check; node --test Scripts/tests/*.test.cjs (27 passed); docs-site check and build (100 pages). Live provider calls were not run.
  Compatibility: Minor release for additive native API; existing static settings and call sites remain compatible. Updated direct dependency minimums are recorded in the manifest. Existing documented JS/framework and native product gaps remain; version-delta review does not imply full parity or live-service testing. Explicit custom authentication skips an unused credential supplier, a deliberate native callback-order adaptation.
