---
title: Predicting evolutionary innovation
description: Mapping genotype to phenotype to fitness across species, to predict how and when plants adapt.
icon: spark
weight: 30
eyebrow: "Theme 3 · Extending to more traits"
keywords: [Convergent evolution, Phylogenetic mixed models, Adaptation, Heat & salt tolerance, Common garden]
# DOIs of related papers, as they appear in the CV (shown in CV order):
publications:
  - https://doi.org/10.1093/molbev/msaf324
  - https://doi.org/10.64898/2026.06.01.729361
---

## The idea

Different environments select for different traits, and over time this leaves a mark on the
genomes of the species living there. If species are best adapted to their native habitats, then
across many species we expect habitat, adaptive traits and the genes that shape them to vary
together, even among distantly related species. Mapping these links from **genotype to phenotype
to fitness** is the key to understanding, and eventually predicting, adaptation.

## What our proof of concept showed

In {{< paper doi="10.64898/2026.06.01.729361" text="our convergent-adaptation study" >}}, we combined the habitats from our [niche work](../niche/) with gene-activity scores
from our [AI models](../ai-genomics/) in **phylogenetic mixed models**, which separate repeated
change from shared ancestry.

- **Genome-wide shifts.** Lineages entering similar environments shifted in the same directions
  in proteome-wide properties, such as the nitrogen-to-carbon balance and the biosynthetic cost
  of their proteins.
- **Recurring genes.** Several hundred genes were repeatedly associated with distinct axes of
  environmental variation, enriched for proteins working in extracellular and organellar
  compartments.
- **Predictable routes.** Grass adaptation appears channeled by layered constraints at
  genome-wide and gene-specific scales, which makes evolutionary trajectories partly predictable.

## Extending to more traits

So far, the environment has stood in for the phenotype. Next we measure the phenotypes directly:

- **Common gardens.** Controlled heat and salt stress experiments on about 100 representative
  grass species, measuring molecular and whole-plant traits to fill the phenotype layer between
  genes and environments.
- **Traits we focus on:** heat and salt resilience, the most pressing challenges for agriculture
  and grasslands in Taiwan; nutrient use, building on our {{< paper doi="10.1111/tpj.70319" text="rhizosphere nitrogen work" >}}; the
  evolution of perennial and annual life histories; and cold and freezing tolerance.

The resulting candidate genes and variants are concrete targets for breeding climate-resilient
crops and for guiding conservation.
