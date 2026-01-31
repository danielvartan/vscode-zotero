# Zotero Citation Picker

[Positron](https://positron.posit.co/) (and other VS Code IDE) extension to insert citations from [Zotero](https://www.zotero.org/) to your document and its associated `.bib` file. Requires the [Better BibTeX](https://retorque.re/zotero-better-bibtex/) Zotero plugin.

Fork of <https://github.com/mblode/vscode-zotero> (no longer maintained).

## Features

### Citation Picker

Execute *Zotero Citation Picker* to open a citation picker that lets you find your Zotero citations and insert them into your document and its associated `.bib` file. Activate it using <kbd>Option + Shift + Z</kbd> (macOS) or <kbd>Alt + Shift + Z</kbd> (Windows/Linux).

Alternatively, open the Command Palette with <kbd>Command + Shift + P</kbd> (macOS) or <kbd>Ctrl + Shift + P</kbd> (Windows/Linux) and search for *Zotero Citation Picker*.

### Citation Picker Modes

The extension supports two citation picker modes:

- **Native VS Code Picker (Default)**: Search and select citations within VS Code using a QuickPick interface.
- **Zotero Picker**: Use Zotero's built-in "Cite as you Write" popup window.

Configure the citation picker behavior in VS Code settings:

- `zotero-citation-picker.citeMethod`: Choose between `"vscode"` (native picker) or `"zotero"` (Zotero's CAYW popup)
- `zotero-citation-picker.port`: Customize the Zotero Better BibTeX URL (only used in Zotero picker mode)


#### Native VS Code Citation Picker Features

The native picker offers flexible search options:

- **Simple search**: Just start typing to search across titles, authors, and other fields
- **Advanced search**: Use field-specific prefixes to narrow your search:
  - `author:vuorre`: Find works by a specific author
  - `title:climate`: Search within titles
  - `year:2023`: Filter by publication year
  - `journal:nature`: Search by journal or publication name
  - `tag:statistics`: Find items with specific tags
  - `doi:10.1000`: Search by DOI
  - `author:smith title:climate`: Mix and match multiple fields


### Open Zotero

Open Zotero using <kbd>Command + Option + Shift + Z</kbd> (macOS) or <kbd>Ctrl + Alt + Shift + Z</kbd> (Windows/Linux).

### PDF Opening

Open PDFs from inserted citations by placing your cursor on the citation and pressing <kbd>Control + Command + Option + Shift + Z</kbd> (macOS) or <kbd>Ctrl + Alt + Shift + Win + Z</kbd> (Windows/Linux).

## Development

Test files are in `playground/` (test.md, test.qmd). Press F5 to launch extension in debug mode with test.md open.
