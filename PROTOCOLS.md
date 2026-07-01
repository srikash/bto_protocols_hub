# BRAIN-TO Protocol Parameter Reference

Protocols target the **Siemens MAGNETOM Prisma 3T** running **XA30 software**.

> For full acquisition parameters, download the PDF from each Zenodo record.

---

## Protocol Sets

| Set | Modalities | Zenodo DOI | Download |
|---|---|---|---|
| Complete | All below | 10.5281/zenodo.10685481 | [Link](https://zenodo.org/records/10685481) |
| Anatomy | T1w, T2w, FLAIR, MWF | 10.5281/zenodo.10685475 | [Link](https://zenodo.org/records/10685475) |
| fMRI | BOLD, ME-BOLD | 10.5281/zenodo.10685458 | [Link](https://zenodo.org/records/10685458) |
| Diffusion | DWI, DTI | 10.5281/zenodo.10685449 | [Link](https://zenodo.org/records/10685449) |
| ASL | pCASL | 10.5281/zenodo.10685308 | [Link](https://zenodo.org/records/10685308) |

---

## Detailed Parameters

> **Note:** Operating mode (1st-level / 2nd-level), SAR limits, and acceleration factors require physicist sign-off before clinical use. See [REVIEW.md](REVIEW.md) §6.

### Anatomy Set

| Sequence | Resolution | TR (ms) | TE (ms) | Acceleration | Notes |
|---|---|---|---|---|---|
| T1w MP2RAGE | TBD | TBD | TBD | TBD | |
| T2w SPACE | TBD | TBD | TBD | TBD | |
| FLAIR | TBD | TBD | TBD | TBD | |
| MWF | TBD | TBD | TBD | TBD | |

### fMRI Set

| Sequence | Resolution | TR (ms) | TE (ms) | Volumes | Acceleration | Notes |
|---|---|---|---|---|---|---|
| BOLD EPI | TBD | TBD | TBD | TBD | TBD | |
| ME-BOLD EPI | TBD | TBD | TBD | TBD | TBD | Multi-echo |

### Diffusion Set

| Sequence | Resolution | TR (ms) | b-values | Directions | Acceleration | Notes |
|---|---|---|---|---|---|---|
| DWI EPI | TBD | TBD | TBD | TBD | TBD | |

### ASL Set

| Sequence | Resolution | TR (ms) | PLD (ms) | Label duration (ms) | Notes |
|---|---|---|---|---|---|
| pCASL | TBD | TBD | TBD | TBD | |

---

## Compatibility

| Item | Status |
|---|---|
| Target platform | Siemens MAGNETOM Prisma 3T |
| Software version | XA30 |
| Other Prisma versions | See PDF parameter sheets on Zenodo |
| Non-Prisma scanners | Not validated |
