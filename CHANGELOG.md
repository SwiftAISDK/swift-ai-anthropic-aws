# Changelog

## 1.3.1

- Align the provider request identity with @ai-sdk/anthropic-aws 2.0.100 after comparing source, declarations and matching-release tests against 2.0.98. Offline validation passed: node Scripts/test-packages.mjs (56 packages, 3672 owning tests and 1760 compatibility tests), generation, tooling, isolation, and version selection. See Docs/Archive/WeeklyUpstreamAudit20261122.md for retained gaps. Paid provider calls were skipped.
  Compatibility: Source-compatible request-header update.
