File for download:

https://zenodo.org/record/582600/files/mutant_R1.fastq
https://zenodo.org/record/582600/files/mutant_R2.fastq
https://zenodo.org/record/582600/files/wildtype.fna


use wget command to download the files

```bash
wget https://zenodo.org/record/582600/files/mutant_R1.fastq
wget https://zenodo.org/record/582600/files/mutant_R2.fastq
wget https://zenodo.org/record/582600/files/wildtype.fna
```
or download all at once using the following command

```bash
wget -i https://zenodo.org/record/582600/files/urls.txt
```
file urls.txt contains the urls of the files to be downloaded





### Homework BASH Practice 1
#### Objectives:
- Practice navigating directories using relative and absolute paths. 
- Understand and apply file and directory operations (`ls`, `cd`, `cp`, `mv`, `mkdir`). 
- Utilize wildcards and special characters (`~`, `*`, `?`, `..`). 
- Use `seqkit` for sequence data statistics.
#### Tasks: 

1. **Navigation and Directory Structure** : 
- Navigate to the `Genomics_Data` directory on your `~/Desktop/shell-lesson-data` using an absolute path. 
- Return to your home directory using the `~` shortcut. Then navigate back to `Genomics_Data` using a relative path.
- List all files in the `Genomics_Data/Raw_Data` directory. What type of files are in this directory?
- List all files ending with `.txt` in the `Genomics_Data/Info` directory in one command. 
2. **Using Wildcards and Special Characters** : 
- List all `fasta` files in `Raw_Data` using a single command and wildcards.
- List all `fasta` files with name starting with `sample` in `Raw_Data` using a single command and wildcards.
- List all `fastq` files in `Raw_Data` using a single command and wildcards. 
- Create directory `fastq` in `Processed_Data` and **copy** all `fastq` files from `Raw_Data` to `Processed_Data/fastq` using a single command and wildcards.
- Create directory `fasta` in `Processed_Data` and **move** all `fasta` files from `Raw_Data` to `Processed_Data/fasta` using a single command and wildcards.
3. **Get sequence statistics using `seqkit` program** :
- Navigate to `Processed_Data/fasta` and use `seqkit stats` to get statistics for all `.fasta` files. Use wildcards to select all `.fasta` files.
- To write the statistics to a file, use `seqkit stats` with `-o` option: `seqkit stats *.fasta -o fasta_stats.txt`.
- Does the fasta files contain protein or nucleotide sequences?
- Navigrate to `Processed_Data/fastq` and use `seqkit stats` to get statistics for all `.fastq` files. Use wildcards to select all `.fastq` files.
- To write the statistics to a file, use `seqkit stats` with `-o` option: `seqkit stats *.fastq -o fastq_stats.txt`. 
- What is the average read length for each fastq file?

#### Homework Submission:
From konsole menu use `File` -> `Save Output` to save the output of the commands to a text file.

