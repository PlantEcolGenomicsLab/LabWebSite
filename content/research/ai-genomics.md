---
title: AI for cross-species genomics
description: Genomic language models that read gene activity directly from DNA and protein sequence, across the plant tree of life.
icon: dna
weight: 20
eyebrow: "Theme 2 · Extending to better models"
keywords: [DNA language models, Protein language models, Fine-tuning, Gene annotation, Comparative genomics]
# DOIs of related papers, as they appear in the CV (shown in CV order):
publications:
  - https://doi.org/10.1016/j.xgen.2026.101329
  - https://doi.org/10.64898/2026.11.09.765485
  - https://doi.org/10.1111/tpj.70483
---

## The challenge

Across species, the effects of mutations tend to converge at the level of whole genes rather than
single nucleotides, so comparing **orthologous genes** is central to cross-species genomics.
Classic approaches rely on multiple sequence alignments and evolutionary models, and their cost
grows steeply as more species are added.

## Language models for genomes

DNA and protein language models, such as {{< paper doi="10.1126/science.ade2574" text="ESM2" >}} for proteins and {{< paper doi="10.1073/pnas.2421738122" text="PlantCaduceus (PlantCAD)" >}} for plant
DNA, are trained on sequences from many species. Much as chat models learn the grammar of human
language, they learn the "grammar" of genomes.

- **{{< paper doi="10.64898/2026.06.01.729361" text="In our proof-of-concept study" >}}**, scores from these models detected mutational effects as subtle as
  single amino-acid changes in experimentally characterized mutants, and scaled to tens of
  thousands of genes across hundreds of grass genomes, without any alignments.
- **Plant foundation models.** With collaborators we develop DNA foundation models for plants,
  from flowering plants ({{< paper doi="10.1016/j.xgen.2026.101329" text="PlantCAD2" >}}) to bryophytes ({{< paper doi="10.64898/2026.11.09.765485" text="BryoCAD" >}}), and use them to evaluate and improve
  gene annotation ({{< paper doi="10.1111/tpj.70483" text="reelGene" >}}, {{< paper doi="10.1101/2025.10.31.685877" text="GeneCAD" >}}).

## Extending to better models

- **From zero-shot to fine-tuned.** Training models on labeled pairs of related genes, so they
  learn to rank differences in expression level and protein activity across species, not just
  spot broken genes.
- **Feeding the other themes.** These gene-activity predictions are the genotype layer of our
  [evolutionary-innovation analyses](../innovation/), and will scale to the new
  genomes from our [species sampling](../niche/).
- **Open tools.** Making the models available, so other groups can screen gene activity across
  their own species.
