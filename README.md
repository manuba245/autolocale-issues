# AutoLocale VS Code Extension

## 🌐 Overview

**AutoLocale** is a powerful and user-friendly VS Code extension for managing localization in Angular projects using `ngx-translate`. It scans your codebase for translation keys, helps insert and edit them inline, and offers intuitive UIs to manage, validate, and sync translations across multiple language files.

---

## 🚀 Features

- ✨ **Inline Translation Pipe Detection**  
  Highlights `{{ 'key' | translate }}` in HTML and `this.translate.transform('key')` in TypeScript automatically.

- 🖱️ **Cursor-Aware Popup Editor**  
  Instantly view and update translations with a smart popup when your cursor lands inside a translation pipe.

- ➕ **Insert Translation Pipe**  
  Insert a `translate` pipe with a pre-filled key at the current cursor position.

- 📁 **Automatic Translation File Discovery**  
  Scans your workspace for `*.json` files in `/i18n`, `/locales`, `/lang`, etc., and auto-maps language codes.

- 🧾 **Translation Table Editor**  
  Edit all keys and languages in a sortable, filterable table with inline editing, bulk save, import/export, and conflict highlighting.

- ✏️ **Edit & Save Translations**  
  Easily update translations in multiple languages using intuitive popups or the table editor.

- ✅ **Validation & Consistency Checks**  
  Detects:
  - Missing translations across language files
  - Duplicate keys
  - Conflicting values
  - Non-nested vs flat key inconsistencies

- 📤 **Export Translations to CSV**  
  Export selected or all language keys to a UTF-8 BOM-compatible CSV (Excel-friendly).

- 📥 **Import Translations from CSV**  
  Merge translated keys/values from a CSV file back into language JSON files.

- ⚙️ **Custom Regex & File Path Settings**  
  Customize how translation keys are detected per language type, and manage user-defined or ignored file paths.

- 🧩 **Quick Command Menu**  
  Access all features from a status bar menu or the Command Palette.

---

## 🛠️ Usage

### 🌐 Use the Status Bar Menu

Click the **🌐 AutoLocale** button in the VS Code status bar (bottom left) to open a quick-access menu with all translation commands.

### 🔍 Detect & Highlight Translation Pipes

- Open any `.html` or `.ts` file — translation pipes are automatically highlighted.
- Placing the cursor inside a pipe opens a popup translation editor.

### ✍️ Edit Translations

- Modify translation keys or values directly from the popup.
- All detected language files are updated accordingly.

### 🧾 Use the Translation Table Editor

- Run `Edit All Translations (Table View)` from the Command Palette or status bar menu.
- Quickly search, filter, edit, and delete translation keys across all languages.

### ➕ Insert Translation Pipe

- Run `Insert Translation Pipe` from the Command Palette.
- A new key like `new.translation.key` will be inserted at the cursor.

### 🧭 Manage Translation Files

- JSON translation files are auto-detected by language name (`en.json`, `fr.json`, etc.).
- You can also add custom paths or ignore certain files in the Settings panel.

### ✅ Validate Translations

Run `Validate Translations` to check for:

- 🔸 Missing keys
- 🔸 Duplicate entries
- 🔸 Key formatting issues
- 🔸 Inconsistencies across language files

Fix problems interactively using the popup validator.

### 📤 Export / 📥 Import

- Use `Export Translations (CSV)` to save keys/values to a semicolon-delimited CSV.
- Use `Import Translations (CSV)` to sync values from CSV back to JSON files.

---

## 📦 Installation

1. Open Visual Studio Code.
2. Go to Extensions (`Ctrl+Shift+X` / `Cmd+Shift+X`).
3. Search for **AutoLocale** or `Scan Translation Pipes`.
4. Click **Install** and reload VS Code.

---

## 💻 Commands

| Command | Description |
|--------|-------------|
| `Insert Translation Pipe` | Insert a new `translate` pipe at the cursor position. |
| `Validate Translations` | Check translation files for missing/duplicate keys. |
| `Export Translations (CSV)` | Save translations into a CSV file. |
| `Import Translations (CSV)` | Load and merge translations from a CSV file. |
| `Scan Translation Files` | Re-scan the workspace for translation files. |
| `Edit All Translations (Table View)` | Open the full table editor to manage all keys. |
| `Open Translation Settings` | Manage language files, regex patterns, and preferences. |

---

## ⚙️ Configuration & File Naming

Translation files should follow naming conventions such as:

- `en.json`
- `fr.json`
- `es-ES.json`

And reside in standard folders such as:

- `/i18n/`
- `/locales/`
- `/lang/`

You can customize detection and override paths from the Settings panel.

---

## 📋 Requirements

- **VS Code** v1.60 or higher
- Angular project using `@ngx-translate/core`
- JSON-based translation files

---

## ⚠️ Known Issues

- Large translation files may reduce performance during validation or table rendering.
- Dynamic translation keys (e.g., via variables or runtime strings) are not currently supported.

---

## 🤝 Contributing

Found a bug? Have an idea?  
Open an issue or submit a pull request!

📎 [GitHub Repository](https://github.com/manuba245/autolocale-issues)

---
