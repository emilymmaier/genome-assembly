# genome-assembly
E. coli genome assembly via Unicycler and Flye and analysis of results. Commands and arguments supplied to command line tools are captured in text files.

## Dependencies
- BLASTn 2.12.0
- Unicycler 0.4.4
- Flye 2.6
- ABRicate 1.0.0
- PlasmidFinder 2.0

## Output
genome_assembly.txt: All commands and output messages produced while using Unicycler and Flye, as well as comments describing the      process. The Unicycler assembly was executed in an HCP environment, and unfortunatley output files were not transferred to the local computer. Therefore the following output files are from the Flye assembly only.

> assembly.fasta: Result of E. coli genome assembly via Flye, this file gives the sequence of each contig.

> flye_match_ncbi.txt: blastn result comparing the Flye assembly to the reference database obtained from NCBI


genome_assembly_report.pdf: Summary of results from assemblies produced by Flye and Unicycler, as well as comparison of performance of each tool and their strengths and weaknesses.


flye_assembly_analysis.txt: All commands and output messages produced while analyzing the Flye assembly using ABRicate and PlasmidFinder, as well as comments describing the process. The Flye assembly was selected for analysis since this assembly produced fewer contigs than the Unicycler assembly.

> flye_abricate.csv: Output from analysis of the Flye assembly in ABRicate identifying antimicrobial resistance and virulance genes.
 
