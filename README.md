# Greenland mycorrhiza 2

Mapping of shotgun sequencing data against the UNITE database. Updated analysis pipeline using Snakemake 8, the 2025 version of the UNITE database and a second batch of data. The old repository can be found in: https://github.com/alberdilab/greenland_mycorrhiza


# Usage

## Clone repository

```sh
git clone https://github.com/alberdilab/greenland_mycorrhiza2.git
```

## Add reads and UNITE

Place all reads in: **resources/reads**
Place the decompressed fasta file of the UNITE database in: **resources/database**

UNITE database for all eukaryotes: https://s3.hpc.ut.ee/plutof-public/original/b02db549-5f04-43fc-afb6-02888b594d10.tgz

## Run the pipeline

```sh
screen -S greenland_mycorrhiza2
cd greenland_mycorrhiza2
snakemake --workflow-profile profile/slurm
```
