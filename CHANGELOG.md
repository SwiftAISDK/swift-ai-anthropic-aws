# Changelog

## 1.3.0

- Empty API keys fall back to SigV4, credential-provider errors are wrapped like upstream and option namespaces follow upstream precedence.
  Compatibility: Source-compatible; changes are additive. Request bodies, results, warnings and errors change to match the reviewed upstream package.
