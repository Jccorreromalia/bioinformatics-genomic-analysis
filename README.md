# Bioinformatics Genomic Analysis

Comparative genomic and bioinformatics analysis of the **POLR1C** gene associated with **Treacher Collins Syndrome**, including orthologue identification, multiple sequence alignment, comparative protein analysis, phylogenetic inference and genome assembly workflows.

---

# Project Overview

This repository contains **two independent bioinformatics workflows** developed as part of an academic bioinformatics project.

Although both analyses were performed within the same course context and using similar bioinformatic methodologies, they correspond to different biological objectives and workflows.

The repository is therefore divided into:

1. **Comparative Genomic Analysis of the POLR1C Gene**
2. **Genome Assembly and Annotation Workflow**

The analyses were mainly performed using the **Galaxy bioinformatics platform** together with external bioinformatic tools.

---

# PART I — Comparative Genomic Analysis of POLR1C

## Biological Background

The first part of the project focuses on the bioinformatic analysis of the **POLR1C** gene associated with **Treacher Collins Syndrome (TCS)**.

Treacher Collins Syndrome is a rare genetic disorder characterized by craniofacial developmental abnormalities.

POLR1C encodes a subunit of RNA polymerases I and III involved in ribosomal RNA synthesis.

Mutations affecting this gene can alter ribosome biogenesis, leading to:

* Neural crest cell apoptosis
* Oxidative stress
* Craniofacial developmental defects

The objective of this section was to study the evolutionary conservation and comparative genomics of POLR1C across multiple mammalian species.

---

## Workflow

### 1. Disease and Gene Selection

A literature review was performed to understand:

* The molecular basis of Treacher Collins Syndrome
* The biological role of POLR1C
* Mutation-associated phenotypes
* Experimental therapeutic approaches

The project also reviewed experimental studies involving zebrafish models and TP53-associated apoptosis mechanisms.

---

### 2. Sequence Retrieval

Nucleotide and protein sequences were retrieved from:

* NCBI
* UniProt

Sequences included:

* Human reference sequences
* Mammalian orthologue sequences

Species analyzed:

* Homo sapiens
* Pan troglodytes
* Pan paniscus
* Pongo abelii
* Panthera leo
* Acinonyx jubatus
* Puma yagouaroundi
* Equus quagga
* Diceros bicornis minor
* Hippopotamus amphibius kiboko

---

### 3. Orthologue Identification

Orthologue searches were performed across multiple taxa.

The original objective was to identify orthologues in:

* Mammals
* Plants
* Bacteria

However, no significant orthologues were identified in plants or bacteria.

The analysis therefore focused on mammalian evolutionary conservation.

---

### 4. Multiple Sequence Alignment (MSA)

Multiple sequence alignments were performed using **Clustal Omega**.

Two independent alignments were generated:

#### Nucleotide alignment

Used for:

* Comparative genomics
* Conservation analysis
* Identity matrix generation
* Phylogenetic analysis

#### Protein alignment

Used for:

* Conserved motif identification
* Functional conservation analysis
* Structural comparison

The alignments revealed strong evolutionary conservation among mammalian species.

---

### 5. Protein Analysis and Secondary Structure Prediction

Protein sequences corresponding to the POLR1C orthologues were analyzed to identify:

* Conserved regions
* Conserved domains
* Structurally important motifs

Secondary structure prediction analyses suggested that conserved sequence regions are associated with structurally and functionally essential protein regions.

---

### 6. Phylogenetic Analysis

Phylogenetic analyses were performed using **MEGA (Molecular Evolutionary Genetics Analysis)**.

The workflow included:

1. Sequence alignment
2. Evolutionary model selection
3. Maximum Likelihood tree generation
4. Bootstrap analysis

Both linear and circular phylogenetic trees were generated to evaluate evolutionary relationships among mammalian orthologues.

---

# PART II — Genome Assembly and Annotation Workflow

The second part of the repository corresponds to an independent genome assembly and sequencing quality analysis workflow.

This section focuses on the comparison of different sequencing technologies and assembly strategies.

Unlike the POLR1C analysis, this workflow is not related to Treacher Collins Syndrome.

---

## Workflow

### 1. Sequencing Datasets

The workflow used two different sequencing technologies:

#### Illumina paired-end reads

Datasets:

* SRR3137854-forward.fastqsanger
* SRR31378544-reverse.fastqsanger

#### Nanopore long reads

Dataset:

* SRR21079301.fastq

Raw FASTQ files are not included in this repository due to GitHub file size limitations.

---

### 2. Sequencing Quality Analysis

Read quality was evaluated using:

* FastQC
* MultiQC
* NanoPlot

The analyses included:

* Quality score evaluation
* GC content analysis
* Adapter contamination assessment
* Duplication analysis
* Read length distribution
* Coverage estimation

---

### 3. Genome Assembly

Different assembly approaches were compared depending on the sequencing technology used.

#### SPAdes

Used for Illumina short reads.

#### Flye

Used for Nanopore long reads.

---

### 4. Assembly Evaluation

Assemblies were evaluated using:

* QUAST

Parameters evaluated included:

* Misassemblies
* Indels
* Mismatches
* Fragmentation
* Structural accuracy

The SPAdes assembly showed higher structural accuracy, while Flye generated more complete but less precise assemblies.

---

# Repository Structure

```text
bioinformatics-genomic-analysis/
│
├── presentation/
├── sequences/
├── phylogenetic-analysis/
└── assembly-and-annotation/
```

## `presentation/`

Contains the final report and project presentation.

## `sequences/`

Contains all nucleotide and protein FASTA sequences used during the project.

Includes:

* Human reference sequences
* Mammalian orthologues
* Multi-FASTA alignment files

## `phylogenetic-analysis/`

Contains files related to phylogenetic inference and evolutionary analysis.

Includes:

* MEGA project files
* Alignment files

## `assembly-and-annotation/`

Contains files and documentation related to sequencing quality analysis and genome assembly workflows.

---

# Technologies and Tools

## Bioinformatics Platforms

* Galaxy
* NCBI
* UniProt

## Alignment and Phylogeny

* Clustal Omega
* MEGA

## Sequencing Quality Analysis

* FastQC
* MultiQC
* NanoPlot

## Genome Assembly

* SPAdes
* Flye
* QUAST

---

# Notes

Some raw sequencing datasets were not uploaded due to GitHub file size limitations.

Datasets used during the project include:

* SRR3137854
* SRR21079301

---

# Author

Juan Carlos Correro Malia

Biomedical Sciences / Genomics&Proteomics-related academic project.
