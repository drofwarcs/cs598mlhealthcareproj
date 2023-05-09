# cs598 Deep Learning for Healthcare Spring 2023

This was our final project for @Baymatt and myself for the spring 2023 class. This repo consist of a Jupyter Notebook detailing the entire process to re-implent the paper [Predicting Heart Failure Readmission from Clinical Notes using Deep Learning](https://ieeexplore.ieee.org/document/8983095).

### Dependencies
Dependencies can be found in the [environment.yml](https://github.com/drofwarcs/cs598mlhealthcareproj/blob/data/environment.yml) file or directly in the Jupyter notebook towards the top.

### Data Access
This project uses the following data:

- MIMIC III clinical data. [Download instructions here](https://physionet.org/content/mimiciii/1.4/). More info about whats in the data and its schema can be [found here](https://mimic.mit.edu/docs/).
- Word2Vec embeddings. The paper makes use of a compiled word2vec word vector help build word embeddings for the machine learning models. The file can be [downloaded here](PubMed-and-PMC-w2v.bin) and more info on the data can be [found here](http://bio.nlplab.org/#word-vector-tools).


### Results

We were not able to reproduce the results in the paper. Our results turned out better, which could be due to over-fitting the models.

#### General Readmissions
| Model                     | Prec | Rec  | F1   | Acc  |
| ------------------------- |------|------|------|------|
| Deep Learning (CNN)       |0.79  |0.84  |0.82  |0.8   |
| Random Forest (TF-IDF)    |0.82  |0.81  |0.82  |0.81  |

#### 30 day Readmissions
| Model                     | Prec | Rec  | F1   | Acc  |
| ------------------------- |------|------|------|------|
| Deep Learning (CNN)       |0.89  |0.91  |0.90  |0.87   |
| Random Forest (TF-IDF)    |0.82  |0.96  |0.88  |0.83  |
