# Talunivo Flashcards

Brazilian Portuguese (pt-BR) with German translations (de), for an introductory A0/A1 learning path.

Revision 3 contains 50 starter packages with 428 vocabulary cards, plus two Café add-ons with 13 cards: 52 catalog packages and 441 cards in total. Each card has a bilingual example and a German learning note. Cards contain individual words or short expressions; full sentences belong in the examples. The numbers zero to ten, numbers eleven to nineteen, tens to one hundred, all seven weekdays and all four seasons are covered. Common vocabulary intentionally recurs across related topics and shares progress for identical expression/translation pairs.

## Local import

Use **Pakete → Datei auswählen** and select an individual `.talunivo` file, or `talunivo-start-ptbr-50.zip` for the complete collection. Review the validated preview and confirm the import explicitly. Installed content and SQLite learning progress remain available offline. Packages with more than eight cards have several lesson parts, linked from each lesson.

All 50 package IDs and all 426 vocabulary card IDs and word pairs from revision 2 are retained. Revision 3 corrects 75 bilingual examples, adds learning notes and adds the missing spring and autumn vocabulary. Format version 2 declares `isVocabulary: true`. Package version 3 is separate from the format version. Use Talunivo 1.3 or newer.

Updates preserve repetition progress for identical word pairs. The app archives replaced sentence cards from version 1 rather than transferring their scores to individual new words. Downloading or previewing a package does not import it. The app catalog on the main branch supplies these revisions. Reload the catalog and explicitly confirm each update after reviewing its preview.

## Files and validation

- `catalog.json`: package metadata and SHA-256 checksums.
- `pt-BR/de/start/*.talunivo`: UTF-8 JSON starter vocabulary packages, with 8–20 cards depending on the topic.
- `pt-BR/de/cafe/*.talunivo`: the Café text add-on (package version 3) and illustrated pilot (package version 2, format 3).
- `talunivo-start-ptbr-50.zip`: all 50 starter packages for a single confirmed import.
- `pt-BR/de/start/SHA256SUMS.txt`: per-file checksums.
- `pt-BR/de/start/README.md`: German topic guide.

In the app repository, `scripts/Review-LearningPackages.py` rebuilds this revision from the preserved source archive. `tools/Talunivo.PackageValidator` checks the actual app parser, catalog metadata, hashes and generated lessons. A separate JSON-Schema check also validates the package structure. Editorial review by Codex is complete; independent review by a native-speaking teacher and a device import remain separate steps. This is an introductory collection, not a certified A1 course.

See [revision 3 notes](REVISION-3.md) for the corrections and update behavior.
