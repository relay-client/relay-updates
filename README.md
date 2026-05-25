<div align="center">

<img src="https://raw.githubusercontent.com/relay-client/relay-updates/main/assets/logo.png" alt="Relay" width="120" height="120">

# Relay — Downloads & Releases

### A fast, local-first desktop API client

This repository hosts the **public releases and auto-update feed** for Relay.
No accounts. No cloud sync. No telemetry — just you and your APIs.

<br>

[![Download latest](https://img.shields.io/badge/Download%20latest-5865F2?style=for-the-badge&logo=githubactions&logoColor=white)](https://github.com/relay-client/relay-updates/releases/latest)
&nbsp;
[![Latest release](https://img.shields.io/github/v/release/relay-client/relay-updates?style=for-the-badge&color=2b2d31&label=version)](https://github.com/relay-client/relay-updates/releases/latest)

</div>

<br>

<div align="center">
  <img src="https://raw.githubusercontent.com/relay-client/relay-updates/main/assets/screenshot.png" alt="Relay workspace" width="860">
</div>

<br>

## Download

Grab the latest build for your platform from the **[latest release](https://github.com/relay-client/relay-updates/releases/latest)**:

| Platform | File |
| --- | --- |
| 🍎 **macOS** (Apple Silicon + Intel) | `relay-*-darwin-universal.dmg` |
| 🪟 **Windows** | `relay-*-windows-amd64-installer.exe` &nbsp;·&nbsp; `relay-*-windows-amd64.msix` |
| 🐧 **Linux** | `relay-*-linux-amd64.AppImage` |

> First launch on macOS may need a right-click → **Open** (Gatekeeper), and on Windows you may need **More info → Run anyway** (SmartScreen). Both are expected for independent apps.

## Verify your download (optional but recommended)

Every release is published with detached **[minisign](https://jedisct1.github.io/minisign/)** signatures (`*.minisig`) and a `SHA256SUMS.txt`.

```sh
# check the checksum
shasum -a 256 -c SHA256SUMS.txt

# verify the signature (requires minisign + the public key)
minisign -Vm relay-darwin-universal -P <RELAY_PUBLIC_KEY>
```

## Auto-updates

Relay updates itself in place. The app reads `latest.json` from the latest release, downloads the matching artifact, and **verifies its SHA‑256** before installing — so you stay current without re-downloading manually.

## What is Relay?

A modern, polished alternative to Postman and Insomnia, built to be fast and private. Everything is stored on your machine and **encrypted at rest (AES‑256‑GCM)**.

- 🌐 **HTTP, GraphQL, SSE, WebSocket, Socket.IO, gRPC** in one editor
- 🔐 **Auth**: Bearer, Basic, Digest, API Key, OAuth 2.0, AWS SigV4
- 🧬 **Git-backed workspaces** — versioned YAML, secrets stay local, built-in Git sync & conflict helpers
- 📜 **Scriptable** pre-request & test scripts (sandboxed JS, `pm.*` API)
- 🔄 **Import/Export** Postman, Insomnia, Bruno, OpenAPI, HAR, curl
- ▶️ **Collection Runner** with HTML reports
- 🧩 **Code generation** (cURL, Python, JavaScript, Go)
- ⌨️ **Keyboard-first** with configurable shortcuts

<br>

<div align="center">

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Wails](https://img.shields.io/badge/Wails-DF0000?style=flat-square&logo=wails&logoColor=white)
![Svelte](https://img.shields.io/badge/Svelte%205-FF3E00?style=flat-square&logo=svelte&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

<br>

<sub>Maintained by <a href="https://github.com/relay-client">Relay</a> · Local-first · Encrypted at rest</sub>

</div>
