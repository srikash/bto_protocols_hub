# Helper Scripts

Individual processing steps for BRAIN-TO data. These scripts wrap FSL and Python tools.

> **Prefer containers?** See [containers/README.md](../containers/README.md) — no local installation needed.

---

## Dependencies

| Tool | Minimum version | Install |
|---|---|---|
| Python | 3.8 | [python.org](https://www.python.org/downloads/) |
| FSL | 6.0 | [fsl.fmrib.ox.ac.uk](https://fsl.fmrib.ox.ac.uk/fsl/docs/#/install/index) |

Python package requirements: `requirements.txt` — coming soon.

---

## Scripts

### `scanbids.py` — BIDS Dataset Summary

Prints a summary of files in a BIDS-formatted dataset directory.

```bash
python scripts/scanbids.py --bids_dir /path/to/bids
```

---

### `fieldmap/dualecho_fieldmap.sh` — Dual-Echo GRE Fieldmap

Computes a fieldmap from a dual-echo GRE acquisition using FSL tools.

```bash
bash scripts/fieldmap/dualecho_fieldmap.sh \
  --echo1 /path/to/echo1.nii.gz \
  --echo2 /path/to/echo2.nii.gz \
  --output /path/to/output
```

---

### `fieldmap/phasediff_fieldmap.sh` — Phase-Difference Fieldmap

Computes a fieldmap from a phase-difference image using FSL PRELUDE and FUGUE.

```bash
bash scripts/fieldmap/phasediff_fieldmap.sh \
  --phasediff /path/to/phasediff.nii.gz \
  --magnitude /path/to/magnitude.nii.gz \
  --output /path/to/output
```

---

### `preprocessing/run_fsl_flirt.py` — Linear Registration (FSL FLIRT)

Registers a moving image to a reference using FSL FLIRT with BBR cost function.

```bash
python scripts/preprocessing/run_fsl_flirt.py \
  --moving /path/to/moving.nii.gz \
  --reference /path/to/reference.nii.gz \
  --output /path/to/output
```

---

### `preprocessing/run_fsl_topup.py` — Distortion Correction (FSL TOPUP)

Corrects susceptibility-induced distortions using FSL TOPUP.

```bash
python scripts/preprocessing/run_fsl_topup.py \
  --input /path/to/epi.nii.gz \
  --blip_up /path/to/blip_up.nii.gz \
  --blip_down /path/to/blip_down.nii.gz \
  --output /path/to/output
```

---

## Known Issues

See [REVIEW.md](../REVIEW.md) §3 and §5 for a full list of bugs and planned fixes.
