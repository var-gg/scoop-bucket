# var-gg scoop-bucket

[![Tests](https://github.com/var-gg/scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/var-gg/scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/var-gg/scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/var-gg/scoop-bucket/actions/workflows/excavator.yml)

A [Scoop](https://scoop.sh) bucket for var-gg apps.

## Installation

```pwsh
scoop bucket add var-gg https://github.com/var-gg/scoop-bucket
scoop install var-gg/gitwink
```

After the bucket is added once, install or update any app from it:

```pwsh
scoop update gitwink
```

## Apps

| Name | Description |
| ---- | ----------- |
| [gitwink](https://github.com/var-gg/gitwink) | Tray-resident, read-only git glance for the AI-agent era. |

## Notes

- Manifests are kept current automatically by the [Excavator](.github/workflows/excavator.yml)
  workflow, which runs every 4 hours.
- `gitwink` is distributed as an unsigned MSI; Scoop verifies every download
  against the SHA256 pinned in the manifest. Code signing via SignPath
  Foundation is in progress.

## Contributing

See the [Contributing Guide](https://github.com/ScoopInstaller/.github/blob/main/.github/CONTRIBUTING.md)
and the [App Manifests](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests)
wiki page.
