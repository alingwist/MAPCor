# Changelog

## 2.0.0 (2026-10-30)

- Renamed the corpus **MAPCor: Moroccan Arabic Plurals Corpus**.
- Expanded from 1,166 to 3,708 singular–plural pairs by adding nouns and adjectives from Harrell's (1966) *Dictionary of Moroccan Arabic*, filtered for contemporary use against the Atlaset corpus.
- Added adjectives and new columns: `singular_arabic` and `plural_arabic` (Arabic-script spellings), `pos` (noun or adjective), `feminine` (grammatical gender of the singular), and `id`.
- Split sound plurals by suffix (`sound -at`, `sound -in`, `sound -a`).
- Renamed columns to a consistent style (`singular_pattern`, `plural_pattern`).
- Removed duplicate rows, filled in missing glosses, and corrected typos in glosses and a few IPA transcriptions.
- DOI: 10.5281/zenodo.23812106

## 1.0.0 (2025-01-14)

- First release as "Moroccan Arabic Plurals Corpus": 1,166 singular–plural noun pairs derived from the Darija Open Dataset (DODa), with IPA transcriptions, glosses, patterns, and plural type. DOI: 10.5281/zenodo.14642330
