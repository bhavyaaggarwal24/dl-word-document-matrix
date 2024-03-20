# Creation of word-document matrix using python and Numpy

This code generates a word-document matrix (A) from a text dataset. If the vocabulary (set of unique words) size is M and the number of documents is N, then the size of this matrix will be M X N. Using numpy data structures to create and manipulate this matrix.

**Consolidating all files in a list:** This involves collecting all text files into a single list, likely containing strings representing the text content of each document.

**Creating a list of Vocabulary:** Generating a list of unique words found across all documents in the dataset. This list will serve as the columns of the word-document matrix.

**Creating a null matrix with size M*N and adding words in the matrix to create a word-document matrix:** Using numpy, initialized a matrix of zeros with dimensions M x N, where M is the size of the vocabulary list and N is the number of documents. Then, iterate through each document, tokenize it (split into words), and update the matrix accordingly by incrementing the corresponding cell for each word occurrence in the document.

**Using Heatmap to visualize the matrix:** After generating the word-document matrix, visualized it using a heatmap, where higher frequency of word occurrences is represented by darker shades.

**Calculating TF-IDF score for each word in the matrix:** Computed the TF-IDF (Term Frequency-Inverse Document Frequency) score for each word in the word-document matrix. TF-IDF reflects the importance of a word in a document relative to its occurrence across all documents in the dataset.

**Using Cosine-similarity to find similar documents of a particular document:** Computed the cosine similarity between a particular document and all other documents in the dataset. Cosine similarity measures the cosine of the angle between two vectors, representing document representations, in a high-dimensional space.

**Using numpy to create a new matrix B of size N x N, where Bij represents the number of common words between document i and j:** Created a new matrix B with dimensions N x N (where N is the number of documents) using numpy. Each cell (i, j) in matrix B represents the number of common words between document i and document j in the dataset.
