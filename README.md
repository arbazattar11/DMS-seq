# DMS-seq Data Analysis Pipeline

This pipeline is designed to analyze DMS-seq sequencing data. Below are the steps involved:

1. **Quality Control (QC) for DMS-seq Data:**
   - FASTQ files are checked for quality using FastQC, and a summary report is generated.

2. **Read Alignment for DMS-seq Data:**
   - Reads are aligned to the reference genome using BWA, and sorted and indexed BAM files are generated.

3. **Peak Calling for DMS-seq Data:**
   - DMS-modified sites are identified using DMS-seq specific algorithms like DMS-MaPseq.

4. **Annotation of DMS-modified Sites:**
   - Annotate the identified DMS-modified sites with genomic features using tools like BEDTools and annotatePeaks.pl.

5. **Visualization and Interpretation:**
   - Visualize and interpret the identified DMS-modified sites to gain insights into RNA secondary structure.

## Usage
- Clone this repository.
- Place your DMS-seq FASTQ files and reference genome in the same directory as the pipeline script.
- Modify the script as necessary to specify paths and parameters.
- Run the pipeline using `./pipeline.sh`.

## Requirements
- BWA
- Samtools
- BEDTools
- DMS-seq specific algorithms/tools (e.g., DMS-MaPseq)
- FastQC
- Deeptools (for visualization)

## Notes
- Adjust parameters and additional analysis steps based on specific experimental needs.
- Ensure reference genome files are available and properly indexed.
