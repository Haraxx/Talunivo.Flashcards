# Talunivo Flashcards

Brazilian Portuguese (pt-BR) with German translations (de), for an introductory A0/A1 learning path.

Revision 4 contains 50 starter packages and 428 vocabulary cards with 397 distinct expression/translation pairs. Each card has a bilingual example and a German learning note. The reviewed revision updates all examples and explanations. Three separate AI reviewers checked the full content snapshot and confirmed the corrections; this does not claim approval by a human or native-speaking teacher.

The full local catalog additionally contains two Café add-ons with 13 cards: 52 packages and 441 cards total. The text add-on is version 4; the media add-on is version 3 and retains the reviewed original PNG.

## Local import

Use **Pakete → Datei auswählen** and select a `.talunivo` file or `talunivo-start-ptbr-50.zip` for the 50 starter packages. Use `talunivo-ptbr-52.zip` to import all 52 packages, including the Café add-ons. The starter ZIP intentionally contains 50 packages and its own 50-package catalog. Review the validated preview and confirm the import explicitly. Installed content and SQLite progress remain available offline. Packages with more than eight cards have several lesson parts.

All 50 package IDs and all 428 card IDs from revision 3 are retained. The only changed translation is estudar: lernen (Studium) becomes lernen; studieren. Use an app build containing the explicit estudar progress migration when upgrading package 42 from version 3. The current app source preserves its review schedule and counters; an already trained target is retained. Other identical word pairs keep their progress. Replaced sentence cards from version 1 are archived rather than transferring their scores to individual words. The package format remains version 2; package version 4 is a separate value.

## Files and validation

- `catalog.json`: metadata and SHA-256 checksums for each listed package.
- `pt-BR/de/start/*.talunivo`: 50 UTF-8 JSON packages with 8–20 cards each.
- `pt-BR/de/start/SHA256SUMS.txt`: per-package checksums.
- `SHA256SUMS.txt`: checksums of the delivery ZIP files.

In the app repository, `scripts/Promote-ReviewedLearningContent.py` verifies the promoted snapshot and deterministic ZIP builds; `--apply` rebuilds local deliveries. Earlier authoring scripts describe historical revisions. `tools/Talunivo.PackageValidator` checks the actual app parser, catalog metadata, checksums and generated lessons. JSON Schema is checked separately. The old productive sources remain in `docs/content/archive/learning-content-before-revision-4.zip` in the app repository.

This is an introductory collection, not a certified A1 course. A confirmed device import and final UI verification remain separate checks. Local preparation does not publish packages.
