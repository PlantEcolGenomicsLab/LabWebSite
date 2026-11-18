---
title: "AI models: reading gene activity from sequence"
description: Genomic language models that predict how gene function differs across species, directly from DNA and protein sequence.
icon: dna
weight: 40
keywords: [DNA language models, Protein language models, Fine-tuning, Gene annotation, Comparative genomics]
# DOIs of related papers, as they appear in the CV (shown in CV order):
publications:
  - https://doi.org/10.1016/j.xgen.2026.101329
  - https://doi.org/10.64898/2026.11.09.765485
  - https://doi.org/10.1101/2025.10.31.685877
  - https://doi.org/10.1111/tpj.70483
---

## The challenge

Across species, the effects of mutations tend to converge at the level of whole genes rather than
single nucleotides, so comparing **orthologous genes** is central to cross-species genomics.
Classic approaches rely on multiple sequence alignments and evolutionary models, and their cost
grows steeply as more species are added.

## Language models for genomes

DNA and protein language models, such as ESM2 for proteins and PlantCaduceus (PlantCAD) for plant
DNA, are trained on sequences from many species. Much as chat models learn the grammar of human
language, they learn the "grammar" of genomes. In our grass work, scores from these models
detected the effects of mutations as subtle as single amino-acid changes in experimentally
characterized mutants, and scaled to tens of thousands of genes across hundreds of genomes.

## Where we are going

- **From zero-shot to fine-tuned.** Training models on labeled pairs of related genes so they
  learn to rank differences in expression level and protein activity across species, not just
  spot broken genes.
- **Plant foundation models.** Continuing to co-develop DNA foundation models for plants, from
  flowering plants (PlantCAD2) to bryophytes (BryoCAD), and their use in genome annotation
  (GeneCAD, reelGene).
- **Open tools.** Making the fine-tuned models available, so other groups can screen gene
  activity across their own species.
