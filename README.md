# Katib — Arabic Script Dataset Editor
![Katib logo](katib.png)

**Katib** is a lightweight, browser-based editor for working with bilingual or Arabic-script datasets stored in **JSON** or **JSONL** files.

It is designed for workflows where you need to review, edit, validate, and export records that contain **Latin/LTR text** alongside **Arabic/RTL text** — directly in the browser.

Katib is especially useful for building and cleaning datasets for **machine translation**, **transliteration**, **Arabic NLP**, and **localization** workflows.

It can help you start creating parallel datasets for language pairs such as:

- **English ↔ Hassaniya**
- **French ↔ Hassaniya**
- **English ↔ Arabic**
- **English ↔ Darija**

More language pairs can be supported as your datasets grow.

## Why Katib?

Editing Arabic text inside structured dataset files can be slow and error-prone in general-purpose editors.

Katib makes that easier by giving you:

- a **record-by-record editing view**
- proper **RTL support** for Arabic text
- an **on-screen Arabic keyboard**
- support for both **JSON arrays** and **JSONL**
- **field mapping** for different dataset schemas
- **search**, **review tracking**, and **export**

## Features

- Open **`.json`**, **`.jsonl`**, or pasted content
- Detect and map dataset fields for:
  - **Latin / LTR text**
  - **Arabic / RTL text**
- Edit records one by one in a focused interface
- Switch to a **raw editor** for direct JSONL editing
- Validate dataset structure before export
- Export as:
  - **JSONL**
  - **JSON**
- Search across records
- Mark records as **reviewed**
- Track review progress
- Add, duplicate, undo, or delete records
- Drag and drop files directly into the app
- Use the built-in **Arabic keyboard** with:
  - standard letters
  - extended letters
  - diacritics
  - digits and punctuation

## Supported formats

### JSONL
One JSON object per line:

```json
{"latin":"selam","arabic":"سلام"}
{"latin":"kitab","arabic":"كتاب"}
```

### JSON
An array of JSON objects:

```json
[
  { "latin": "selam", "arabic": "سلام" },
  { "latin": "kitab", "arabic": "كتاب" }
]
```

## How it works

1. Open a JSON or JSONL file
2. Katib detects the available fields
3. If there are more than two fields, you choose:
   - which field is the **LTR / Latin** field
   - which field is the **RTL / Arabic** field
4. Review and edit records
5. Validate your data
6. Download the edited result as JSONL or JSON

## Use cases

Katib is useful for:

- creating datasets for **machine translation**
- Arabic dataset review
- transliteration correction
- parallel text editing
- localization QA
- annotation cleanup
- script conversion review
- preparing Arabic NLP training data
- checking bilingual records before export

## Interface overview

### Record view
A focused record-by-record editor with:

- LTR field editor
- RTL field editor
- previous / next navigation
- jump-to-record
- search
- review status
- add / duplicate / delete actions

### Raw editor
A plain text editing mode for working directly with JSONL content.

### Arabic keyboard
A built-in on-screen keyboard for entering Arabic characters and marks more easily.

## Privacy

Katib runs entirely in the browser.

All data stays on your device while you use the app. There is **no server-side processing**, **no backend**, and **no file upload** built into Katib itself.

## License

This project is licensed under the **MIT License**. See the `LICENSE` file for details.

## Contributing

Issues, suggestions, and improvements are welcome.

If you use Katib in machine translation, Arabic NLP, localization, annotation, or dataset preparation workflows, feedback is especially helpful.
