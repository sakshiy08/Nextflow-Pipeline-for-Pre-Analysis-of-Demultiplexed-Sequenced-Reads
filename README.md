# Nextflow-Pipeline-for-Pre-Analysis-of-Demultiplexed-Sequenced-Reads

Sequencing reads from a multiplexed library are initially separated based on their barcode sequences into different subdirectories during the demultiplexing process. This step ensures that reads originating from different samples can be distinguished and analyzed separately. As part of the pre-analysis data processing pipeline, these reads are then concatenated according to their barcodes. This concatenation aggregates all reads belonging to the same sample into a single file, facilitating downstream bioinformatics workflows. Additionally, each concatenated file is labeled with the actual sample name derived from metadata associated with the barcode, enabling clear identification and tracking of each sample throughout the analysis pipeline.

This pre-analysis preparation can be done manually or by using a bash script shown in the file <preprocessing.sh>

But if the workflow starts from the barcode subdirectories, contanetanes the reads, labels them, and feeds into the downstream analyses. This will make this process fully automated from the start to the end 


