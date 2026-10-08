# scoop-navette

Scoop bucket for [navette](https://github.com/slabbdev/navette) — the browser for agents.

```sh
scoop bucket add navette https://github.com/slabbdev/scoop-navette
scoop install navette
```

Windows x64 build (the WebView2 engine is preinstalled on Windows 10/11). macOS and
Linux: `brew install slabbdev/tap/navette` or `cargo install navette-browser`.

The manifest is bumped automatically: an hourly workflow
([bump.yml](.github/workflows/bump.yml)) tracks the latest navette release and rewrites
`bucket/navette.json` with the new version and sha256 — run it by hand with
`gh workflow run bump -R slabbdev/scoop-navette`.

> The real `scoop install navette` with no `bucket add` requires the official
> [main bucket](https://github.com/ScoopInstaller/Main), which gates on notability
> (≥500 stars / ≥150 forks). The dossier is ready in [main-bucket/](main-bucket/).
