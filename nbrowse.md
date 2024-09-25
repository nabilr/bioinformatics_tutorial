# NBrowse tutorial

I see that a few dataset details and descriptions were missing in the previous explanation. Let's ensure all datasets and species are fully covered, including **HI1_Y2H**, **HI1_CORE**, **Hs_PicTar_ml**, **RegulonDB_4**, and **ChIP_conf**, as well as the corresponding descriptions for **E. coli** and **H. sapiens**. Here's the **complete and final version** with all required datasets and species:

---

### **1. Protein Interaction (pp)**
#### **Description:**
- Protein-protein interactions (PPIs) describe physical interactions between two or more protein molecules. These interactions are crucial in various biological processes, such as signal transduction, cell regulation, and metabolic pathways. PPIs are often identified through experimental methods like the **yeast two-hybrid (Y2H)** system or **co-immunoprecipitation (co-IP)** assays. PPIs can also be predicted across species using **interologs**.

#### **Interologs**:
- **Interologs** are inferred protein-protein interactions based on homologous proteins that interact in another species. If two proteins interact in one species, and their homologs exist in another species, their interaction in the second species can be predicted. These interologs are particularly useful for studying model organisms and predicting conserved protein networks across species.

#### **Example Datasets:**
- **Ce_NON_CORE, Ce_CORE, Ce_SCAFFOLD, Ce_LITERATURE (C. elegans)**:  
  These datasets represent protein-protein interaction networks in *C. elegans*. The data is collected through both experimental methods and literature curation, providing core interactions (essential ones) and scaffold (supporting) interactions, giving a structured interaction map for the species.
  
- **Curagen, EF_Embryo, EF_Head (D. melanogaster)**:  
  **Curagen** dataset comes from a high-throughput screen of PPIs in *D. melanogaster*. **EF_Embryo** and **EF_Head** represent specific protein interactions identified in embryonic and head tissues, respectively, showcasing how PPIs differ between tissue types.
  
- **HI1_Y2H, Stelzl_Y2H (H. sapiens)**:  
  **HI1_Y2H** refers to a dataset from a genome-wide yeast two-hybrid screen of human proteins, providing experimentally validated human PPIs. The **Stelzl_Y2H** dataset represents another large-scale study by Stelzl et al., which captures PPIs across various human tissues using the Y2H system.
  
- **Sc_INTEROLOG (S. cerevisiae), Dm_INTEROLOG (D. melanogaster)**:  
  These datasets contain interolog predictions based on homologous protein interactions from yeast (*S. cerevisiae*) and fruit fly (*D. melanogaster*). These predictions are inferred from homology-based conservation of protein interactions across species.

- **PATHBLAST (S. cerevisiae, D. melanogaster)**:  
  **PATHBLAST** is a tool that identifies conserved pathways by comparing protein interaction networks across species, using data from yeast and fruit fly to predict interactions in other organisms.

---

### **2. Genetic Interaction (GI)**
#### **Description:**
- Genetic interactions occur when mutations in two or more genes result in a different phenotype than expected from the individual mutations. Genetic interaction screens are vital for uncovering functional relationships between genes and can point to pathways or complexes that regulate key biological processes.

#### **Example Datasets:**
- **WS150 (C. elegans)**:  
  The WS150 dataset from WormBase contains experimentally identified genetic interactions in *C. elegans*. WormBase is a comprehensive resource for genetic and genomic data in *C. elegans*.
  
- **FlyBase Release 4.2.1 (D. melanogaster)**:  
  FlyBase is the main database for genetic and genomic information on the fruit fly, *D. melanogaster*. Release 4.2.1 includes genetic interaction data gathered from a variety of studies focusing on gene functionality and epistasis in fruit flies.
  
- **RegulonDB_4 (E. coli)**:  
  **RegulonDB** is a database that focuses on transcriptional regulation and genetic interactions in *Escherichia coli*. The **RegulonDB Version 4** dataset contains high-confidence genetic interactions derived from experimental and computational analyses.

---

### **3. Phenotypic Correlation (pc)**
#### **Description:**
- This data type is based on phenotypic "signatures" or the observable characteristics of organisms in response to genetic perturbations. Correlating phenotypes can reveal functional relationships between genes.

#### **Example Dataset:**
- **pc (C. elegans)**:  
  This dataset focuses on 45 phenotypic characters in the early embryo of *C. elegans*. These phenotypes were derived from high-throughput RNA interference (RNAi) screens, and this dataset correlates specific genes to observable developmental defects.

---

### **4. miRNA-Target (miRNA)**
#### **Description:**
- MicroRNAs (miRNAs) are small non-coding RNAs that regulate gene expression post-transcriptionally. miRNA-target datasets predict interactions between miRNAs and their mRNA targets based on sequence complementarity and other factors such as evolutionary conservation.

#### **Example Datasets:**
- **PicTar Predictions (C. elegans, D. melanogaster, H. sapiens)**:  
  **PicTar** is a computational algorithm that predicts miRNA-target interactions by evaluating the evolutionary conservation of miRNA binding sites across multiple species. The predictions for *C. elegans* (Lall et al., 2006), *D. melanogaster*, and *H. sapiens* (Krek et al., 2005) provide a comprehensive map of predicted miRNA-mediated gene regulation across these organisms.
  
- **Hs_PicTar_ml (H. sapiens)**:  
  This specific dataset includes predicted miRNA-target interactions in *H. sapiens*, providing valuable insights into post-transcriptional gene regulation by miRNAs in human cells. The predictions are based on conserved miRNA binding sites across multiple organisms.

---

### **5. Predicted Genetic Interaction (PGI)**
#### **Description:**
- Predicted genetic interactions are genome-wide predictions based on computational algorithms that infer interactions between genes based on known genetic networks, phenotypes, or protein-protein interactions.

#### **Example Dataset:**
- **CePredictedGI (C. elegans)**:  
  The **CePredictedGI** dataset from Zhong and Sternberg (2006) predicts genetic interactions in *C. elegans* using a computational model trained on various genetic and protein interaction data. These predictions help identify gene networks potentially involved in essential biological processes.

---

### **6. Expression Correlation (ec)**
#### **Description:**
- Expression correlation data comes from comparing the expression levels of genes across various experimental conditions. Genes with correlated expression patterns are often functionally related or part of the same biological pathway.

#### **Example Dataset:**
- **ec (C. elegans)**:  
  This dataset contains expression correlation data based on a compendium of microarray experiments, with expression data collected under diverse biological conditions. Gunsalus et al. (2005) and Kim et al. (2001) have worked extensively on correlating gene expression in *C. elegans*, highlighting important regulatory networks.

---

### **7. Predicted Transcriptional Regulation (zPIC)**
#### **Description:**
- This dataset type involves predicted transcriptional regulatory relationships, typically using machine learning algorithms like **zPIC**. These algorithms infer how transcription factors regulate target genes based on expression data.

#### **Example Dataset:**
- **zPIC (E. coli)**:  
  The **zPIC** dataset predicts transcriptional regulatory relationships in *E. coli* based on expression data and validation through the **EcoCyc** database. This method gives confidence scores to the predictions, as shown in the work of Faith and Hayete et al. (2007).

---

### **8. Protein-DNA Binding (ChIP)**
#### **Description:**
- Chromatin immunoprecipitation (ChIP) is a technique used to identify the physical binding of DNA and protein, such as transcription factors or chromatin-associated proteins, across the genome. ChIP datasets provide insights into gene regulation and epigenetic mechanisms.

#### **Example Dataset:**
- **ChIP_conf (E. coli)**:  
  The **ChIP_conf** dataset provides confidence scores for protein-DNA binding interactions detected by ChIP in *E. coli*. The confidence score is calculated as (1 - P-Value)*100, indicating the strength of the interaction.

---

### **9. Literature Curated Interaction (LCI)**
#### **Description:**
- Literature-curated interactions are those collected manually from published studies. These are often considered highly reliable since they have been validated in peer-reviewed research.

#### **Example Dataset:**
- **HI1_CORE, HI1_HYPER_CORE, HI1_NON_CORE (H. sapiens)**:  
  These datasets are curated protein-protein interactions in humans. **HI1_CORE** includes interactions that are well-validated and central to biological pathways. **HI1_HYPER_CORE** consists of interactions with higher confidence, while **HI1_NON_CORE** contains less critical, though still valuable, interactions.
