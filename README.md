# Talunivo Flashcards

Brazilian Portuguese (pt-BR) with German translations (de), for an introductory A0/A1 learning path.

The reviewed vocabulary revision 4 contains 50 starter packages and 428 vocabulary cards with 397 distinct expression/translation pairs. Each card has a bilingual example and a German learning note. The reviewed revision updates all examples and explanations. Three separate AI reviewers checked the full content snapshot and confirmed the corrections; this does not claim approval by a human or native-speaking teacher.

## Local import

Use **Pakete → Datei auswählen** and select a `.talunivo` file or `talunivo-start-ptbr-50.zip` for the 50 starter packages. Review the validated preview and confirm the import explicitly. The full local content mirror also includes two unchanged Café supplements with 13 cards; `talunivo-ptbr-52.zip` bundles all 52 packages and 441 cards. Installed content and SQLite progress remain available offline. Packages with more than eight cards have several lesson parts.

All 50 package IDs and all 428 card IDs from revision 3 are retained. The only changed translation is estudar: lernen (Studium) becomes lernen; studieren. Use an app build containing the explicit estudar progress migration when upgrading package 42 from version 3. The current app source preserves its review schedule and counters; an already trained target is retained. Other identical word pairs keep their progress. Replaced sentence cards from version 1 are archived rather than transferring their scores to individual words. The 50 starter packages now use package format 4 with 50 learning objectives and 1,468 explicit exam tasks. Ten packages have package version 5 and forty have version 6. Cards are unchanged from revision 4. Use an app build that supports format 4; older builds cannot import these updates. Existing installed packages remain available offline. Exams test recognition, selection and controlled completion; free speaking and free writing are not assessed.

## Files and validation

- `catalog.json`: metadata and SHA-256 checksums for each listed package.
- `pt-BR/de/start/*.talunivo`: 50 UTF-8 JSON packages with 8–20 cards each.
- `pt-BR/de/start/SHA256SUMS.txt`: per-package checksums.
- `SHA256SUMS.txt`: checksums of the delivery ZIP files.

In the app repository, `scripts/Promote-ReviewedFormat4.py` verifies this promoted snapshot and deterministic ZIP builds; `--apply` rebuilds local deliveries. Earlier authoring scripts describe historical revisions. `tools/Talunivo.PackageValidator` checks the actual app parser, catalog metadata, checksums and generated lessons. JSON Schema is checked separately. The immediately previous starter files (format 2, package version 4) are archived in `docs/pruefungen/format4-produktiv-2026-10-29/productive-before.zip` in the app repository. Earlier revisions remain in their historical archives.

This is an introductory collection, not a certified A1 course. A confirmed device import and final UI verification remain separate checks. Local preparation does not publish packages.
