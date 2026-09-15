# BRAIN-TO (BTO) MRI Protocols

Optimised MRI acquisition protocols for Siemens 3 T and 7 T systems running XA60.

## Motivation

MRI research is becoming more collaborative while scanner time and research
funding are under increasing pressure. Data are also being reused more often:
a control group acquired for one study may support another study, and datasets
collected at different sites may be combined.

That work depends on acquisition parameters being shared and understood. In
practice, protocols often vary between studies at the same site. Small changes
in resolution, timing, acceleration, reconstruction, or coil configuration can
make data harder to compare and can affect later processing. The problem is
larger in multi-site studies, where local scanner setups and established
practices already differ.

Access is another constraint. Hospitals and research groups may not be able to
obtain or maintain specialised research sequences. BRAIN-TO uses Siemens
product sequences so that collaborating sites can implement the protocols
without Work-in-Progress packages or C2Ps.

BRAIN-TO provides a stable starting point for researchers, MR physicists, and
technologists who need dependable protocols without designing every sequence
from scratch. The aim is consistent performance and practical reuse, rather
than pushing individual scanner settings to their limit.

## Design principles

The protocol sets follow a small number of practical principles:

- They use Siemens product sequences that can be shared across sites.
- They favour isotropic voxels to support consistent spatial sampling and
  reduce partial-voluming concerns.
- Most scans target 5–6 minutes at 3 T and 6–8 minutes at 7 T. Multi-echo
  FLASH, multi-shell diffusion, resting-state MRI, and functional MRI can take
  longer where the acquisition needs it.
- They use the acceleration available from the head coil, with variants where
  coil configuration changes the appropriate protocol choice.
- Data acquired with BRAIN-TO protocols have been evaluated with
  community-standard MRI processing software.

These principles support general-purpose acquisitions that can be implemented
locally and used reliably in downstream research workflows.

## Choose a protocol collection

| Scanner | Protocol sets | Download |
|---|---|---|
| 3 T XA60 | Anatomy, fMRI, diffusion, ASL | [3 T protocol page](3T/README.md) · Zenodo link to be added |
| 7 T XA60 | Anatomy, fMRI, diffusion | [7 T protocol page](7T/README.md) · Zenodo link to be added |

Each field-strength page describes the collection and will link directly to
its Zenodo record.

The 7 T collection does not include a product ASL protocol. If you are
interested in 7 T ASL options, contact
[sriranga.kashyap@utoronto.ca](mailto:sriranga.kashyap@utoronto.ca).

## Scripts and processing

- [3 T scripts](3T/scripts/README.md)
- [7 T scripts](7T/scripts/README.md)

GHCR container links will be listed on the relevant field-strength page when
they are available.

## Use in research

Before using a protocol, confirm that it is appropriate for the local scanner
configuration, coil, participant group, safety procedures, ethics approval,
and study question. Local MR physics and technologist review remains essential.

## Previous version

The complete XA30 protocol set is available on the
[`xa30_archive`](../../tree/xa30_archive) branch.

## Contact

For questions about protocol selection, implementation, or 7 T ASL options,
email [sriranga.kashyap@utoronto.ca](mailto:sriranga.kashyap@utoronto.ca).
