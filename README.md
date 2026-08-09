waam-logger/
│
├── metadata/          # Material, process, and registry-level metadata
├── processed/         # Cleaned geometric descriptors (CSV/Parquet)
├── raw/               # Raw profilometric scans (external links if large)
├── schema/            # Machine-readable data dictionary and field definitions
├── code/              # Feature extraction, QC routines, and benchmark models
└── docs/              # Workflow documentation, FAIR notes, usage examples
Here is a **polished, publication‑quality `README.md`** for a WAAM dataset repository.  
It is structured, professional, and ready to drop directly into GitHub.

---

# WAAM Logger Dataset
A traceable, FAIR‑aligned experimental dataset for single‑bead Wire Arc Additive Manufacturing (WAAM).  
This repository provides structured process records, profilometric metrology, geometric descriptors, and benchmark models designed to support reproducible research, machine‑learning development, and digital‑thread workflows in arc‑based additive manufacturing.

---

## Repository Structure

```
waam-logger/
│
├── metadata/          # Material, process, and registry-level metadata
├── processed/         # Cleaned geometric descriptors (CSV/Parquet)
├── raw/               # Raw profilometric scans (external links if large)
├── schema/            # Machine-readable data dictionary and field definitions
├── code/              # Feature extraction, QC routines, and benchmark models
└── docs/              # Workflow documentation, FAIR notes, usage examples
```

---

##  Dataset Overview

The dataset contains **traceable single-bead WAAM depositions** across multiple materials and process conditions.  
Each deposition run is assigned a **unique `exp_id`** and includes:

- Commanded process parameters (Voltage, WFS, TS, CTWD)
- Material identity (e.g., ER70S‑6, 316LSi)
- Profilometric surface scans (Keyence VR‑600)
- Extracted height and width descriptors
- Aspect ratio and uniformity metrics
- Quality-control flags and provenance records

The dataset supports **registry-level consistency checks**, **predictive modeling**, and **DOE analysis**.

---

## Data Subsets

| Subset | Description |
|--------|-------------|
| **Traceable registry** | Full set of deposition runs with complete metadata |
| **Height-resolved subset** | Runs with validated longitudinal height profiles |
| **Paired geometry subset** | Runs with both height and multi-level width descriptors |

These subsets ensure analyses use only validated, quality-controlled records.

---

##  Metrology & Profilometry

Profilometric imaging is performed using a **Keyence VR‑600 optical scanner**, producing:

- 3D surface reconstructions  
- Longitudinal height profiles at seven standardized locations  
- Multi-level width measurements at normalized height fractions  
- High-resolution point clouds  

All scans are linked to their corresponding `exp_id`.

---

## Geometric Descriptors

The WAAM Logger provides standardized geometry metrics, including:

- Mean height and height variation  
- Multi-level width measurements  
- Aspect ratio  
- Core-region descriptors  
- Longitudinal uniformity metrics  

These descriptors follow the definitions in the WAAM Logger workflow and are reproducible across runs.

---

##  Benchmark Models

The repository includes baseline predictive models for:

- Mean height  
- Height variation  
- Representative width  
- Aspect ratio  

Models use **grouped, condition-disjoint validation** to avoid leakage across replicates.  
These baselines provide a reference point for new machine-learning approaches.

---

##  FAIR Compliance

The dataset follows the **FAIR data principles**:

- **Findable:** Unique `exp_id`, searchable metadata, repository DOI  
- **Accessible:** Repository landing page and access protocol  
- **Interoperable:** CSV/Parquet formats, schema, controlled vocabulary, SI units  
- **Reusable:** Provenance, QC flags, environment files, examples, changelog  

The mapping follows the **data‑pedigree intent of ASTM F3490 and ISO/ASTM guidance**.  
Formal standards compliance was not independently assessed.

---

##  Citation

If you use this dataset, please cite:

```
[Insert citation for WAAM Logger paper or dataset DOI]
```

---

## ** Contact**

For questions, contributions, or collaboration inquiries, please open an issue or contact the maintainers.
