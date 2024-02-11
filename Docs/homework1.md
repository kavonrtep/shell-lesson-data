## Homework BASH 1
### Objectives:
- Practice navigating directories using relative and absolute paths. 
- Understand and apply file and directory operations (`ls`, `cd`, `cp`, `mv`, `mkdir`). 
- Utilize wildcards and special characters (`~`, `*`, `?`, `..`). 
- Use `seqkit` for sequence data statistics.

### Tasks: 

1. **Navigation and Directory Structure** : 
   - Navigate to the `Genomics_Data` directory on your `~/Desktop/shell-lesson-data` using an absolute path. 
   - Return to your home directory using the `~` shortcut. Then navigate back to `Genomics_Data` using a relative path.
   - List all files in the `Genomics_Data/Raw_Data` directory. What type of files are in this directory? **Q1**
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
   - Does the fasta files contain protein or nucleotide sequences? **Q2**
   - Navigate to `Processed_Data/fastq` and use `seqkit stats` to get statistics for all `.fastq` files. Use wildcards to select all `.fastq` files.
   - To write the statistics to a file, use `seqkit stats` with `-o` option: `seqkit stats *.fastq -o fastq_stats.txt`. 
   - What is the average read length for each fastq file?  **Q3**
   

### Homework Submission:
- From konsole menu use `File` -> `Save Output As` to save the output of the commands to a text file. This file contains all the commands and their outputs. You can inspect the file with `gedit` or `nano` to ensure that all the outputs are saved.
- Submit the text file also answer the questions.

- **Q1**:
- **Q2**:
- **Q3**: 

---
- ## Domácí úkol BASH 1
### Cíle:
- Procvičovat navigaci v adresářích pomocí relativních a absolutních cest. 
- Porozumět a aplikovat operace se soubory a adresáři (`ls`, `cd`, `cp`, `mv`, `mkdir`). 
- Využívat zástupné znaky a speciální znaky (`~`, `*`, `?`, `..`). 
- Používat `seqkit` pro analýzu sekvencí.

### Úkoly: 
1. **Navigace a Struktura Adresářů** : 
   - Navigujte do adresáře `Genomics_Data` na vaší `~/Desktop/shell-lesson-data` pomocí absolutní cesty. 
   - Vraťte se do vašeho domovského adresáře pomocí zkratky `~`. Poté se vraťte do `Genomics_Data` pomocí relativní cesty. 
   - Vypište všechny soubory v adresáři `Genomics_Data/Raw_Data`. Jaké typy souborů se v tomto adresáři nacházejí? **Q1** 
   - Vypište všechny soubory končící na `.txt` v adresáři `Genomics_Data/Info` jedním příkazem. 
2. **Používání Zástupných a Speciálních Znaků** : 
   - Vypište všechny `fasta` soubory v `Raw_Data` jedním příkazem a pomocí zástupných znaků. 
   - Vypište všechny `fasta` soubory s názvem začínajícím na `sample` v `Raw_Data` jedním příkazem a pomocí zástupných znaků. 
   - Vypište všechny `fastq` soubory v `Raw_Data` jedním příkazem a pomocí zástupných znaků. 
   - Vytvořte adresář `fastq` v `Processed_Data` a **zkopírujte**  všechny `fastq` soubory z `Raw_Data` do `Processed_Data/fastq` jedním příkazem a pomocí zástupných znaků. 
   - Vytvořte adresář `fasta` v `Processed_Data` a **přesuňte**  všechny `fasta` soubory z `Raw_Data` do `Processed_Data/fasta` jedním příkazem a pomocí zástupných znaků. 
3. **seqkit** : 
   - Navigujte do `Processed_Data/fasta` a použijte `seqkit stats` pro získání statistik pro všechny soubory `.fasta`. Použijte zástupné znaky pro výběr všech souborů `.fasta`. 
   - Pro zápis statistik do souboru použijte `seqkit stats` s možností `-o`: `seqkit 
    stats *.fasta -o fasta_stats.txt`. 
   - Obsahují soubory fasta proteinové nebo nukleotidové sekvence? **Q2** 
   - Navigujte do `Processed_Data/fastq` a použijte `seqkit stats` pro získání statistik pro všechny soubory `.fastq`. Použijte zástupné znaky pro výběr všech souborů `.fastq`. 
   - Pro zápis statistik do souboru použijte `seqkit stats` s možností `-o`: `seqkit stats *.fastq -o fastq_stats.txt`. 
   - Jaká je průměrná délka čtení pro každý soubor fastq? **Q3**

### Odevzdání Domácího Úkolu: 
- Z konzolového menu použijte `File` -> `Save Output As` pro uložení výstupu příkazů do textového souboru. Tento soubor obsahuje všechny příkazy a jejich výstupy. Soubor můžete prohlédnout pomocí `gedit` nebo `nano`, abyste se ujistili, že jsou všechny výstupy uloženy.
- Odevzdejte textový soubor a také odpovězte na otázky. 

- **Q1** : 
- **Q2** : 
- **Q3** :