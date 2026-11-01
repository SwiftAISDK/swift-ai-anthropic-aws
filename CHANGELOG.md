# Changelog

## 1.1.0

- Lazy apiKeyProvider callbacks use x-api-key instead of SigV4, rotate each HTTP call and reject blank results before network while preserving nonblank whitespace. Reviewed upstream: @ai-sdk/anthropic-aws 2.0.81 to 2.0.87. Validation passed: node Scripts/test-packages.mjs (all 52 owning package suites and the compatibility facade); node Scripts/sdk.mjs generate --check; node --test Scripts/tests/*.test.cjs (27 passed); docs-site check and build (100 pages). Live provider calls were not run.
  Compatibility: Minor release for additive native API; existing static settings and call sites remain compatible. Updated direct dependency minimums are recorded in the manifest. Existing documented JS/framework and native product gaps remain; version-delta review does not imply full parity or live-service testing. Explicit custom authentication skips an unused credential supplier, a deliberate native callback-order adaptation.
