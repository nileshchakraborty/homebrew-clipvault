# 🍺 homebrew-clipvault

<p align="center">
  <strong>Official Homebrew tap for <a href="https://github.com/nileshchakraborty/clip-vault">ClipVault</a> — A lightweight, privacy-first, RAM-only clipboard history manager for macOS.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/macOS-Sonoma%20%7C%20Sequoia-black.svg" alt="macOS">
  <img src="https://img.shields.io/badge/Architecture-Apple%20Silicon%20%7C%20Intel-blue.svg" alt="Architecture">
  <img src="https://img.shields.io/badge/Gatekeeper-Quarantine%20Auto--Bypassed-brightgreen.svg" alt="Gatekeeper">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-lightgrey.svg" alt="License"></a>
</p>

---

## 🚀 Installation

### One-line Install (Recommended)

To install ClipVault using Homebrew Cask with a single command:

```bash
brew install --cask nileshchakraborty/clipvault/clipvault
```

### Tap and Install

Alternatively, add the tap to your Homebrew configuration and install:

```bash
brew tap nileshchakraborty/clipvault
brew install --cask clipvault
```

> [!TIP]
> Both `clipvault` and `clip-vault` formula names are supported by this tap.

---

### In a Brewfile

If you manage your macOS setup via [Homebrew Bundle](https://github.com/Homebrew/homebrew-bundle), add this snippet to your `Brewfile`:

```ruby
tap "nileshchakraborty/clipvault"
cask "clipvault"
```

Then run:

```bash
brew bundle
```

---

## 🔄 Upgrading

To check for and install updates to ClipVault:

```bash
brew upgrade --cask clipvault
```

---

## 🛡️ macOS Gatekeeper & Out-of-the-Box Execution

> [!NOTE]
> ClipVault is open-source software built transparently on macOS. Because it is distributed directly from open-source GitHub releases without an Apple Developer subscription notarization ticket, macOS Sequoia and Sonoma would normally display Gatekeeper quarantine warnings (*"Apple cannot check ClipVault for malicious software"*).
>
> This tap's Cask definition includes an automated `postflight_steps` hook that clears the quarantine flag (`xattr -d com.apple.quarantine`), allowing ClipVault to launch **out-of-the-box seamlessly** without requiring manual security bypass.

---

## 🗑️ Clean Uninstallation

To completely uninstall ClipVault along with all local configuration files and application caches:

```bash
brew uninstall --cask --zap clipvault
```

---

## 📂 Available Casks in this Tap

| Cask | Description | Cask File |
|---|---|---|
| `clipvault` | Primary ClipVault Cask formula | [`Casks/clipvault.rb`](Casks/clipvault.rb) |
| `clip-vault` | Convenience alias formula | [`Casks/clip-vault.rb`](Casks/clip-vault.rb) |

---

## 🔗 Related Repositories

* **Main Application Repository**: [nileshchakraborty/clip-vault](https://github.com/nileshchakraborty/clip-vault)
* **Author**: [Nilesh Chakraborty](https://github.com/nileshchakraborty)
* **License**: MIT License
