# ClassicalGuitarOntology v1.6.0 — Frozen Reproducibility Release

## Purpose

This directory contains the compact reviewer-facing evidence associated with ClassicalGuitarOntology v1.6.0.

The release documents the validated OWL 2 DL baseline, the final SWRL supplement, formal validation evidence, and a representative inference trace.

Competency-question results are summarized in the associated manuscript. Detailed validation, competency-question, provenance, traceability, and integrity records were retained as part of the study documentation.

## Frozen baseline

Ontology file:

`ClassicalGuitarOntology_v1.6.0.owl`

SHA-256:

`da8267d5a9be3bd68fe6114157effaeec8cbe377c6ed7cc147274dcc8ceaee36`

The v1.6.0 OWL ontology is the authoritative frozen baseline. It was not modified during the subsequent SWRL and competency-question phases.

## SWRL supplement

File:

`ClassicalGuitarOntology_v1.6.0_SWRL_Supplement_v1.0.0.owl`

SHA-256:

`b9aff4640b0169414717ca06de04bb4887f3f806d04b6fbdc7153296dead29ae`

Accepted rules:

- `R01_SameLevelSkillAlignment`
- `R02_ObjectiveSkillFromTeachingPractice`

SWRL execution was performed through SWRLAPI/Drools. HermiT was used separately for OWL description-logic classification and validation; it was not used to execute the SWRL rules.

## Included reviewer-facing evidence

### `ClassicalGuitarOntology_v1.6.0_HermiT_Evidence_Log_2026-08-17.txt`

Compact Phase 1 formal-validation evidence, including the validated ontology identity, HermiT classification evidence, and ROBOT OWL 2 DL profile result.

### `SWRL_Validation_Summary.txt`

Compact summary of the validated R01 and R02 rule behavior, including isolated results and the controlled R02-to-R01 chaining effect.

### `Representative_R02_R01_Inference_Trace.txt`

One complete representative inference chain distinguishing asserted OWL, OWL-inferred typing, SWRL-derived assertions, and SPARQL retrieval.

## Competency questions

The associated manuscript reports the compact results for:

- CQ3A-01 through CQ3A-08: asserted competency questions
- CQ3B-01 through CQ3B-04: inference-dependent competency questions

Detailed SPARQL queries, outputs, CQ-specific provenance records, differential controls, and cross-phase traceability records were retained as part of the study documentation and are not duplicated in this compact release directory.

## Knowledge-layer distinction

The release maintains an explicit distinction between:

1. ASSERTED OWL knowledge
2. OWL-INFERRED knowledge
3. SWRL-DERIVED knowledge
4. SPARQL query results
5. VALIDATION / METADATA evidence

Absence of an assertion or inference is not interpreted as logical negation under the Open World Assumption.

## Integrity

The SHA-256 values above are provided to support verification of byte-level artefact identity and integrity.

Checksums do not, by themselves, establish semantic correctness or independent reproduction.

## Citation and license

Version-specific citation metadata and licensing information are included in this release directory through:

- `CITATION.cff`
- `LICENSE`

The repository root also contains the current repository-level citation and license metadata.

## Release status

ClassicalGuitarOntology v1.6.0

`FINAL / FROZEN / VALIDATED`

The frozen OWL baseline remains the authoritative ontology artefact for this release.
