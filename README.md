# LongQC-singularity
A singularity container for LongQC.

## I. Download

`LongQC.sif` can be downloaded from the [releases page](https://github.com/raspberryenvoie/LongQC-singularity/releases).

## II. Usage

```bash
singularity run LongQC.sif <parameters>
```

## III. Container implementation

1. The official LongQC [Dockerfile](https://github.com/yfukasawa/LongQC/blob/master/Dockerfile) was used as a reference.
2. The Dockerfile was converted to a Singularity `.def` file. [Singularity Python](https://singularityhub.github.io/singularity-cli/recipes) can help with that, although some adjustments may be needed.
3. A singularity container was then built from this `.def` file (cf [Github Workflow](https://github.com/raspberryenvoie/LongQC-singularity/blob/main/.github/workflows/buil_container.yml)).
