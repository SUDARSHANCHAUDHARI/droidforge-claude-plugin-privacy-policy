# DroidForge — Privacy Policy

This repository hosts the official privacy policy for the **DroidForge** Claude Code plugin.

**Live privacy policy:** https://sudarshanchaudhari.github.io/droidforge-claude-plugin-privacy-policy/

---

## About DroidForge

**DroidForge** is a Claude Code plugin for solo Android developers. It automates every repetitive task across your Play Store app portfolio — keystore creation, signing configuration, version bumping, Gradle version catalog management, new app scaffolding, and release checklists — all from commands inside Claude Code.

### What It Does

1. Run `/droidforge:setup` once per project — saves your developer conventions locally
2. Scaffold a complete new Android app with correct package names, signing config, and version catalog
3. Generate keystores with consistent conventions — shows the `keytool` command, asks before running
4. Bump `versionCode` and `versionName` with semver (patch / minor / major)
5. Update `libs.versions.toml` with compatibility checks (AGP ↔ Gradle ↔ Kotlin ↔ Compose)
6. Run an interactive pre-submission checklist before every Play Store release

### Commands

| Command | Description |
|---|---|
| `/droidforge:setup` | One-time setup — saves your Android developer conventions |
| `/droidforge:new-app` | Scaffold a complete new Android app with all files |
| `/droidforge:keystore` | Generate a keystore (shows keytool command, asks first) |
| `/droidforge:signing-config` | Write signing config for build.gradle.kts |
| `/droidforge:version-bump` | Bump versionCode and versionName |
| `/droidforge:gradle-update` | Update version catalog dependencies with compatibility checks |
| `/droidforge:release-checklist` | Interactive pre-submission checklist for Play Store |

### Agents

| Agent | Purpose |
|---|---|
| `setup-agent` | Scaffolds complete Android project files |
| `gradle-agent` | Handles Gradle / version catalog issues and updates |
| `release-agent` | Version bump, changelog generation, git tagging |

---

## Install

```bash
/plugin install https://github.com/SUDARSHANCHAUDHARI/DroidForge
```

Run `/droidforge:setup` once per project to save your conventions. All other commands use your saved config automatically — no repeated questions, no hardcoded values.

---

## Plugin Repository

Full source code, documentation, and issue tracker:
**https://github.com/SUDARSHANCHAUDHARI/DroidForge**

---

## Privacy Policy for This Plugin

DroidForge does **not** collect, transmit, or store any user data. All file reading and generation happens locally on your machine. Your developer conventions (name, company, package prefix, keystore password) are stored only in `.claude-plugin-config.json` on your local machine — automatically excluded from git.

The full privacy policy for this plugin is available at:
**https://sudarshanchaudhari.github.io/droidforge-claude-plugin-privacy-policy/**

---

## Author

**SUDARSHANCHAUDHARI** — [github.com/SUDARSHANCHAUDHARI](https://github.com/SUDARSHANCHAUDHARI)
SudarshanTechLabs | sudarshantechlabs@gmail.com

## License

MIT
