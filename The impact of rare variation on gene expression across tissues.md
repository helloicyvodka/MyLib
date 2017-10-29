# The impact of rare variation on gene expression across tissues


# Introduction


## Problem  
rare variants  —>  phenotypic effects ???

rare non-coding variants ~ extreme gene expression  

* single tissues   —> ORIGIN
* multiple tissues  —> **GTEx**

## Overall Conclusion 
* rare variants contribute to large gene expression changes across tissues 
* provide an integrative method for interpretation of rare variants in individual genomes ：RIVER


# Methods

## Outliers

* single-tissue expression outliers 
* multi-tissue expression outliers  




## Genetic Variants Identification

* common genetic variants   
genetic association studies + +
* rare genetic variants
	* protein-coding alleles + +
	* non-coding variants  - -




## Genotype- Tissue Expression (GTEx) 
* v6p
* across 44 human tissues
* combined analyses of: 
	* **whole genomes** 
	*  **multi-tissue RNA-sequencing data**  






## RIVER (RNA-informed variant effect on regulation)  
* a Bayesian statistical model  
* incorporates expression data to predict a regulatory effect for rare variants
* higher accuracy than models using genomic annotations alone

## PEER (probabilistic estimation of expression residuals)
removed hidden factors estimated by PEER (probabilistic estimation of expression residuals)13 from each tissue before outlier discovery  
**(Extended Data Figs 1, 2 and Supplementary Tables 1, 2)**

  
    
      
       
       

# Results 


## Figure 1: Gene expression outliers and sharing between tissues.

![fig.1](https://www.nature.com/nature/journal/v550/n7675/images/nature24267-f1.jpg)
  
 
### Fig. 1a

gene expression outliers (表达量异常值）

* 58% of underexpression 
* 28% of overexpression outliers    

have nearby conserved rare variants（compared to 8% of non-outliers） 



 
We identified  

* a single-tissue expression outlier for ≥99% of expressed genes in each tissue 
* a multi-tissue outlier for 4,919 out of 18,380 genes that were tested (27%)
* a single- tissue outlier for a median of 83 genes per tissue
* a multi-tissue outlier for a median of 10 genes

### Fig. 1b

**repilication rate**  

* Single-tissue outliers that were found in one tissue replicated in other tissues at rates of up to 33%, with higher rates among related tissues

### Fig. 1c
Estimated replication rate of multi-tissue outliers in a constant held-out set of tissues for different sets of discovery tissues.

* replication rate for multi-tissue outliers was much higher (outlier >> random)
* replication rate increased with the number of tissues used for discovery 


## Figure 2: Enrichment of rare variants and ASE in outliers
![fig.2](https://www.nature.com/nature/journal/v550/n7675/images/nature24267-f2.jpg)

**the influence of rare genetic variation on extreme expression levels**  

### Fig. 2a

* Multi- tissue outliers were strongly enriched for nearby rare variants. 
* short insertions and deletions (indels) > single-nucleotide variants (SNVs) 
	* Because most rare variants occur as heterozygotes, expression outliers driven by rare variants in cis should exhibit allele-specific expression (ASE). Both single-tissue and multi-tissue outliers were significantly enriched for ASE compared to non-outliers  


* For underexpression outliers with exonic rare variants, the rare allele was generally underexpressed with respect to the common allele and conversely so for overexpression outliers, consistent with the rare variant causing the effect 
* The enrichment for rare variants and ASE was stronger for multi-tissue outliers than for single-tissue outliers (Fig. 2b, c and Extended Data Fig. 6a), especially at higher Z-score thresholds.

### Fig. 2b

* The enrichment for rare variants and ASE was stronger for multi-tissue outliers than for single-tissue outliers,especially at higher Z-score thresholds.(Fig. 2b, c and Extended Data Fig. 6a)


### Fig. 2c

* Both single-tissue and multi-tissue outliers were significantly enriched for ASE compared to non-outliers (see Methods; two-sided Wilcoxon rank-sum tests, each nominal P < 2.2 × 10−16; Fig. 2c)


## Figure 3 | Stratification of multi-tissue outliers by rare variant classes

rare variants ~ large changes in gene expression

### Fig. 3a
Outliers were enriched, in order of significance, for structural variants, variants near splice sites, introducing frameshifts, at start or stop codons, near the transcription start site and in conserved regions

### Fig. 3b
relationship between outlier gene expression and functional annotations. 

* Multi-tissue outliers were strongly enriched for variants in **promoter or CpG-rich regions** and had variants with higher conservation and CADD (combined annotation-dependent depletion) scores than non-outliers. We observed weaker enrichment in **enhancers and transcription- factor-binding sites**.
 
### Fig. 3c
Combining all classes of variation, other than non-conserved, non-coding, rare variants (excluded as less likely candidates for causal effects),we observed that 

* 58% of underexpression and 28% of overexpression outliers had rare variants near the relevant gene, compared to 8% for non-outliers.

### (Extended Data Fig. 5b)
Overexpression outliers were more common overall, potentially because detection of underexpression outliers for very low expression genes is inherently limited 
### (Extended Data Fig. 5c)
Overexpression outliers were also less enriched for functionally annotated rare variants 
### Fig. 3d
Some variant classes had strong directionality concordant with their expected impact: duplications caused overexpression, whereas dele- tions, start- and stop-codon variants and frameshifts coincided with underexpression
### Fig. 3e
We also observed strong ASE for outliers carrying all classes of variants, except non-conserved variants 

## Figure 4 | Evolutionary constraint of genes with multi-tissue outliers.
We hypothesized that functional, large-effect rare variants have been under recent selective pressure.

### Fig. 4a
As expected, we found that rare promoter variants of outliers were significantly less frequent in the UK10K cohort of 3,781 individuals than rare promoter variants of non-outliers for the same genes.

### Fig. 4b
Additionally, genes intolerant to loss-of-function and missense mutations were depleted of both multi-tissue outliers and multi-tissue **expression quantitative trait loci** (eQTLs; Fisher’s exact test, all P < 2 × 10−15; Fig. 4b and Extended Data Fig. 8a)

### Fig.4c
We observed a similar depletion in two curated disease gene lists—genes involved in heritable cardiovascular disease and genes in the guidelines of the American College of Medical Genetics and Genomics for incidental findings20—but not in broader gene lists (Fig. 4c and Extended Data Fig. 8b, c)

### (Extended Data Fig. 8d, e)




Variants in coding regions contributed disproportionately to outlier expression; enrichments weakened for all variants types (SNVs, indels and structural variants) when excluding exonic regions (Extended Data Fig. 6b)