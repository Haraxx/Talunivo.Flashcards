# Revision 3: reviewed examples and complete topic coverage

The starter collection retains all 50 package IDs and all 426 existing vocabulary card IDs and word pairs. Each starter package is raised from version 2 to 3, retaining schema version 2. The collection now has 428 cards, including the missing spring and autumn vocabulary.

- Corrected or clarified 75 bilingual example pairs. Examples now illustrate their actual learning word, including zero, numbers eleven to thirteen, hunger, telephone number and several verbs.
- Each starter card has a bilingual example and a German learning note covering usage, gender, plurals, inflection or Brazilian Portuguese where relevant.
- Every number from zero to ten has its own application example. Numbers eleven to nineteen, tens through one hundred, all seven weekdays and all four seasons are covered.
- Replaced shared counting lists with individual examples. Common words intentionally recur across related topics and retain a shared review identity.
- Added the reviewed Café text add-on (3 cards, package version 3) and Café image pilot (10 cards, package version 2) under pt-BR/de/cafe. The illustration is embedded in format 3; no external image request is needed.

The catalog contains 52 packages and 441 cards. The starter ZIP contains only the 50 starter packages. The catalog records each file's version, card count and SHA-256 checksum. Packages, checksums and generated exercises were validated with the actual app parser; package JSON was checked independently against the app schema. The preceding review passed 152 core tests, 274 UI tests and an Android Debug build. Independent native-speaker approval is still outstanding.

## Update in Talunivo

Open **Pakete → Katalog aus Git laden**, reload the catalog, select the updated package and inspect the preview. Confirm the import to apply the update. Identical word pairs preserve repetition progress. When upgrading the original sentence-based version 1, old sentence cards remain archived rather than copying their scores to several new vocabulary words.

Larger packages contain several lesson sections, with at most eight cards per section. All sections remain available on the learning path. The accompanying app change also adds links between sections directly inside the lesson; receiving that navigation improvement requires installing the updated app build. The content updates themselves are provided by this repository.

Imports remain explicit and learning remains offline after import. No app database or learning history is uploaded.
