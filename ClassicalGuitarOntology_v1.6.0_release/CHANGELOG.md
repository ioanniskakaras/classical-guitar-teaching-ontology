# CHANGELOG — ClassicalGuitarOntology v1.6.0

## Release

Version: v1.6.0  
Release date: 2026-09-08  
Status: FINAL / FROZEN / VALIDATED

## Summary

ClassicalGuitarOntology v1.6.0 is a major scope and validation expansion of the ontology.

Whereas the previous public release, v1.0.5, represented only Level 1 of the classical guitar curriculum, v1.6.0 extends the ontology to all six curriculum levels (Levels 1–6) and introduces a substantially more rigorous validation, reasoning, competency-question, provenance, and reproducibility-oriented workflow.

The OWL ontology file `ClassicalGuitarOntology_v1.6.0.owl` is the authoritative frozen baseline for this release.

---

## Major changes since v1.0.5

### 1. Curriculum scope expanded from Level 1 to Levels 1–6

- Extended the ontology from a Level 1-only representation to a six-level curriculum model.
- Added curriculum entities required to represent Levels 2, 3, 4, 5, and 6.
- Preserved the ontology-based representation of learning objectives, teaching practices, skills, techniques, exercises, repertoire, evaluation criteria, historical content, and related curriculum structures across the expanded scope.
- The resulting v1.6.0 baseline contains the complete six-level ontology used in the present study.

### 2. Frozen OWL 2 DL baseline established

The final ontology baseline is:

`ClassicalGuitarOntology_v1.6.0.owl`

SHA-256:

`da8267d5a9be3bd68fe6114157effaeec8cbe377c6ed7cc147274dcc8ceaee36`

The baseline was frozen after Phase 1 validation and was not modified during the subsequent SWRL and competency-question phases.

### 3. Formal ontology validation strengthened

The v1.6.0 release includes a formal validation workflow covering:

- OWL 2 DL profile validation
- HermiT classification
- consistency-oriented inspection
- inspection for named unsatisfiable classes
- ROBOT-based OWL 2 DL profile checking

The compact release includes:

`ClassicalGuitarOntology_v1.6.0_HermiT_Evidence_Log_2026-08-17.txt`

### 4. Separate SWRL reasoning supplement introduced

SWRL reasoning was developed in a separate ontology artefact:

`ClassicalGuitarOntology_v1.6.0_SWRL_Supplement_v1.0.0.owl`

SHA-256:

`b9aff4640b0169414717ca06de04bb4887f3f806d04b6fbdc7153296dead29ae`

Two rules were accepted after isolated and integration validation:

- `R01_SameLevelSkillAlignment`
- `R02_ObjectiveSkillFromTeachingPractice`

SWRL execution was performed through SWRLAPI/Drools.

HermiT was used separately for OWL description-logic classification and validation and was not used to execute the SWRL rules.

### 5. SWRL rule validation and chaining evidence added

The accepted rules were tested individually and jointly.

Validated results include:

- R01: 468 novel `alignsWith` assertions
- R02: 11 novel `achievesSkill` assertions
- R02 -> R01 chaining: 5 additional expected `alignsWith` assertions
- no unexpected or missing novel rule-head assertions in the validated tests

Compact reviewer-facing evidence is provided in:

- `SWRL_Validation_Summary.txt`
- `Representative_R02_R01_Inference_Trace.txt`

### 6. Competency-question validation added

Two competency-question branches were introduced.

Phase 3A comprised eight asserted-knowledge competency questions:

- CQ3A-01 through CQ3A-08

Phase 3B comprised four validated inference-dependent competency questions:

- CQ3B-01 through CQ3B-04

A fifth candidate competency question, CQ3B-05, was formally assessed as NOT REQUIRED.

The compact CQ results are reported in the associated manuscript. Detailed SPARQL queries, outputs, CQ-specific provenance records, differential controls, and validation evidence were retained as part of the study documentation and are not duplicated in the compact release folder.

### 7. Provenance and knowledge-layer separation strengthened

The v1.6.0 workflow explicitly distinguishes:

1. ASSERTED OWL knowledge
2. OWL-INFERRED knowledge
3. SWRL-DERIVED knowledge
4. SPARQL query results
5. VALIDATION / METADATA evidence

This separation supports controlled interpretation of reasoning results and avoids conflating retrieval with inference.

### 8. Cross-phase traceability introduced

The complete validation workflow was connected through a cross-phase traceability framework covering:

- baseline validation
- SWRL rule validation
- integration validation
- asserted competency questions
- inference-dependent competency questions
- provenance evidence
- reproducibility closure

The full traceability record contains `TR-001` through `TR-022` and was retained as part of the study documentation rather than duplicated in the compact release folder.

### 9. Reproducibility-oriented documentation strengthened

The v1.6.0 workflow retains detailed validation, reasoning, competency-question, provenance, traceability, and integrity records supporting the study.

These detailed records are not duplicated in the compact public release folder.

---

## Files in the compact v1.6.0 release folder

- `ClassicalGuitarOntology_v1.6.0.owl`
- `ClassicalGuitarOntology_v1.6.0_SWRL_Supplement_v1.0.0.owl`
- `ClassicalGuitarOntology_v1.6.0_HermiT_Evidence_Log_2026-08-17.txt`
- `SWRL_Validation_Summary.txt`
- `Representative_R02_R01_Inference_Trace.txt`
- `README.md`
- `CITATION.cff`
- `LICENSE`
- `CHANGELOG.md`

---

## Version relationship

### v1.0.5

- Public ontology release focused on Level 1 of the classical guitar curriculum.

### v1.6.0

- Extends the ontology to Levels 1–6.
- Adds formal OWL 2 DL validation evidence.
- Adds a separately validated SWRL reasoning supplement.
- Adds asserted and inference-dependent competency questions.
- Adds provenance-aware reasoning validation.
- Adds cross-phase traceability.
- Strengthens reproducibility-oriented study documentation.

---

## Release note

v1.6.0 should be treated as a new frozen research release associated with the six-level ontology and its validated reasoning and reproducibility-oriented workflow.

Earlier releases remain historical records and should not be retroactively modified to represent the scope or evidence of v1.6.0.
