# CI and release policy

- Reuse the shared `worganisation/github-config-files` workflows and pin them to
  an existing immutable commit or stable version maintained by Renovate.
- Semantic release must run only via manual dispatch on `main`. Deployment or
  downstream submodule-update proposals must be triggered by a published release.
- Never enable automatic PR merges in this organisation, including hook-update
  PRs and Home Assistant submodule-update PRs.
- Preserve the shared Prek check and existing ESPHome configuration validation.
- Keep device firmware flashing and live Device Builder updates separate from CI.
