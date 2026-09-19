
# From Gene Mutation to Disease: Investigating How DNA Sequence Changes Affect Protein Products and Human Phenotypes

## Disease Background

Classic galactosemia is an inherited metabolic disorder caused by deficient activity of galactose-1-phosphate uridylyltransferase (GALT), an enzyme required for normal galactose metabolism. Reduced GALT activity disrupts galactose processing and causes the accumulation of galactose and related metabolites. Affected newborns may develop poor feeding, vomiting, diarrhea, failure to thrive, jaundice, cataracts, and an increased risk of *Escherichia coli* sepsis. Long-term complications may include developmental delay, speech difficulties, neurological abnormalities, and reproductive problems.

Classic galactosemia is caused by pathogenic variants in the **GALT** gene and follows an autosomal recessive inheritance pattern. The documented variant investigated in this study is **GALT c.563A>G (p.Gln188Arg; Q188R)**, a missense variant associated with classic galactosemia.

## Gene and Normal Protein Function

The **GALT** gene is located on chromosome 9p13.3 and encodes galactose-1-phosphate uridylyltransferase. The enzyme functions in the cytosol as part of the **Leloir pathway**, which is responsible for galactose metabolism.

GALT catalyzes the transfer of a uridylyl group from UDP-glucose to galactose-1-phosphate, producing UDP-galactose and glucose-1-phosphate. Normal GALT activity allows galactose-derived metabolites to enter normal carbohydrate metabolism and prevents harmful metabolite accumulation.

## Documented Mutation

| Parameter | Information |
|---|---|
| Gene | GALT (galactose-1-phosphate uridylyltransferase) |
| Reference Transcript | NM_000155.4 |
| Exact Variant | NM_000155.4:c.563A>G (p.Gln188Arg) |
| Nucleotide Change | A → G at position 563 |
| Predicted Protein Change | p.Gln188Arg (Q188R) |
| Mutation Type | Missense variant / single-nucleotide substitution |
| ClinVar Accession | VCV000003614.140 |
| Clinical Interpretation | Pathogenic |
| Reference | Fridovich-Keil et al. (1995); Elsevier & Fridovich-Keil (1996) |

## Hypothesis

The **GALT c.563A>G** mutation is predicted to produce a missense substitution in which glutamine (Q) is replaced by arginine (R) at amino acid position 188. Because only one nucleotide is substituted, the reading frame and protein length are expected to remain unchanged. The amino-acid substitution may alter GALT structure or enzymatic function and consequently impair normal galactose metabolism.

## Methods

**1.** **Sequence Retrieval:** The human GALT wild-type coding sequence was obtained using reference transcript **NM_000155.4**.

**2.** **Control Translation:** The wild-type CDS was translated using the Galaxy translation tool in **Frame 1** to obtain the predicted GALT protein sequence.

**3.** **Documented Mutation Engineering:** The nucleotide at position 563 was changed from **A to G** to reproduce the documented **c.563A>G** variant.

**4.** **Mutant Translation:** The modified CDS was translated using the same procedure as the wild-type sequence. The resulting protein was compared with the wild-type sequence to identify amino-acid changes, protein-length changes, and premature stop codons.

**5.** **Artificial Mutation:** A second single-nucleotide substitution was created at position 564, changing the codon from **AGG to AAG**. This was predicted to change arginine (R) to lysine (K).

**6.** **Sequence Alignment:** Needle was used to compare the wild-type and mutant GALT protein sequences and determine sequence identity, similarity, gaps, and amino-acid differences.

**7.** **Workflow Management:** Sequence processing, mutation construction, translation, and alignment were performed using Galaxy (https://usegalaxy.org/u/ella_cadungog/h/cadungog-classicgalactosemia-galt-q188r-lab) and documented through GitHub.

# Results

## Wild-Type Control Parameters

| Parameter | Result |
|---|---|
| CDS Length | 1,140 bp |
| Predicted Protein Length | 379 aa |
| Start Codon | ATG |
| Stop Codon | * |
| Reading Frame | Frame 1 |
| First 10 Amino Acids | MSRSGTDPQQ |
| Last 10 Amino Acids | LPEVHYHLGQ |

## Documented Mutation Results

| Parameter | Result |
|---|---|
| Mutation | c.563A>G |
| Original Nucleotide | A |
| Mutant Nucleotide | G |
| Bases Affected | 1 |
| Bases Inserted | 0 |
| Bases Deleted | 0 |
| Bases Substituted | 1 |
| Mutation Type | Missense |
| Mutant CDS Length | 1,140 bp |
| Predicted Protein Length | 379 aa |
| Reading Frame | Frame 1 |
| Amino Acid Change | Q188R |
| Premature Stop Codon | Absent |

## WT versus Mutant Protein Comparison

The wild-type GALT protein contains 379 amino acids. The documented **c.563A>G** mutation produces a single amino-acid substitution at position 188, changing glutamine (Q) to arginine (R), or **p.Gln188Arg (Q188R)**. The reading frame and predicted protein length remain unchanged, with no amino-acid insertions, deletions, or premature stop codons.

## Mutation Comparison Matrix

| Parameter | Wild-Type | Documented Mutation (c.563A>G) | Artificial Mutation (c.564G>A) |
|---|---|---|---|
| CDS Length | 1,140 bp | 1,140 bp | 1,140 bp |
| Protein Length | 379 aa | 379 aa | 379 aa |
| Mutation Type | None | Missense | Missense |
| Reading Frame Change | No | No | No |
| Premature Stop Codon | Absent | Absent | Absent |
| Amino Acid Affected | None | Q188R | R188K |
| Expected Consequence | Normal GALT function | May alter GALT structure/function | May alter local GALT properties; requires validation |

## Artificial Mutation Experiment

The artificial mutation was created at nucleotide position 564 by changing the wild-type codon **AGG** to **AAG**. AGG encodes arginine (R), whereas AAG encodes lysine (K). Therefore, the predicted result is a missense substitution **R188K**. Because no nucleotide was inserted or deleted, the reading frame and predicted protein length remain unchanged.

## Alignment Results

Needle alignment of the GALT protein sequences showed **379/380 identical positions (99.7% identity)** and **380/380 similar positions (100% similarity)**. No gaps were detected. The alignment identified the amino-acid substitution at position 188, consistent with **Q188R**.

| Parameter | Needle Alignment Result |
|---|---:|
| Alignment Length | 380 aa |
| Identity | 379/380 (99.7%) |
| Similarity | 380/380 (100%) |
| Gaps | 0/380 (0%) |
| Amino Acid Difference | Q188R |
| Frameshift | None |
| Premature Stop Codon | None |

## Molecular Interpretation

**Gene → Mutation → Protein → Cellular Effect → Phenotype**

The **GALT** gene encodes galactose-1-phosphate uridylyltransferase, an enzyme required for galactose metabolism. The documented **c.563A>G** substitution changes one nucleotide and produces the **Q188R** amino-acid substitution. The computational results show that the mutation does not alter the reading frame or predicted protein length but changes one amino acid at position 188. This substitution may alter GALT structure or enzymatic activity, potentially reducing normal galactose metabolism. Impaired GALT activity can lead to accumulation of galactose-related metabolites and contribute to the clinical manifestations of classic galactosemia.

## Limitations

The analysis was based on computational sequence translation and alignment. These methods can identify nucleotide and predicted amino-acid changes but cannot directly demonstrate protein expression, folding, stability, enzyme activity, or cellular effects. The functional consequence of the artificial **R188K** mutation therefore remains a prediction and requires experimental validation.

## Conclusion

The analysis demonstrated that the documented **GALT c.563A>G** variant is a missense mutation producing the **Q188R** amino-acid substitution. The mutation preserves the reading frame and predicted protein length while changing one amino acid at position 188. The artificial **c.564G>A** mutation similarly produces a missense substitution, **R188K**, without altering protein length or reading frame. These results demonstrate how single-nucleotide substitutions can produce localized changes in protein sequence while potentially affecting protein function.

### References

Berry, G. T. (2021). Classic galactosemia and clinical variant galactosemia. In M. P. Adam, S. Bick, G. M. Mirzaa, et al. (Eds.), *GeneReviews®*. University of Washington, Seattle. https://www.ncbi.nlm.nih.gov/books/NBK1518/

National Center for Biotechnology Information. (n.d.). *Galactosemia (Concept ID: C0016952).* NCBI MedGen. https://www.ncbi.nlm.nih.gov/medgen/C0016952

National Library of Medicine. (n.d.). *GALT gene: Galactose-1-phosphate uridylyltransferase.* MedlinePlus Genetics. https://medlineplus.gov/genetics/gene/galt/

National Center for Biotechnology Information. (n.d.). *NM_000155.3(GALT):c.563A>G (p.Gln188Arg) and deficiency of UDPglucose-hexose-1-phosphate uridylyltransferase.* ClinVar. https://www.ncbi.nlm.nih.gov/clinvar/RCV000003798.6/

Coelho, A. I., Trabuco, M., Ramos, R., Silva, M. J., Tavares de Almeida, I., Leandro, P., Rivera, I., & Vicente, J. B. (2014). Functional and structural impact of the most prevalent missense mutations in classic galactosemia. *Molecular Genetics and Genomic Medicine, 2*(6), 484–496. https://doi.org/10.1002/mgg3.94
