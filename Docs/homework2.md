
## Homework BASH 2
#### Objective

Learn how to download genomic data from NCBI, navigate through the dataset, and perform basic exploration of downloaded data sets using command-line tools.

### Steps 
1. **Finding the Genome Assembly on NCBI**  
   - Go to the NCBI database at [https://www.ncbi.nlm.nih.gov]() .
   - Find the assembly for *Genlisea aurea*. *Genlisea aurea* is a carnivorous plant species with a small genome size.
2. **Obtaining the Download Link** 
   - On the assembly summary page, locate the "curl" link and obtain URL for downloading the genome.
3. **wget** 
   - Open your terminal.
   - Create directory `Genlisea_aurea` in your `~/Desktop` directory. 
   - Navigate to the `Genlisea_aurea` directory.
   - Use the `wget` command followed by the copied URL link to download the genome. 
   - Example: `wget -O genome.zip [URL]` (option `-O` is used to specify the name of the downloaded file.
4. **Unzipping the Downloaded File**  
   - Downloaded file is `.zip` archive, use the `unzip` command to extract its contents. 
   - Example: `unzip genome.zip` 
   - After extraction, use `ls` to view the new directory, which will often be named `ncbi_dataset`. 
5. **Exploring the Extracted Data**  
   - Navigate into the `ncbi_dataset` directory: `cd ncbi_dataset` 
   - Use `ls -l -R` to recursively list the contents of the directory and subdirectories. 
6. **seqkit**  
   - Navigate to the directory containing the `.fna` and `.faa` files (`cd data/GCA_000441915.1`). 
   - Run `seqkit stat` on the `.fna` and `.faa` files to get statistics about the sequences.
   - What is the length of the shortest contig in genome assembly? **Q1**
   - Very short contigs in genome assembly are usually not to useful for downstream analysis. How many contigs are shorter than 1000 bp? **Q2**
   - HINT: you can use `seqkit set -m 1000` to filter contigs longer than 1000 bp or `seqkit grep -M 1000` to filter contigs shorter than 1000 bp.
   - Explore the `genomic.gff` file using commands like `head`, `less -S` to view content of the fil.
   - What does the `.gff` file contain? **Q3**
 
7. Homework Submission:
   - From konsole menu use `File` -> `Save Output As` to save the output of the commands to a text file. This file contains all the commands and their outputs. You can inspect the file with `gedit` or `nano` to ensure that all the outputs are saved.
   - Submit the text file also answer the questions.

- **Q1**:
- **Q2**:
- **Q3**: 

---
- ## Domácí úkol BASH 2
#### Cíl

Naučte se, jak stahovat genomová data z NCBI, procházet datovou sadu a prozkoumat ztažené data pomocí nástrojů příkazového řádku.
### Kroky 
1. **Hledání assembly genomu na NCBI**  
   - Přejděte do databáze NCBI na adrese [https://www.ncbi.nlm.nih.gov] . 
   - Najděte assembly pro *Genlisea aurea*. *Genlisea aurea* je druh masožravé rostliny s malou velikostí genomu. 
2. **Získání odkazu ke stažení** 
   - Na stránce se genomové assembly najděte odkaz "curl" a získejte URL pro stahování genomu. 
3. **wget** 
   - Otevřete terminál. 
   - Vytvořte adresář `Genlisea_aurea` ve vaší složce `~/Desktop`. 
   - Přejděte do adresáře `Genlisea_aurea`. 
   - Použijte příkaz `wget` následovaný zkopírovaným URL odkazem ke stažení genomu. 
   - Příklad: `wget -O genome.zip [URL]` (volba `-O` se používá k určení názvu staženého souboru). 
4. **Rozbalení staženého souboru**  
   - Stažený soubor je archiv `.zip`, použijte příkaz `unzip` k extrahování jeho obsahu. 
   - Příklad: `unzip genome.zip` 
   - Po extrakci použijte `ls`, abyste zobrazili nový adresář, který bude často pojmenován `ncbi_dataset`. 
5. **Prozkoumání extrahovaných dat**  
   - Přejděte do adresáře `ncbi_dataset`: `cd ncbi_dataset` 
   - Použijte `ls -l -R` k rekurzivnímu výpisu obsahu adresáře a podadresářů. 
6. **seqkit**  
   - Přejděte do adresáře obsahujícího soubory `.fna` a `.faa` (`cd data/GCA_000441915.1`). 
   - Spusťte `seqkit stat` na souborech `.fna` a `.faa` pro získání statistik o sekvencích. 
   - Jaká je délka nejkratšího kontigu v genomové assembly? **Q1** 
   - Velmi krátké kontigy v genomové assembly obvykle nejsou příliš užitečné pro další analýzu. Kolik kontigů je kratších než 1000 bp? **Q2** 
   - NÁPOVĚDA: můžete použít `seqkit set -m 1000` k filtrování kontigů delších než 1000 bp nebo `seqkit grep -M 1000` k filtrování kontigů kratších než 1000 bp. 
   - Prozkoumejte soubor `genomic.gff` pomocí příkazů jako `head`, `less -S` pro zobrazení obsahu souboru. 
   - Co soubor `.gff` obsahuje? **Q3** 
7. Odevzdání domácího úkolu: 
   - Z nabídky konzole použijte `File` -> `Save Output As` pro uložení výstupu příkazů do textového souboru. Tento soubor obsahuje všechny příkazy a jejich výstupy. Soubor můžete prozkoumat pomocí `gedit` nebo `nano`, abyste se ujistili, že jsou všechny výstupy uloženy.
   - Odevzdejte textový soubor a také odpovězte na otázky. 


- **Q1** : 
- **Q2** : 
- **Q3** :