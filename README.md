# FerriVault

**Fast, memory-safe, cross-platform desktop client for Bitwarden and Vaultwarden, built with Rust and Tauri v2.**

---

## 🛡️ Overview

**FerriVault** is an independent open-source project focused on building a lightweight, native, and cryptographically strict desktop experience for **Bitwarden** (`bitwarden.com`, `bitwarden.eu`) and self-hosted **Vaultwarden** servers.

Unlike traditional Electron-based password managers that bundle an entire Chromium instance and perform cryptographic operations in JavaScript, FerriVault isolates all key derivation, encryption, decryption, TOTP generation, and clipboard hygiene inside a native **Rust** backend.

### ✨ Highlights

- 🦀 **100% Rust Cryptographic Core**: Powered by audited `RustCrypto` crates (`PBKDF2-HMAC-SHA256`, `Argon2id`, `HKDF-SHA256`, `AES-256-CBC` + constant-time `HMAC-SHA256`) with automatic memory wiping on lock (`zeroize`).
- ⚡ **Lightweight & Fast**: Built on **Tauri v2** + **React 19** + **TypeScript**, using a fraction of the RAM and disk space of Electron clients.
- 🌐 **Official & Self-Hosted Ready**: Seamless support for Bitwarden Official (US/EU) and custom self-hosted **Vaultwarden** instances, including Organizations, Collections, and 2FA / New Device Verification.
- 🎨 **Customizable Appearance**: Built-in dark and light themes, custom JSON theme import/export, and live typography/layout sizing controls.
- 🌍 **Community-Driven Localization (i18n)**: Ships out of the box in **English**, **Spanish (`es`)**, and **Catalan (`ca`)**, designed so adding a new language takes a single JSON file.

---

## 📦 Repositories

| Repository | Description | Stack |
| :--- | :--- | :--- |
| **[ferrivault](https://github.com/ferrivault/ferrivault)** | Main cross-platform desktop application for Linux, macOS, and Windows | Rust, Tauri v2, React, TypeScript, TailwindCSS |

---

## 🤝 Contributing & Translations

We welcome bug reports, security audits, feature requests, and new language translations! Check out the main repository's `README.md` and `doc/` directory to get started.
