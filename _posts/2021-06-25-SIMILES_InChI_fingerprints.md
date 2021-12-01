---
title: 'CAS, SMILES, InChl and Fingerprints'
date: 2021-06-25
permalink: /posts/2021/06/SMILES/
tags:
  - drug
  - SMILES
  - InChl
  - Fingerprints
  - chemoinformatics
---

# An introduction to CAS, SMILES, InChl and Fingerprints of drugs or chemicals

CAS: 

* unique numerical identifier assigned by the Chemical Abstracts Service (CAS) to every chemical substance.
* Example: caffeine: 58-08-2

SMILES strings:

* Simplified Molecular Input Line Entry System.
* using short ASCII strings.
* it is very common that there are a lot of SMILES strings that represent the same structure.
* unique SMILES string is also called the “canonical SMILES”.
* Example: CN1C=NC2=C1C(=O)N(C(=O)N2C)C

InChI identifiers:

* IUPAC Chemical Identifier 
* a unique textual label for any chemical substance.
* comprise different layers and sub‐layers of information separated by slashes (/).
* example: caffeine: InChl=1S/C8H10N4O2/c1–10–4–9–6–5(10)7(13)12(3)8(14)11(6)2/h4H,1–3H3
![img](https://chem.libretexts.org/@api/deki/files/202932/InChI%252BLayers.JPG?revision=1)

InChI Keys

* a hashed version of the InChI
![img](https://chem.libretexts.org/@api/deki/files/202988/InChI_Key.PNG?revision=1&size=bestfit&width=725&height=88)
* The hash function is a one-way conversion
![img](https://chem.libretexts.org/@api/deki/files/204060/InChIKeyconversion.JPG?revision=1&size=bestfit&width=740&height=150)

hashed fingerprints: 

* use fixed-length binary values (0/1 bits) to encode molecular features, used to evaluation the similarity or diversity of chemicals.
* one molecule -> one fingerprint; but different molecules may have the same fingerprint.
* cannot confirm the presence of a substructure in a molecule, but confirm the absence of a substructure.
* the structure of a chemical cannot be induced from the fingerprint.

References:

* https://webbook.nist.gov/chemistry/cas-ser/
* https://pubchem.ncbi.nlm.nih.gov/compound/2519
* [Sousa, J. (2017). Processing of SMILES, InChI, and Hashed Fingerprints.](https://onlinelibrary.wiley.com/doi/10.1002/9781119161110.ch4)
* [Line Notation (SMILES and InChI)](https://chem.libretexts.org/Courses/Fordham_University/Chem1102%3A_Drug_Discovery_-_From_the_Laboratory_to_the_Clinic/05%3A_Organic_Molecules/5.08%3A_Line_Notation_(SMILES_and_InChI))

Updated: 1st Dec. 2021