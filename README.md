# LexiMus-UR: Melcior 1859 — Chord Ontology Model

**LexiMus-UR** is the subproject of the Universidad de La Rioja within **LexiMus** (*Léxico en español y ontología de la música*), a coordinated research project whose aim is to model historical Spanish music dictionaries as formal ontologies. The corpus spans five dictionaries published between 1852 and 1929: Fargas (1852), Melcior (1859), Parada (1868), Pedrell (1894), and Lacal (1899).

This repository makes available the ontology models, extraction data, and processing scripts produced by the LexiMus-UR team. Resources are released incrementally as the project progresses.

---

## Repository contents

Resources are organised by source and type. Each release may include ontology models (`.ttl`), extraction datasets (`.csv`), and processing scripts (`.py`).

### Melcior 1859 — chord model (v1.0)

| File | Description |
|------|-------------|
| `melcior_1859_modelo_acorde_v3.ttl` | Chord entry + semantic neighbourhood (1,328 triples, 71 classes, 37 properties). Cited in associated publication. |

Additional models for related entries (interval, sound, consonance/dissonance) will be released in subsequent versions.

---

## Model overview

The chord model (`v3`) covers:
- **1,328 triples**
- **71 classes** (CIDOC-CRM anchored: E73, E29, E89, E21, plus domain-specific extensions)
- **37 properties**: 24 object properties, 12 datatype properties, 1 annotation property
- **Namespace**: `http://leximus.es/ontology#` (`leximus:`)

Upper-level ontology: **CIDOC-CRM** (ISO 21127:2023).
Domain-specific properties cover normative, evaluative, perceptual, and epistemic content absent from current music ontologies.

---

## Method

Definitions were decomposed into subject–predicate–object triples through propositional analysis. Extraction followed a reactive validation protocol: LLM-assisted first-pass identification of candidate propositions, followed by expert review and semantic classification by the PI. All modeling decisions are documented in the associated publication (see Citation).

---

## Corpus

**Melcior, C. J.** (1859). *Diccionario enciclopédico de la música*. Lérida: Imprenta de Agustín Carruez.
Corpus: LexiMus-UR (Universidad de La Rioja). Full corpus: Fargas 1852, Melcior 1859, Parada 1868, Pedrell 1894, Lacal 1899.

---

## Citation

If you use this dataset, please cite:

> LexiMus (2026). *LexiMus-UR: Melcior 1859 chord ontology model* (v1.0) [Dataset]. Zenodo. https://doi.org/10.5281/zenodo.[to be assigned]

And the associated article:

> 

---

## License

[Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE)

---

## Acknowledgements

Propositional extraction was carried out using a reactive validation protocol: candidate subject–predicate–object structures were identified through LLM-assisted first-pass extraction (Claude Sonnet, Anthropic), followed by expert review, semantic classification, and modeling decisions by the PI. All intellectual and analytical decisions are the responsibility of the research team.

This work is part of the project "Léxico en español y ontología de la música (LexiMus)" (PID2022-139589NB-C32), funded by MCIN/AEI/10.13039/501100011033/FEDER, UE.

---

## Contact

Teresa Cascudo García-Villaraco · Universidad de La Rioja / SCRIUR
[teresa.cascudo@unirioja.es](mailto:teresa.cascudo@unirioja.es)

Arturo de las Casas Escolar · Universidad de La Rioja / SCRIUR
