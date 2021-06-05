# Biomarker Extraction - NLP

Authors: Junxia Lin, Yuezheng He, Chul Kim, Siminar Boca

This repository contains custom modules and a program used to extract biomarkers of FDA-approved target therapies listed on [NIH National Cancer Institue (NCI)](https://www.cancer.gov/about-cancer/treatment/types/targeted-therapies/targeted-therapies-fact-sheet) from their NCI webpage and DailyMed webpage(s). 

A variaty of biomarkers can be extracted, including target therapies' name, disease name, drug brand name, gene, protein, and medication. These biomarker detection and extraction tasks are performed based on the named-entity recognition (NER) pre-training models from [scispacy](https://github.com/allenai/scispacy). In addition, the package includes functions to detect negation from sentences by using two pre-trained negation models obtained from Aditya Khandelwal & Suraj Sawant's [NegBERT](https://github.com/adityak6798/Transformers-For-Negation-and-Speculation) program. The negation tasks include negation cue detection and negation scope extraction from sentence. The package also provides function to detect a few other indications between the drug and disease, such as first-line treatment, accerelated approval, metastatics. 
