# Classical Guitar Teaching Ontology

This repository contains the public releases, documentation, citation metadata,
and selected validation evidence for ClassicalGuitarOntology, an OWL ontology
for the curriculum-derived representation of classical guitar education.

The ontology has evolved from an initial Level 1 model into a validated
six-level curriculum ontology. Earlier public releases are preserved as
historical records, while v1.6.0 is the current recommended frozen release.

## Current recommended release

### ClassicalGuitarOntology v1.6.0

Status: FINAL / FROZEN / VALIDATED

Release directory:

[`ClassicalGuitarOntology_v1.6.0_release/`](ClassicalGuitarOntology_v1.6.0_release/)

ClassicalGuitarOntology v1.6.0 extends the ontology from the Level 1 scope of
the previous public release to all six curriculum levels (Levels 1–6).

The public v1.6.0 release includes:

- the authoritative frozen OWL 2 DL ontology baseline;
- a separately validated SWRL supplement;
- compact formal-validation evidence;
- a compact summary of the validated SWRL behavior;
- one representative R02-to-R01 inference trace;
- version-specific documentation, citation metadata, and licensing information.

Detailed validation, competency-question, provenance, traceability, and
integrity records were retained as part of the study documentation.

### Authoritative v1.6.0 baseline

`ClassicalGuitarOntology_v1.6.0.owl`

SHA-256:

`da8267d5a9be3bd68fe6114157effaeec8cbe377c6ed7cc147274dcc8ceaee36`

The v1.6.0 OWL ontology was frozen after formal validation and was not modified
during the subsequent SWRL and competency-question phases.

## Public release history

### v1.0.0

[`ClassicalGuitarOntology_v1.0.0_release/`](ClassicalGuitarOntology_v1.0.0_release/)

Initial public ontology release.

### v1.0.5

[`ClassicalGuitarOntology_v1.0.5_release/`](ClassicalGuitarOntology_v1.0.5_release/)

Public release focused on Level 1 classical guitar education.

Intermediate versions `v1.0.1` through `v1.0.4` were local working versions
used during ontology refinement and were not published as separate GitHub
releases.

### v1.6.0

[`ClassicalGuitarOntology_v1.6.0_release/`](ClassicalGuitarOntology_v1.6.0_release/)

Major curriculum-scope and validation release.

Key differences from v1.0.5 include:

- expansion from Level 1 to Levels 1–6;
- establishment of a frozen OWL 2 DL baseline;
- formal validation with HermiT and ROBOT;
- addition of a separate SWRL reasoning supplement;
- validation of `R01_SameLevelSkillAlignment` and
  `R02_ObjectiveSkillFromTeachingPractice`;
- asserted and inference-dependent competency-question evaluation;
- provenance-aware separation of asserted, OWL-inferred, SWRL-derived, and
  SPARQL-retrieved knowledge;
- cross-phase traceability and reproducibility-oriented study documentation.

For detailed version changes, see:

[`ClassicalGuitarOntology_v1.6.0_release/CHANGELOG.md`](ClassicalGuitarOntology_v1.6.0_release/CHANGELOG.md)

## Repository structure

```text
classical-guitar-teaching-ontology/
├── ClassicalGuitarOntology_v1.0.0_release/
├── ClassicalGuitarOntology_v1.0.5_release/
├── ClassicalGuitarOntology_v1.6.0_release/
├── ontology/
├── CITATION.cff
├── LICENSE
└── README.md
```

Each public release directory is intended to remain a version-specific record
with its own ontology artefact and associated metadata.

The v1.6.0 release directory additionally contains selected validation and
reasoning evidence corresponding to the ontology-engineering study.

## v1.6.0 reasoning and validation model

The v1.6.0 workflow maintains a strict distinction between:

1. ASSERTED OWL knowledge
2. OWL-INFERRED knowledge
3. SWRL-DERIVED knowledge
4. SPARQL query results
5. VALIDATION / METADATA evidence

SPARQL is used as a retrieval mechanism and is not treated as an inference
mechanism.

Under the Open World Assumption, absence of an assertion or inference is not
interpreted automatically as logical negation.

### SWRL execution

The accepted v1.6.0 SWRL rules were executed through SWRLAPI/Drools.

HermiT was not used to execute the SWRL rules. HermiT was used separately for
OWL description-logic classification and validation.

Accepted rules:

- `R01_SameLevelSkillAlignment`
- `R02_ObjectiveSkillFromTeachingPractice`

## Integrity

The authoritative v1.6.0 OWL baseline and the SWRL supplement are identified
by SHA-256 checksums in the version-specific release documentation.

Checksums support verification of byte-level artefact identity and integrity;
they do not by themselves establish semantic correctness or independent
reproduction.

## License

ClassicalGuitarOntology is released under the Creative Commons Attribution 4.0
International License (CC BY 4.0).

See:

[`LICENSE`](LICENSE)

## Citation

Please cite the ontology using the metadata provided in:

[`CITATION.cff`](CITATION.cff)

The root citation metadata identifies the current recommended release.

Version-specific citation metadata is retained inside the corresponding release
directories. For v1.6.0, see:

[`ClassicalGuitarOntology_v1.6.0_release/CITATION.cff`](ClassicalGuitarOntology_v1.6.0_release/CITATION.cff)

## Versioning policy

Public release directories are treated as historical version records.

Earlier releases are not retroactively modified to represent the ontology
scope, validation evidence, or reasoning capabilities of later releases.

For reproducibility-sensitive work, users should cite and retrieve the exact
version associated with the relevant study.
