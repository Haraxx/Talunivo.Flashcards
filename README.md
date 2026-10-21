# Talunivo Flashcards

Language-learning flashcard packages for Talunivo, organized by language and topic.

The initial collection teaches **Brazilian Portuguese (pt-BR) with German translations (de)**. No prior knowledge required. Further language pairs can be added as the app's import format supports them.

This content-only repository contains 50 numbered packages with 8 cards each: 400 distinct expression/translation pairs, German learning hints, and 50 extra bilingual examples. Six expressions intentionally reinforce items in Talunivo's base course. Topics progress from greetings and introductions to shopping, transport, accommodation, everyday needs, and short conversation missions. This is an introductory collection, not a certified A1 course.

## Use in Talunivo

In a current app version, open **Pakete → Katalog aus Git laden**, find a topic, and select **Paket zur Vorschau laden**. Review its contents, then confirm **Paket importieren**. Merely downloading or opening the preview does not save cards to your learning progress.

You can also download individual `.talunivo` files from `pt-BR/de/start/` and use **Pakete → Datei auswählen**. For all packages, download this repository as a ZIP using GitHub's **Code → Download ZIP** and select that ZIP in Talunivo. Confirm **Alle Pakete importieren** only after checking the preview.

Start with package 01 and a few cards per day. Read the Portuguese expression, try to recall its meaning, then reveal the German answer. Use “Noch üben” or “Gewusst” honestly. Imported cards remain available offline; existing SQLite learning progress is preserved. Downloads require internet, but practice does not.

## Files and updates

- `catalog.json`: versioned index with package ID, version, title, card count, relative path and SHA-256 checksum.
- `pt-BR/de/start/*.talunivo`: one editable UTF-8 JSON file per package, containing its eight cards.
- `pt-BR/de/start/SHA256SUMS.txt`: checksums of the individual package files.
- `.gitattributes`: preserves package bytes across Git checkouts, so checksums remain stable.

No app source, credentials, personal information, progress databases, scripts or executable content are included. This repository is publicly readable; the app uses ordinary HTTPS downloads without authentication. No automatic downloads, imports or updates occur.

Existing cards must remain unchanged when publishing an additive package version. Increment `packageVersion` only when adding cards; corrections to existing cards currently require a new package ID. Regenerate the catalog and checksums whenever package bytes change. The Talunivo app repository includes `scripts/Update-PackageCatalog.ps1` and `scripts/Export-FlashcardRepository.ps1` to prepare and verify this content-only repository.
