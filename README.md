# ACEiP_DB

A curated database of **ACE (Angiotensin-Converting Enzyme) inhibitory peptides** with physicochemical properties and literature references.

## Overview

This database contains **1,807 peptide entries** collected from published literature, covering peptide sequences ranging from **2 to 50 amino acids** in length. Each entry includes experimentally reported IC50 values (where available), physicochemical descriptors, and traceable literature sources.

## Data Fields

| Field | Description |
|-------|-------------|
| `Seq` | Peptide amino acid sequence |
| `length` | Sequence length |
| `ic50` | IC50 value with unit (e.g., μM, mM) |
| `reference` | Source publication title(s) |
| `doi` | Digital Object Identifier(s) |
| `PubMedID` | PubMed identifier(s) |
| `MW (Da)` | Molecular weight in Daltons |
| `pI` | Isoelectric point |
| `Charge (pH7)` | Net charge at pH 7.0 |
| `GRAVY` | Grand average of hydropathicity |
| `Instability` | Instability index |
| `Hydrophobic%` | Fraction of hydrophobic residues |
| `Boman Index` | Potential protein interaction index |
| `Helix%` | Predicted α-helix propensity |
| `Turn%` | Predicted turn propensity |
| `Sheet%` | Predicted β-sheet propensity |

## Statistics

- **Total entries**: 1,807
- **Entries with IC50 data**: 1,257 (69.6%)
- **Entries with DOI**: 1,139
- **Entries with PubMed ID**: 1,194
- **Peptide length range**: 2–50 amino acids

## Usage

```python
import pandas as pd

df = pd.read_excel("ACEiP_DB.xlsx", sheet_name="ACEiP_Properties")
```

## License

This database is compiled from publicly available literature for academic research purposes.

## Citation

If you use this database in your research, please cite the original publications referenced in the `reference`, `doi`, and `PubMedID` columns.
