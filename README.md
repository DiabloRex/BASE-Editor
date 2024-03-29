# BASE-Editor Local version

## Requirements

Microsoft .Net FrameWork

All requirements of cas-offinder. http://www.rgenome.net/cas-offinder/portable

## Preparations and instructions

1. Download all the files and folder structures in the repository
2. Download genome files from NCBI website, including genome sequence FASTA files and annotation GTF files. Decompress all the files. For mouse, view https://www.ncbi.nlm.nih.gov/data-hub/genome/GCF_000001635.27/ and download desire assembly and GFF file.
3. Install dependencies. Scoring sgRNA is performed by looking all the off-target sites, which is excuted by CasOFFinder. So, you have to install its dependencies. Goto http://www.rgenome.net/cas-offinder/portable and install OpenCL as instructed in STEP1.
4. open the program BaseEdit.exe.
5. Add genome. Goto TAB<Genome Editor>, at create new genome section, input genome name, select genome FASTA files (single file or FASTA folder) and the GFF file downloaded previously, then press the Create New Genome button.
6. (optional) Add plasmid. Goto TAB<Plasmid Editor>, click "New ..." to add new plasmid info, each box is restrict enzyme cleavage site. This is mainly for linking the sgRNAs to target plasmid.
7. (optional) Add Editting mode. Two mode are provided already. If you want to use a new mode, you have to create it first. Click "New ..." to add new mode info, all the settings are pretty intuiative.
8. For single gene. Goto TAB<Single Query>, input your query, both NCBI RefseqID and gene name are supported. Choose the editting mode, target plasmid, target Genome, result folder, number of mismatches for off-target searching and run searching on CPU or GPU (if you have one). Then hit the Query button and wait, this may take a lot of time depending on your computer.
9. For multiple genes. Goto TAB<Multiple Query>, input your queries, both NCBI RefseqID and gene name are supported, but only one type at a time. Like single gene query, choose the editting mode, target plasmid, target Genome, result folder, number of mismatches for off-target searching and run searching on CPU or GPU (if you have one). Then hit the Query Multiple button and wait, this may take a lot of time depending on your computer.
10. Results. In single gene mode, resulting text is displayed at the textbox below. In both single and multiple mode, result can be opened using the Open button. This will open the result folder, which contains the resulting text and a simple graphic representation of the target gene and sgRNA locations.

## Problems

If you find yourself hard to make the program work, please feel free to contact us. We will reply as soon as possible, and update the program to improve user experiences. Thank you!

E-mail: yanmeng@sibs.ac.cn

## Citation

Please cite us: Li Q#, Lu J#, Yin X#, Chang Y#, Wang C#, Yan M#, Feng L, Cheng Y, Gao Y, Xu B, Zhang Y, Wang Y, Cui G, Xu L, Sun Y, Zeng R, Li Y, Jing N, Xu GL*, Wu L*, Tang F* & Li J*. Base editing-mediated one-step inactivation of the Dnmt gene family reveals critical roles of DNA methylation during mouse gastrulation. Nat Commun 2023, 14(1): 2922. https://doi.org/10.1038/s41467-023-38528-z

