# Awesome Phage Structure 🦠🤖
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0](https://img.shields.io/badge/License-CC0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/shandley/awesome-phage-structure/pulls)

> A curated list of AI and deep learning tools for phage functional annotation and structural biology

## 🎯 Mission

This repository aims to catalog and organize the rapidly growing ecosystem of AI/ML tools that can help illuminate phage "dark matter" - the vast majority of phage genes with unknown function. By leveraging structure prediction, protein language models, and advanced computational methods, these tools are revolutionizing our understanding of phage biology.

## 📚 Contents

- [Protein Structure Prediction](#-protein-structure-prediction)
- [Functional Annotation Tools](#-functional-annotation-tools)
- [Protein-Protein Interactions](#-protein-protein-interactions)
- [Sequence Analysis & Language Models](#-sequence-analysis--language-models)
- [Structural Databases & Resources](#️-structural-databases--resources)
- [Downstream Analysis Tools](#-downstream-analysis-tools)
- [Computational Platforms & Workflows](#-computational-platforms--workflows)
- [Benchmarks & Datasets](#-benchmarks--datasets)
- [Contributing](#-contributing)
- [Resources & Reviews](#-resources--reviews)

---

## 🧬 Protein Structure Prediction

Tools for predicting 3D structures of phage proteins from sequence alone.

### General Purpose Structure Prediction

- **[AlphaFold3](https://github.com/google-deepmind/alphafold3)** - Latest iteration of AlphaFold with improved accuracy for protein complexes, nucleic acids, and small molecules `[2024]`
  - Web server: [AlphaFold Server](https://alphafoldserver.com)
  - Supports protein-DNA/RNA interactions crucial for phage biology

- **[Boltz-1](https://github.com/jwohlwend/boltz)** `[pip]` - First fully open-source model approaching AlphaFold3 accuracy `[2024]`
  - MIT licensed alternative to AlphaFold
  - Supports proteins, nucleic acids, small molecules, and modified residues
  
- **[ESMFold](https://github.com/facebookresearch/esm)** `[pip, conda]` - Language model-based structure prediction `[2023]`
  - Fast single-sequence structure prediction
  - No MSA required, ideal for novel phage proteins

- **[BioEmu](https://github.com/microsoft/bioemu)** `[pip]` - Microsoft's biomolecular emulator for sampling protein structural ensembles `[2024]`
  - Generates multiple conformations from single sequence
  - Useful for understanding protein flexibility

- **[RoseTTAFold2](https://github.com/uw-ipd/RoseTTAFold2)** `[conda]` - Enhanced accuracy for protein-nucleic acid complexes `[2023]`
  - Particularly good for DNA-binding proteins

### Specialized Phage Structure Tools

- **[ColabFold](https://github.com/sokrypton/ColabFold)** `[conda, docker]` - User-friendly AlphaFold2 implementation `[2024]`
  - Optimized for batch processing of phage proteomes
  - Google Colab notebooks available

## 🔬 Functional Annotation Tools

AI-powered tools for assigning functions to phage proteins.

### Structure-Based Annotation

- **[phold](https://github.com/gbouras13/phold)** `[pip, conda]` - Phage annotation using protein structural homology `[2024]`
  - Uses ProstT5 protein language model for 3Di representations
  - Searches 1.36 million phage protein structures
  - Integrates PHROGs, CARD, VFDB databases

- **[Foldseek](https://github.com/steineggerlab/foldseek)** `[conda, docker]` - Ultra-fast structural alignment `[2024]`
  - 3Di alphabet for structure representation
  - Powers phold's structural searches

### Sequence-Based Functional Prediction

- **[Pharokka](https://github.com/gbouras13/pharokka)** `[pip, conda]` - Fast phage genome annotation `[2024]`
  - PHROGs and VFDB integration
  - Combines with phold for enhanced accuracy

- **[PhageAI](https://phage.ai/)** - Web platform for phage genome analysis `[2024]`
  - Lifestyle prediction
  - Host range analysis

## 🧪 Protein-Protein Interactions

Tools for predicting phage-host and protein complex interactions.

- **[Boltz-2](https://github.com/jwohlwend/boltz)** `[pip]` - Joint structure and binding affinity prediction `[2024]`
  - 1000x faster than physics-based FEP methods
  - Crucial for understanding phage-host interactions

- **[AlphaFold-Multimer](https://github.com/google-deepmind/alphafold)** `[docker]` - Protein complex structure prediction `[2023]`
  - Predicts quaternary structures
  - Useful for tail proteins and receptor binding

- **[DiffDock](https://github.com/gcorso/DiffDock)** `[pip]` - Molecular docking using diffusion models `[2024]`
  - Predicts small molecule binding sites
  - Applications in phage-antibiotic synergy

## 📊 Sequence Analysis & Language Models

Large language models trained on biological sequences.

### DNA Language Models

- **[Evo2](https://github.com/arcinstitute/evo2)** `[pip, docker]` - DNA foundation model with 1M base pair context `[2024]`
  - Trained on 8.8 trillion tokens across all domains of life
  - Zero-shot variant effect prediction
  - Generate DNA sequences from prompts

- **[DNABERT-2](https://github.com/MAGICS-LAB/DNABERT_2)** `[pip]` - Bidirectional encoder for DNA `[2024]`
  - Pre-trained on multi-species genomes
  - Fine-tunable for phage-specific tasks

### Protein Language Models

- **[ESM-2](https://github.com/facebookresearch/esm)** `[pip, conda]` - 15B parameter protein language model `[2023]`
  - Zero-shot function prediction
  - Variant effect prediction

- **[ProtTrans](https://github.com/agemagician/ProtTrans)** `[pip]` - Collection of protein transformers `[2023]`
  - Multiple architectures (BERT, T5, XLNet)
  - Pre-trained embeddings for downstream tasks

- **[ProstT5](https://github.com/mheinzinger/ProstT5)** `[pip]` - Protein language model for 3Di sequences `[2024]`
  - Bilingual model (amino acids + 3Di)
  - Powers phold's structural searches

## 🗄️ Structural Databases & Resources

Curated databases of phage and viral structures.

### Specialized Phage Databases

- **[BFVD](https://bfvd.steineggerlab.workers.dev)** - Bacteriophage Function and Structure Database `[2024]`
  - Comprehensive structural annotations
  - Functional domain predictions
  - Interactive visualization

- **[Viro3D](https://viro3d.cvr.gla.ac.uk)** - Viral capsid and genome organization database `[2024]`
  - 3D capsid reconstructions
  - Genome packaging visualizations

- **[PhageScope](https://phagescope.deepomics.org/)** - Phage genome and structure browser `[2024]`
  - Integrated structural predictions
  - Taxonomic organization

### General Structural Resources

- **[PDB](https://www.rcsb.org/)** - Protein Data Bank `[Updated daily]`
  - Experimentally determined structures
  - Growing collection of phage proteins

- **[AlphaFold Database](https://alphafold.ebi.ac.uk/)** - Pre-computed structure predictions `[2024]`
  - Covers multiple proteomes
  - Downloadable structures

- **[ESM Metagenomic Atlas](https://esmatlas.com/)** - 617M protein structure predictions `[2023]`
  - Includes environmental phage proteins
  - Searchable by sequence

## 🔍 Downstream Analysis Tools

Tools for analyzing and validating predicted structures, identifying functional sites, and understanding structural implications.

### Structure Validation & Quality Assessment

- **[MolProbity](http://molprobity.biochem.duke.edu/)** `[web]` - Comprehensive structure validation service `[2024]`
  - Validates protein geometry and steric clashes
  - Particularly useful for AI-predicted structures

- **[SAVES v6.0](https://saves.mbi.ucla.edu/)** `[web]` - Structure validation server suite `[2024]`
  - Includes VERIFY3D, ERRAT, PROVE, PROCHECK
  - Generates detailed quality reports

- **[QMEAN](https://swissmodel.expasy.org/qmean/)** `[web, API]` - Quantitative Model Energy ANalysis `[2024]`
  - Estimates model quality for entire structures
  - Provides local quality estimates per residue

### Functional Site & Domain Prediction

- **[CASTp](http://sts.bioe.uic.edu/castp/)** `[web]` - Computed Atlas of Surface Topography of proteins `[2024]`
  - Identifies and measures protein pockets and cavities
  - Essential for understanding phage-host binding sites

- **[InterProScan](https://www.ebi.ac.uk/interpro/search/sequence/)** `[web, API, docker]` - Functional domain identification `[2024]`
  - Scans against multiple domain databases
  - Includes Pfam, SMART, CDD, SUPERFAMILY

- **[DALI](http://ekhidna2.biocenter.helsinki.fi/dali/)** `[web]` - Structure-based domain identification `[2024]`
  - Compares structures against PDB database
  - Identifies remote homologs missed by sequence methods

- **[ConSurf](https://consurf.tau.ac.il/)** `[web]` - Evolutionary conservation analysis `[2024]`
  - Maps conservation scores onto 3D structures
  - Identifies functionally important regions

### Binding Site & Interaction Prediction

- **[P2Rank](https://github.com/rdk/p2rank)** `[source, docker]` - Machine learning-based pocket prediction `[2024]`
  - Ligand binding site prediction
  - Works well with AlphaFold structures

- **[ProBiS](http://probis.cmm.ki.si/)** `[web]` - Protein Binding Sites detection `[2024]`
  - Detects structurally similar binding sites
  - Database of 400,000+ protein structures

- **[PLIP](https://plip-tool.biotec.tu-dresden.de/)** `[web, source]` - Protein-Ligand Interaction Profiler `[2024]`
  - Analyzes and visualizes protein-ligand interactions
  - Useful for phage-antibiotic synergy studies

### Electrostatics & Surface Analysis

- **[APBS](https://www.poissonboltzmann.org/)** `[source, web]` - Adaptive Poisson-Boltzmann Solver `[2024]`
  - Calculates electrostatic properties
  - Critical for understanding phage tail-receptor interactions

- **[PDB2PQR](https://pdb2pqr.poissonboltzmann.org/)** `[web, source]` - Prepares structures for electrostatics calculations `[2024]`
  - Assigns charges and radii
  - Optimizes hydrogen bonding networks

### Structural Alignment & Comparison

- **[TM-align](https://zhanggroup.org/TM-align/)** `[web, source]` - Structure alignment independent of sequence `[2024]`
  - Robust for comparing distantly related proteins
  - Provides TM-score for quality assessment

- **[FATCAT](https://fatcat.godziklab.org/)** `[web, source]` - Flexible structure alignment `[2024]`
  - Detects conformational changes
  - Useful for comparing different phage protein states

- **[PDBeFold](https://www.ebi.ac.uk/msd-srv/ssm/)** `[web]` - Secondary Structure Matching service `[2024]`
  - Fast 3D structure comparison
  - Interactive superposition viewer

### Mutation Effect Prediction

- **[DynaMut2](http://biosig.unimelb.edu.au/dynamut2/)** `[web]` - Predicts mutation effects on stability and dynamics `[2024]`
  - Analyzes impact on protein stability
  - Includes dynamics and conformational changes

- **[FoldX](http://foldxsuite.crg.eu/)** `[source]` - Protein design and mutational effects `[2024]`
  - Quantitative estimation of interaction energies
  - Useful for engineering phage proteins

- **[SAAFEC-SEQ](https://compbio.cs.toronto.edu/saafec-seq/)** `[web]` - Sequence-based mutation effect prediction `[2024]`
  - Predicts functional effects of mutations
  - No structure required

## 🧮 Computational Platforms & Workflows

Integrated platforms for phage analysis pipelines.

### Analysis Pipelines

- **[PhageCloud](https://phagecloud.com/)** - Cloud-based phage analysis platform `[2024]`
  - Automated annotation pipelines
  - Visualization tools

- **[Galaxy-Phage](https://cpt.tamu.edu/galaxy-pub/)** - Galaxy instance for phage genomics `[2024]`
  - Pre-configured workflows
  - Educational resources

### Visualization & Analysis

- **[ChimeraX](https://www.cgl.ucsf.edu/chimerax/)** `[conda]` - Molecular visualization with AlphaFold integration `[2024]`
  - Structure analysis tools
  - Publication-quality figures

- **[PyMOL](https://pymol.org/)** `[conda, pip]` - Molecular visualization system `[2024]`
  - Extensive plugin ecosystem
  - Scripting capabilities

- **[Mol*](https://molstar.org/)** - Web-based molecular viewer `[2024]`
  - No installation required
  - Modern, fast rendering

## 📈 Benchmarks & Datasets

Standard datasets and benchmarks for model evaluation.

### Phage-Specific Datasets

- **[PHROGs](https://phrogs.lmge.uca.fr/)** - Prokaryotic Virus Remote Homologous Groups `[2024]`
  - 38,880 protein families
  - Functional annotations

- **[INPHARED](https://github.com/RyanCook94/inphared)** - Integrated Phage Host Reference Database `[2024]`
  - Curated phage-host pairs
  - Genomic sequences

### Structure Prediction Benchmarks

- **[CASP15](https://predictioncenter.org/casp15/)** - Critical Assessment of Structure Prediction `[2024]`
  - Includes viral protein targets
  - Blind prediction challenge

- **[CAMEO](https://www.cameo3d.org/)** - Continuous Automated Model Evaluation `[Updated weekly]`
  - Rolling benchmark
  - Multiple assessment categories

## 🤝 Contributing

Contributions are warmly welcomed! Please see our [contribution guidelines](CONTRIBUTING.md) for details on:
- Adding new tools
- Updating existing entries
- Suggesting new categories
- Reporting issues

### Inclusion Criteria

Tools should be:
1. Relevant to phage functional annotation or structural biology
2. Actively maintained (updated within last 2 years)
3. Publicly available (open source preferred)
4. Documented with clear usage instructions

## 📖 Resources & Reviews

### Key Reviews & Perspectives

- [The global virome: How much diversity and how many independent origins?](https://doi.org/10.1016/j.virol.2023.05.008) (2023)
- [Illuminating the Virosphere Through Global Metagenomics](https://doi.org/10.1146/annurev-biochem-080320-103701) (2021)
- [Structure-based protein function prediction using graph neural networks](https://doi.org/10.1038/s41467-021-23303-9) (2021)

### Tutorials & Online Courses

- [SEA-PHAGES Phage Genomics Guide](https://seaphages.org/) - Comprehensive guide for phage genome annotation using DNA Master and PECAAN `[2025]`
- [CPT Galaxy Training Resources](https://cpt.tamu.edu/training-material/) - Texas A&M tutorials and videos for phage annotation `[2024]`
- [Coursera Bioinformatics Specialization](https://www.coursera.org/specializations/bioinformatics) - UC San Diego course series including genomics analysis
- [Johns Hopkins Genomic Data Science](https://www.coursera.org/specializations/genomic-data-science) - Coursera specialization with computational biology focus

### Communities & Forums

- [PhagesDB](https://phagesdb.org/) - Actinobacteriophage database and community
- [Phage Directory](https://phage.directory/) - Global phage research community
- [r/phage](https://www.reddit.com/r/phage/) - Reddit community for phage enthusiasts

---

## 📝 License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

This work is licensed under a [Creative Commons Zero v1.0 Universal License](https://creativecommons.org/publicdomain/zero/1.0/).

## 🙏 Acknowledgments

Special thanks to:
- The developers of all listed tools for advancing phage research
- The phage research community for continuous feedback
- Contributors who help keep this list updated

---

**Last Updated**: December 2024

**Maintainer**: [Scott Handley](https://github.com/shandley)

**Citation**: If you use this resource, please consider citing:
```
@misc{awesome-phage-structure,
  author = {Scott Handley},
  title = {Awesome Phage Structure: A curated list of AI tools for phage structural and functional annotation},
  year = {2024},
  publisher = {GitHub},
  url = {https://github.com/shandley/awesome-phage-structure}
}
```