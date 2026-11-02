# homebrew-clipvault

Official Homebrew tap for [ClipVault](https://github.com/nileshchakraborty/clip-vault) — A lightweight, privacy-first, RAM-only macOS clipboard history manager.

---

## 🚀 Installation

### One-line Install (Recommended)

To install ClipVault via Homebrew Cask, simply run:

```bash
brew install --cask nileshchakraborty/clipvault/clipvault
```

Or tap the repository first and install:

```bash
brew tap nileshchakraborty/clipvault
brew install --cask clipvault
```

*(Note: Both `clipvault` and `clip-vault` formula names are supported)*

---

### In a Brewfile

If you manage your software with [Homebrew Bundle](https://github.com/Homebrew/homebrew-bundle), add the following to your `Brewfile`:

```ruby
tap "nileshchakraborty/clipvault"
cask "clipvault"
```

---

## 🔄 Upgrading

To upgrade ClipVault to the latest release:

```bash
brew upgrade --cask clipvault
```

---

## 🛡️ macOS Gatekeeper & Out-of-the-Box Execution

> [!NOTE]
> ClipVault is open-source software built transparently. Because it is distributed directly from open-source GitHub releases without an Apple Developer subscription notarization ticket, macOS Sequoia and Sonoma would normally trigger Gatekeeper quarantine dialogs (*"Apple cannot check ClipVault for malicious software"*).
>
> This tap's Cask definition includes automated postflight quarantine removal (`xattr -d com.apple.quarantine`) so ClipVault launches **out-of-the-box seamlessly** without requiring manual security bypass!

---

## 🗑️ Uninstallation

To cleanly remove ClipVault along with all local configuration files:

```bash
brew uninstall --cask --zap clipvault
```

---

## 🔗 Project Links

* **ClipVault Main Repository**: [https://github.com/nileshchakraborty/clip-vault](https://github.com/nileshchakraborty/clip-vault)
* **Author**: [Nilesh Chakraborty](https://github.com/nileshchakraborty)
* **License**: MIT
