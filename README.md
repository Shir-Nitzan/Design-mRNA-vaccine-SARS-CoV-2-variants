# :test_tube: Designing an mRNA vaccine against SARS-CoV-2 variants
In this work, we updated the mRNA vaccine based on the BA.2 spike! (assume that the vaccine does not work for the BA.2 variant).

The following findings focused on each part:

# First Part - analysis between Pfizer and moderna Vaccines
We found that the coding regions of the vaccines are identical in the protein level.
On the nucleotide level, the coding regions of the vaccines are not identical.

<img src="https://user-images.githubusercontent.com/62726511/167273832-0b30c00d-adba-4f09-a937-be0107959cf7.png" width="500" >
<img src="https://user-images.githubusercontent.com/62726511/167273837-9c4359bc-ab6a-48d7-97bf-d19e36906388.png" width="500" >


# Second Part - comparison to the Wuhan strain
We found that there were only two differences, and they are adjacent:

![image](https://user-images.githubusercontent.com/62726511/167273901-9ffa7609-b1ec-499e-90ae-d9fb71569623.png)

One K in the Wuhan spike region is replaced by a P in the Pfizer spike region, and likewise for a V.

We found up the lookup table that mapping between the Wuhan strain codons to the Pfizer codons - 
maps non-GC codons to GC codons thus increasing the GC content in the vaccine. This will increase the stability of the vaccine while maintaining the same amino-acid structure.


# Third Part - The variants

BA1-BA2 differences:
There are 21 differences, first difference at index 18
Length of proteins are the same: 1271
BA2 initiation codon is 50 indexes after BA1
Length of mRNA coding regions are both: 3813


We found that the KV being replaced by PP in the vaccine results in a stabilized spike protein in the eprefusion state and contributes to the efficiency of the vaccine. It is thought that the KV is probably not functionally important. Source: [article](https://pubmed.ncbi.nlm.nih.gov/33466921/).
Designing our BA2 vaccine included looking for all the places with substitutions and change the codons by the Pfizer lookup table (from last part).




## Findings Presentation Demo 📝



![www-screencapture-com-2022-5-8-00-09_wQJ2l7jx](https://user-images.githubusercontent.com/62726511/167274240-ff753f11-2bae-4429-90da-dcfa3e9fcafd.gif)



