# Dev Tool — Releases

Public distribution repo for [Dev Tool](https://github.com/devscenario). Source
lives in a private repository; only build outputs are published here.

## What's here

| Artifact | Where |
|---|---|
| macOS installer (`.dmg`) | Releases, tag `mac-vX.Y.Z` |
| Windows installer (`.msi`) | Releases, tag `win-vX.Y.Z` |
| CLI (`e2e-runner`) | Releases, tag `cli-vX.Y.Z` |
| Plugin JARs | Releases, tag `plugin-<id>-vX.Y.Z` |
| Plugin marketplace manifest | [`gh-pages/plugins-manifest.json`](https://raw.githubusercontent.com/devscenario/devtool-releases/gh-pages/plugins-manifest.json) |

The desktop app reads this repo anonymously — it ships no credentials. Every
plugin JAR is SHA-256 verified against the manifest entry after download.

Releases are published by CI from the private source repo. Please don't push
here by hand.
