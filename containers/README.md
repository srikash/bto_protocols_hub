# Processing Pipelines — Docker Containers

Docker containers for the BRAIN-TO processing pipelines are hosted on DockerHub.

> **No local installation of FSL, Python, or other dependencies required.**
> You only need [Docker](https://docs.docker.com/get-docker/) installed.

---

## Available Containers

| Pipeline | Description | DockerHub Image | Status |
|---|---|---|---|
| Fieldmap pipeline | Dual-echo GRE and phase-difference fieldmap computation | TBD | Coming soon |
| fMRI preprocessing | TOPUP distortion correction + FLIRT registration | TBD | Coming soon |
| Diffusion preprocessing | TBD | TBD | Coming soon |
| ASL processing | TBD | TBD | Coming soon |

---

## Usage (once published)

```bash
# Pull a container
docker pull braintolab/<image-name>:<tag>

# Run (example — update path and arguments per pipeline)
docker run --rm \
  -v /path/to/your/data:/data \
  braintolab/<image-name>:<tag> \
  --input /data/input --output /data/output
```

---

## Questions or Problems

Open a [processing issue](../../../issues/new?template=processing.yml) on GitHub.
