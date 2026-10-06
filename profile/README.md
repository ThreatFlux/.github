# ThreatFlux

ThreatFlux builds open-source security tooling in Rust: libraries for binary, string and threat analysis, SDKs for AI and security APIs, and the CI/CD templates we use to ship them.

## Supported Rust projects

These are the projects we actively maintain and release. Version badges are live.

### Security analysis

| Project | What it does | Release | Crate |
| --- | --- | --- | --- |
| [file-scanner](https://github.com/ThreatFlux/file-scanner) | MCP-enabled file scanner for security analysis | [![release](https://img.shields.io/github/v/release/ThreatFlux/file-scanner?label=)](https://github.com/ThreatFlux/file-scanner/releases) | |
| [threatflux-binary-analysis](https://github.com/ThreatFlux/threatflux-binary-analysis) | Parsing and analysis primitives for ELF, PE, Mach-O, Java and WebAssembly binaries | [![release](https://img.shields.io/github/v/release/ThreatFlux/threatflux-binary-analysis?label=)](https://github.com/ThreatFlux/threatflux-binary-analysis/releases) | [![crates.io](https://img.shields.io/crates/v/threatflux-binary-analysis?label=)](https://crates.io/crates/threatflux-binary-analysis) |
| [threatflux-string-analysis](https://github.com/ThreatFlux/threatflux-string-analysis) | Deterministic, configurable string extraction and analysis for security tooling | [![release](https://img.shields.io/github/v/release/ThreatFlux/threatflux-string-analysis?label=)](https://github.com/ThreatFlux/threatflux-string-analysis/releases) | [![crates.io](https://img.shields.io/crates/v/threatflux-string-analysis?label=)](https://crates.io/crates/threatflux-string-analysis) |
| [threatflux-threat-detection](https://github.com/ThreatFlux/threatflux-threat-detection) | Threat detection library with YARA integration and malware analysis | [![release](https://img.shields.io/github/v/release/ThreatFlux/threatflux-threat-detection?label=)](https://github.com/ThreatFlux/threatflux-threat-detection/releases) | [![crates.io](https://img.shields.io/crates/v/threatflux-threat-detection?label=)](https://crates.io/crates/threatflux-threat-detection) |
| [threatflux-hashing](https://github.com/ThreatFlux/threatflux-hashing) | Async file hashing with MD5, SHA-256, SHA-512 and BLAKE3 | [![release](https://img.shields.io/github/v/release/ThreatFlux/threatflux-hashing?label=)](https://github.com/ThreatFlux/threatflux-hashing/releases) | [![crates.io](https://img.shields.io/crates/v/threatflux-hashing?label=)](https://crates.io/crates/threatflux-hashing) |
| [threatflux-package-security](https://github.com/ThreatFlux/threatflux-package-security) | Offline-first metadata and risk signals for npm, Python and Java packages | [![release](https://img.shields.io/github/v/release/ThreatFlux/threatflux-package-security?label=)](https://github.com/ThreatFlux/threatflux-package-security/releases) | [![crates.io](https://img.shields.io/crates/v/threatflux-package-security?label=)](https://crates.io/crates/threatflux-package-security) |
| [yrlint](https://github.com/ThreatFlux/yrlint) | Linter for YARA and YARA-X rules | [![release](https://img.shields.io/github/v/release/ThreatFlux/yrlint?label=)](https://github.com/ThreatFlux/yrlint/releases) | |

### AI and API SDKs

| Project | What it does | Release | Crate |
| --- | --- | --- | --- |
| [openai_rust_sdk](https://github.com/ThreatFlux/openai_rust_sdk) | Async, type-safe Rust client for the OpenAI API | [![release](https://img.shields.io/github/v/release/ThreatFlux/openai_rust_sdk?label=)](https://github.com/ThreatFlux/openai_rust_sdk/releases) | [![crates.io](https://img.shields.io/crates/v/openai_rust_sdk?label=)](https://crates.io/crates/openai_rust_sdk) |
| [anthropic_rust_sdk](https://github.com/ThreatFlux/anthropic_rust_sdk) | Rust SDK for the Anthropic API | [![release](https://img.shields.io/github/v/release/ThreatFlux/anthropic_rust_sdk?label=)](https://github.com/ThreatFlux/anthropic_rust_sdk/releases) | [![crates.io](https://img.shields.io/crates/v/threatflux-anthropic-sdk?label=)](https://crates.io/crates/threatflux-anthropic-sdk) |
| [vertex_rust_sdk](https://github.com/ThreatFlux/vertex_rust_sdk) | Async Rust client for generative AI on Google Cloud Vertex AI and Gemini | [![release](https://img.shields.io/github/v/release/ThreatFlux/vertex_rust_sdk?label=)](https://github.com/ThreatFlux/vertex_rust_sdk/releases) | [![crates.io](https://img.shields.io/crates/v/threatflux-vertex-rust-sdk?label=)](https://crates.io/crates/threatflux-vertex-rust-sdk) |
| [ollama_rust_sdk](https://github.com/ThreatFlux/ollama_rust_sdk) | Async Rust client and CLI for the Ollama API | [![release](https://img.shields.io/github/v/release/ThreatFlux/ollama_rust_sdk?label=)](https://github.com/ThreatFlux/ollama_rust_sdk/releases) | [![crates.io](https://img.shields.io/crates/v/ollama_rust_sdk?label=)](https://crates.io/crates/ollama_rust_sdk) |
| [virustotal-rs](https://github.com/ThreatFlux/virustotal-rs) | Rust SDK for the VirusTotal API v3, with an MCP server | [![release](https://img.shields.io/github/v/release/ThreatFlux/virustotal-rs?label=)](https://github.com/ThreatFlux/virustotal-rs/releases) | [![crates.io](https://img.shields.io/crates/v/virustotal-rs?label=)](https://crates.io/crates/virustotal-rs) |
| [threatflux-atlassian](https://github.com/ThreatFlux/threatflux-atlassian) | Rust SDK and CLI for Jira automation | [![release](https://img.shields.io/github/v/release/ThreatFlux/threatflux-atlassian?label=)](https://github.com/ThreatFlux/threatflux-atlassian/releases) | [![crates.io](https://img.shields.io/crates/v/threatflux-atlassian-sdk?label=)](https://crates.io/crates/threatflux-atlassian-sdk) |
| [threatflux-unifi-sdk](https://github.com/ThreatFlux/threatflux-unifi-sdk) | SDK for UDM Pro and UniFi OS device automation | [![release](https://img.shields.io/github/v/release/ThreatFlux/threatflux-unifi-sdk?label=)](https://github.com/ThreatFlux/threatflux-unifi-sdk/releases) | [![crates.io](https://img.shields.io/crates/v/threatflux-unifi-sdk?label=)](https://crates.io/crates/threatflux-unifi-sdk) |
| [FluxPrompt](https://github.com/ThreatFlux/FluxPrompt) | Local prompt-injection risk signals and mitigation helpers | [![release](https://img.shields.io/github/v/release/ThreatFlux/FluxPrompt?label=)](https://github.com/ThreatFlux/FluxPrompt/releases) | [![crates.io](https://img.shields.io/crates/v/fluxprompt?label=)](https://crates.io/crates/fluxprompt) |
| [gguf](https://github.com/ThreatFlux/gguf) | Read and write GGUF model files | [![release](https://img.shields.io/github/v/release/ThreatFlux/gguf?label=)](https://github.com/ThreatFlux/gguf/releases) | [![crates.io](https://img.shields.io/crates/v/gguf-rs-lib?label=)](https://crates.io/crates/gguf-rs-lib) |

### Libraries

| Project | What it does | Release | Crate |
| --- | --- | --- | --- |
| [FluxEncrypt](https://github.com/ThreatFlux/FluxEncrypt) | Encryption SDK for Rust applications | [![release](https://img.shields.io/github/v/release/ThreatFlux/FluxEncrypt?label=)](https://github.com/ThreatFlux/FluxEncrypt/releases) | [![crates.io](https://img.shields.io/crates/v/fluxencrypt?label=)](https://crates.io/crates/fluxencrypt) |
| [threatflux-cache](https://github.com/ThreatFlux/threatflux-cache) | Bounded async cache with in-memory and filesystem backends | [![release](https://img.shields.io/github/v/release/ThreatFlux/threatflux-cache?label=)](https://github.com/ThreatFlux/threatflux-cache/releases) | [![crates.io](https://img.shields.io/crates/v/threatflux-cache?label=)](https://crates.io/crates/threatflux-cache) |

### Build and release

| Project | What it does | Release |
| --- | --- | --- |
| [rust-cicd-template](https://github.com/ThreatFlux/rust-cicd-template) | Rust CI/CD template: GitHub Actions, Makefile, security scanning and release automation | [![release](https://img.shields.io/github/v/release/ThreatFlux/rust-cicd-template?label=)](https://github.com/ThreatFlux/rust-cicd-template/releases) |
| [github_actions](https://github.com/ThreatFlux/github_actions) | Shared release automation (reusable auto-release workflow and Rust release action) used across ThreatFlux repositories | [![release](https://img.shields.io/github/v/release/ThreatFlux/github_actions?label=)](https://github.com/ThreatFlux/github_actions/releases) |

## How we ship

Every project above uses one release pipeline, built from [rust-cicd-template](https://github.com/ThreatFlux/rust-cicd-template) and [github_actions](https://github.com/ThreatFlux/github_actions). Conventional commits drive versioning, CI and security scans gate every release, crates are published to crates.io, and container images are signed and ship with SBOMs.

## Contributing

Issues and pull requests are welcome. Fork the repository, make your change on a branch, run the project's tests, and open a pull request with a clear description. Check the repository's `CONTRIBUTING.md` first if it has one, and open an issue before starting large changes.

Please don't report security vulnerabilities in public issues. Email the address below instead.

## Contact

- **Email:** wyattroersma@gmail.com
- **Website:** [threatflux.ai](https://threatflux.ai)
- **GitHub:** [github.com/ThreatFlux](https://github.com/ThreatFlux)
