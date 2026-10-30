# MAPCor: Moroccan Arabic Plurals Corpus

MAPCor is a corpus of **3,708 singular–plural pairs** of Moroccan Arabic (Darija) nouns and adjectives. Each pair is given in IPA and in Arabic script and is annotated with an English gloss, the patterns (templates) of the singular and plural, the plural type, the part of speech, and the grammatical gender of the singular.

The corpus is designed for research on Moroccan Arabic morphology and phonology, on morphological learning and generalization, and for computational linguistics and NLP.

**Current version:** 2.0.0

## Contents

| | Count | % |
|---|---:|---:|
| **Part of speech** | | |
| Nouns | 2,958 | 79.8% |
| Adjectives | 750 | 20.2% |
| **Plural type** | | |
| Sound plural, suffix *-at* | 1,402 | 37.8% |
| Sound plural, suffix *-in* | 600 | 16.2% |
| Sound plural, suffix *-a* | 243 | 6.6% |
| Broken plural | 1,401 | 37.8% |
| Both (broken stem + suffix) | 62 | 1.7% |
| **Total** | **3,708** | **100%** |

## File

`MAPCor.csv` is a comma-separated, UTF-8 encoded file with one singular–plural pair per row and the following columns:

| Column | Description |
|---|---|
| `id` | Row identifier (1–3,708). |
| `singular` | Singular form, in IPA. |
| `plural` | Plural form, in IPA. |
| `singular_arabic` | Singular form, in Arabic script. |
| `plural_arabic` | Plural form, in Arabic script. |
| `gloss` | English gloss of the singular. |
| `singular_pattern` | Pattern (template) of the singular: consonants are written as `C`, vowels are written out (e.g., `CCiC`). |
| `plural_pattern` | Pattern (template) of the plural. |
| `plural_type` | `sound -at`, `sound -in`, or `sound -a` for suffixed (sound) plurals; `broken` for plurals formed by changing the stem; `both` for plurals that change the stem and also add a suffix (e.g., *ħzin* → *ħzanin* ‘sad’). |
| `pos` | Part of speech: `noun` or `adj`. |
| `feminine` | `yes` if the singular is grammatically feminine (usually marked by final *-a*), otherwise `no`. |

The same singular–plural pair can appear more than once when the word has several unrelated meanings (e.g., *səxra* ‘rock’ and ‘commission’).

### Transcription

Forms are given in IPA. Pharyngealized (emphatic) consonants are marked with ˤ (e.g., *tˤ*, *sˤ*, *dˤ*).

### Arabic script

The Arabic-script forms were generated from the IPA forms with a Python script and then corrected by hand. They follow the way Moroccan Arabic is written in everyday use, such as on social media. Moroccan Arabic has no standard spelling, so when a word is commonly written in more than one way, all spellings are given, separated by ` / ` (e.g., تقيل / ثقيل ‘heavy’). Some of these spellings follow the pronunciation and others follow Standard Arabic; feminine *-a* can be written with ة or ا.

## Sources and construction

MAPCor combines two sources:

1. **Version 1 of this corpus** (Nirheche 2025): 1,166 singular–plural noun pairs derived from the Darija Open Dataset (DODa; Outchakoucht & Es-Samaali 2021).
2. **Harrell’s (1966) *A Dictionary of Moroccan Arabic: Moroccan–English***, whose entries were elicited from native speakers in Fez, Rabat, and Casablanca. Singular and plural forms of nouns and adjectives, with their glosses, were extracted manually from the dictionary. Transliteration into IPA and the assignment of patterns and plural types were done with Python scripts and then checked manually.

Because the dictionary dates from the 1960s, every singular and plural was looked up in Atlaset (AtlasIA 2025), arguably the largest collection of contemporary Moroccan Arabic text. Items whose plural was not attested were reviewed manually: forms no longer used in contemporary Moroccan Arabic were removed, and words still in use whose plurals happen not to appear in Atlaset were kept.

## License

MAPCor is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/), the same license as DODa, from which part of the corpus is derived. You may share and adapt the corpus for non-commercial purposes, with appropriate credit.

## How to cite

If you use MAPCor, please cite:

> Nirheche, Ali. 2026. *MAPCor: Moroccan Arabic Plurals Corpus* (Version 2.0.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.23812106

Please also cite the sources it builds on:

- Harrell, Richard S. 1966. *A Dictionary of Moroccan Arabic: Moroccan–English*. Washington, DC: Georgetown University Press.
- Outchakoucht, Aissam & Hamza Es-Samaali. 2021. Moroccan Dialect – Darija – Open Dataset. arXiv:2103.09687. https://github.com/darija-open-dataset/dataset
- AtlasIA. 2025. Atlaset [Data set]. Hugging Face. https://huggingface.co/datasets/atlasia/Atlaset

## Contact

Ali Nirheche, University of Massachusetts Amherst — anirheche@umass.edu — [alinirheche.org](https://alinirheche.org)
