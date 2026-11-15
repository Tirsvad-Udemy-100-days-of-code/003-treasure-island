# Artifact Registry

This project's artifact state. Types, short names and `CrossReference
Candidates` come from the framework catalog
(`framework/registry/artifact-catalog.md`); this file only records where
each document lives in *this* project and the next version to use.

| Short Name | Artifact Type | Primary File | Next Available Version |
| --- | --- | --- | --- |

## Languages

| Setting | Value |
| --- | --- |
| PO language | en |
| PO domain | it |
| High-level register | IT Executive English |
| Technical register | IT Professional English |
| Wiki languages | en (the PO language is English, so no further language is required) |

Every artifact of a type marked "Yes" below states its language and domain in
its `Language` and `Domain` Metadata rows. `Domain` is a value from this list.

| Domain | Meaning |
| --- | --- |
| it | Software and IT |

| Artifact types | Register | Written in the PO language |
| --- | --- | --- |
| BC, KPI, PP, MIL | IT Executive English | Yes |
| SA, BMC, BPMN, UCD, US, UC, SSD, DM, RA, GOV, DICT | IT Professional English | Yes |
| OC, SD, DCD, ERD, TP, AD, ADR, TM, RC, QC, source code | IT Professional English | No |

## Notes

- "Next Available Version" is the zero-padded (3-digit) version to use the
  *next* time a new document of that type is created.
- `ADR` uses 4 digits (`0001`); `RC` is sequential across all artifact types.
