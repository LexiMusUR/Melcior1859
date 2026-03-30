# LexiMus-UR: Melcior 1859 — Chord Ontology Model

**LexiMus-UR** is the subproject of the Universidad de La Rioja within **LexiMus** (*Léxico en español y ontología de la música*), a coordinated research project whose aim is to model historical Spanish music dictionaries as formal ontologies. The corpus spans five dictionaries published between 1852 and 1929: Fargas (1852), Melcior (1859), Parada (1868), Pedrell (1894), and Lacal (1899).

This repository makes available the ontology models, extraction data, and processing scripts produced by the LexiMus-UR team. Resources are released incrementally as the project progresses.

---

## Repository contents

Resources are organised by source and type. Each release may include ontology models (`.ttl`), extraction datasets (`.csv`), and processing scripts (`.py`).

### Melcior 1859 — chord model (v1.0)

| File | Description |
|------|-------------|
| `melcior_1859_modelo_acorde_v3.ttl` | Main Turtle model: chord entry + semantic neighbourhood (1,328 triples, 71 classes, 37 properties) |
| `melcior_1859_modelo_efecto_consonancia_disonancia_v1.ttl` | Model for consonance/dissonance effect entries |
| `melcior_1859_modelo_intervalo_v1.ttl` | Model for the interval entry |
| `melcior_1859_modelo_sonido_v1.ttl` | Model for the sound entry |

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

> Cascudo García-Villaraco, T. (2026). *LexiMus-UR: Melcior 1859 chord ontology model* (v1.0) [Dataset]. Zenodo. https://doi.org/10.5281/zenodo.[to be assigned]

And the associated article:

> Cascudo García-Villaraco, T. (2026). What counts as ontological? Historical music definitions and the epistemological limits of current knowledge representation. *Journal of New Music Research*.

---

## License

[Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE)

---

## Contact

Teresa Cascudo García-Villaraco
Universidad de La Rioja
[teresa.cascudo@unirioja.es](mailto:teresa.cascudo@unirioja.es)
