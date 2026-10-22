# Talunivo Flashcards

Language-learning flashcard packages for Talunivo, organized by language and topic.

The initial collection teaches **Brazilian Portuguese (pt-BR) with German translations (de)**. No prior knowledge required. Further language pairs can be added as the app's import format supports them.

Revision 2 contains 50 numbered packages and 426 vocabulary cards: individual words and short word groups with German translations. Every card has a separate bilingual example. Common words intentionally recur in related topics and share progress when the expression/translation pair is identical. Topics progress from greetings and introductions to shopping, transport, accommodation and everyday needs. This is an introductory collection, not a certified A1 course. Revision 2 requires Talunivo 1.3 or newer.

## Use in Talunivo

In a current app version, open **Pakete → Katalog aus Git laden**, find a topic, and select **Paket zur Vorschau laden**. Review its contents, then confirm **Paket importieren**. Merely downloading or opening the preview does not save cards to your learning progress.

You can also download individual `.talunivo` files from `pt-BR/de/start/` and use **Pakete → Datei auswählen**. If you download the repository as a ZIP, extract it first and select the desired `.talunivo` files individually. Import support for a ZIP depends on the app version and is not required for these files.

Start with package 01 and a few cards per day. Read the Portuguese expression, try to recall its meaning, then reveal the German answer. Use “Noch üben” or “Gewusst” honestly. Imported cards remain available offline; existing SQLite learning progress is preserved. Downloads require internet, but practice does not.

## Files and updates

- `catalog.json`: versioned index with package ID, version, title, card count, relative path and SHA-256 checksum.
- `pt-BR/de/start/*.talunivo`: one editable UTF-8 JSON file per package, containing its eight cards.
- `pt-BR/de/start/SHA256SUMS.txt`: checksums of the individual package files.
- `.gitattributes`: preserves package bytes across Git checkouts, so checksums remain stable.

No app source, credentials, personal information, progress databases, scripts or executable content are included. This repository is publicly readable; the app uses ordinary HTTPS downloads without authentication. Talunivo 1.3 checks only the catalog at startup to notify users about newer installed packages. Package downloads and imports still require explicit user actions. No learning progress or local content is uploaded.

All package IDs remain unchanged; `packageVersion` is now 2. Format version 2 requires `isVocabulary: true` on every card. Expressions contain at most four words; full sentences belong in `example` and `exampleTranslation`. The selection is editorial: sentences have not been automatically tokenized or machine-translated.

Higher package versions may add, change or remove cards. The app shows the changes before confirmation, applies them atomically and preserves review progress for identical expression/translation pairs. New pairs start fresh; replaced cards and their previous progress are retained in local history. A sentence's learning score is never copied onto several new words. The same version with different contents and version downgrades are rejected. Regenerate the catalog and checksums whenever package bytes change.

The app repository includes `scripts/Revise-Flashcards.py` to reproduce this initial editorial revision from the original version-1 commit, and `tools/Talunivo.PackageValidator` to validate all files using the actual import parser, metadata and SHA-256 checksums. See [revision notes](REVISION-2.md).
