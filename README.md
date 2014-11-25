##An Ebola virus (EBOV) phylogeny annotated with branch-defining mutations##

![2014image](https://github.com/gmagoon/ebolaWestAfrica2014/blob/master/ZEBOV_2014_outbreak_mutations.png)

###Summary###
This is a maximum parsimony tree based on 101 Ebola virus (EBOV or *Zaire ebolavirus*) sequences, including recent sequences from the 2014 West Africa outbreak as published in Baize *et al.* (2014) and Gire *et al.* (2014). The tree is constructed using an iterative reweighting process, as described in Magoon *et al.* (2013), that downweights unstable sites; the approach allows generation of robust trees with explicit branch support, such that individual mutations can be localized to branches of the tree; in this case, the approach also provides insight into conserved genetic regions and stability of individual loci on the Zaire ebolavirus genome. PHYLIP 3.69 (with minor modifications for memory management) is used to provide the maximum parsimony tree generation algorithm and ancestral state reconstruction (Felsenstein 2009). The MAFFT multi-sequence alignment from Gire *et al.* is used here.

Note: The first sample, from the 1976 outbreak, was specified as outgroup for this tree; the chosen sample is somewhat arbitrary and the the rooting arrangement around the samples from 1976 outbreak will not be correct, but the phylogeny for more recent outbreaks, including the 2014 West African outbreak, should be accurate.

###Description of files###
* `ZEBOV_2014_outbreak_mutations.png`: a phylogram depicting branch-defining mutations with a focus on the 2014 West African outbreak subclade; internal branches have been manually annotated with the mutations information from `treeMutationAnnotations.txt` 
* `ZEBOV_mutationcount.png`: per-locus mutation counts in the generated tree (generated from data in `ZEBOV_mutationCounts.tab`); regions without variants (e.g. conserved regions) appear as white bands at the bottom
* `ZEBOV_variantdensity.png`: variant density based on a ~200 bp sliding window
* `treeMutationAnnotations.txt`: a list of mutations associated with each branch of the generated tree; it may be helpful to cross-reference with `asciitree.txt` for node numbers; asterisks indicate that the location of the mutation in the tree is somewhat uncertain and could be located on an upstream branch
* `ZEBOV_mutationcount.tab`: table containing the number of mutations per locus in the generated tree (tab-delimited)
* `asciitree.txt`: text-format tree extracted from PHYLIP output
* `outfile`: PHYLIP output for (final) tree
* `outtree`: Newick format tree from PHYLIP
* `weights`: locus weighting factors used to generate (final) tree (PHYLIP-format)

Note: Locus numbering is based on the multiple sequence alignment from Gire *et al.* (specifically, `ebov.pruned.phy` from the Supporting Information, S1)

Please contact me at ```gmagoon at aerodyne dot com``` with questions and feedback.

###References###

Baize, S., Pannetier, D., Oestereich, L., Rieger, T., Koivogui, L., Magassouba, N. F., ... & Günther, S. (2014). Emergence of Zaire Ebola virus disease in Guinea—preliminary report. New England Journal of Medicine.

Felsenstein, J., PHYLIP (Phylogeny Inference Package) version 3.69. Distributed by the author. Department of Genome Sciences, University of Washington, Seattle. 2009. 

Gire, S. K., Goba, A., Andersen, K. G., Sealfon, R. S., Park, D. J., Kanneh, L., ... & Scheiffelin, J. S. (2014). Genomic surveillance elucidates Ebola virus origin and transmission during the 2014 outbreak. Science, 345(6202), 1369-1372.

Magoon, G. R., Banks, R. H., Rottensteiner, C., Schrack, B. E., Tilroe, V. O., Grierson, A. J. (2013, under review) Generation of high-resolution *a priori* Y-chromosome phylogenies using “next-generation” sequencing data. bioRxiv doi: http://dx.doi.org/10.1101/000802

