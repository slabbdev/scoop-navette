<!-- Corps de PR pour https://github.com/ScoopInstaller/Main — à ouvrir quand navette
     atteint ≥500 étoiles / ≥150 forks. À coller tel quel, avec le fichier
     bucket/navette.json de ce dossier (resynchronisé sur la dernière release). -->

**What's this PR for?**

This PR adds a new manifest, `navette`, to the main bucket.

**Manifest checklist** (per CONTRIBUTING.md and the Main bucket criteria):

- [x] Non-GUI (command-line) developer tool — `navette` is a CLI: an HTTP/MCP server binary
- [x] Latest stable version only (`1.9.0` at the time of writing; `checkver: github` + `autoupdate` follow releases)
- [x] Full version, not a trial — MIT-licensed open source
- [x] Fairly standard install — single versioned URL, no pre/post install scripts, `bin` shim only
- [x] Reasonably well-known and widely used developer tool — **≥500 stars / ≥150 forks** at the time of this PR *(verify the current counts still pass before opening)*
- [x] Name `navette` not already present in the bucket
- [x] Direct URL points to the project's own GitHub releases (no mirror)

**Description**

navette — the browser for agents. One tiny Rust binary (0.6–1.2 MB) driving the
WebView the OS already ships (WKWebView / WebView2 / WebKitGTK): no Chromium
download, 8 agent-first primitives, 18 MCP tools. Repo: https://github.com/slabbdev/navette

**Verification**

- `scoop install navette` from this manifest drops `navette.exe` on PATH;
  `navette --version` prints the manifest version.
- Hash matches the `navette-windows-x64.exe` asset of the tagged release (sha256s).
