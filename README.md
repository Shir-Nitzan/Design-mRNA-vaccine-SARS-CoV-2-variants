# :test_tube: Designing an mRNA vaccine against SARS-CoV-2 variants
In this work, we updated the mRNA vaccine based on the BA.2 spike! (assume that the vaccine does not work for the BA.2 variant).


Major findings include:
First Part - analysis between Pfizer and moderna Vaccines:
We found that the coding regions of the vaccines are identical in the protein level.
On the nucleotide level, the coding regions of the vaccines are not identical.

![image](https://user-images.githubusercontent.com/62726511/167273832-0b30c00d-adba-4f09-a937-be0107959cf7.png)
![image](https://user-images.githubusercontent.com/62726511/167273837-9c4359bc-ab6a-48d7-97bf-d19e36906388.png)

Second Part - comparison to the Wuhan strain:
We found that there were only two differences, and they are adjacent:

![image](https://user-images.githubusercontent.com/62726511/167273901-9ffa7609-b1ec-499e-90ae-d9fb71569623.png)

One K in the Wuhan spike region is replaced by a P in the Pfizer spike region, and likewise for a V.

We found up the lookup table that mapping between the Wuhan strain codons to the Pfizer codons - 
maps non-GC codons to GC codons thus increasing the GC content in the vaccine. This will increase the stability of the vaccine while maintaining the same amino-acid structure.
![image](https://user-images.githubusercontent.com/62726511/167274192-22415134-42eb-493d-9752-39a6f60dcabd.png)

Third Part - The variants

BA1-BA2 differences:
There are 21 differences, first difference at index 18
Length of proteins are the same: 1271
BA2 initiation codon is 50 indexes after BA1
Length of mRNA coding regions are both: 3813


We found that the KV being replaced by PP in the vaccine results in a stabilized spike protein in the eprefusion state and contributes to the efficiency of the vaccine. It is thought that the KV is probably not functionally important. Source: [article](https://pubmed.ncbi.nlm.nih.gov/33466921/).
Designing our BA2 vaccine included looking for all the places with substitutions and change the codons by the Pfizer lookup table (from last part).




## Use case 📲
1. Run the python server from app.py start point.
2. Enter localhost:
```bash
http://127.0.0.1:8080/
```
3. Follow the demo:

![HackatonIDC2021](https://user-images.githubusercontent.com/62726511/120941407-4cbe6780-c72b-11eb-9158-a4371a007288.gif)

4. Once you upload images of driver license, car license and car policy, the app will automatically fill all of the forms details 📝.

