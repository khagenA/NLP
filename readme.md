# Project: NSF abstract clustering using k-mean clustering

This project implement K-means clustering algorithm. We will be using the NSF Abstract dataset in this project.

## Getting Started

These instructions will get run different stages of the project. The project is written in Jupyter Notebook using Python3 language.

### Prerequisites

Python3 packages needed to install 

▪	numpy		(Data structuring)
▪	pandas	 	(Data structuring)
▪	scipy	 	(distance calculations between vectors)
▪	sklearn	 	(PCA)
▪	seaborn	 	(Visualization)
▪	matplotlib (Visualization
▪	jupyter notebook	(python code execution in browser)
▪	nltk		(Tokenization)

### Starting Jupyter Notebook
Running jupyter notebook in project directory

Terminal: jupyter notebook 

Then open the required notebook file in the browser.

You can use Menu->Kernel->Restart & Run All option to execute all cells.
You can also use Shift+Enter to execute a single cell.

### Data-Set and Google Word2Vec data
Data-Set: NSF Grant documents: Part1
https://archive.ics.uci.edu/ml/machine-learning-databases/nsfabs-mld/

Word2Vec Library File: GoogleNews-vectors-negative300.bin.gz 


## Running the project:

### Pre-Processing: Pre-Processing.ipynb
(Note: Takes a while to read data from word2vec pre-trained data.)
Estimated Time: 10 mins

•	Includes Word2Vec library from gensim model to convert doc to vector
•	Read all the grant proposals in the 'Part1' folder and extract document identifier 'Award Number' and abstract content
•	Filter empty abstracts
•	Save data to ’docs_vector.csv’ file for post-processing


### Pre-Visualization: Pre-Visualization.ipynb
(Note: Takes a while to read all grant proposal files from the directory tree of 'Part1' folder.)
Estimated Time: 10 mins

2D visualization of the data with PCA 2-component decomposition.
Drop outliers and save final data to 'docs_vector_final.csv'.


### K-Means Clustering and Post-Visualization: K-Means-scratch.ipynb

K-Means Clustering for K = (1, 2, 3, 4, 5, 6, 7, 8, 9, 10). Post-visualization of labels assigned to docs and distribution of docs in each cluster. Also shows the SSE Profile for different values of K.
### K-Means Clustering and Post-Visualization: K-Means-sklearn.ipynb
K-Means Clustering using scikit learn.
## Author:
Khagendra Adhikari
