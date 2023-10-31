# HealthClaimInsights:Text-Mining-Analysis-of-Exaggerated-Causal-Claims

**Background:**
Explore various text mining tasks related to health claim analysis. Yu et al. (2020) have employed Natural Language Processing (NLP) techniques to identify exaggerated causal claims in health news headlines. They categorized sentences into four distinct labels: no relationship (0), direct causal (1), conditional causal (2), and correlational (3). The data comes from PubMed research papers and health news headlines from Eurekalert. The goal is to practice cross-domain classification, clustering analysis, and zero-shot learning with these datasets.

**Task 1: Cross-Domain Classification**

Compare SVM and BERT in cross-domain classification. Train a causal claim classifier in one domain and test it in the other.
Report 3-fold cross-validation performance and utilize the entire training data in one domain to build the final model for predicting data in the other domain.
Perform error analysis.
For SVM, report the top 20 features for each category.
Compare SVM and BERT performance in this cross-domain classification task.
Data sets: annotated_pubmed.csv, annotated_eureka.csv

**Task 2: Zero-Shot Classification**

Utilize the Huggingface zero-shot-classification pipeline to predict causal claim strength in the labeled datasets.
Report precision, recall, F1 scores in each category, and macro-F1.
Evaluate if the zero-shot classifier performs consistently well in both domains.

**Task 3: Clustering**

Perform clustering analysis using 10,000 health news headlines.
Build a cluster model using SBERT+kMeans and another using BERTopic.
Compare the insights provided by these two models. Examine how they differ in the health topics they discover.
