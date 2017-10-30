# NIPS2015 Topic Modeling and Network Analysis

This notebook started off from Kaggle's [NIPS 2015 Papers dataset](https://www.kaggle.com/benhamner/nips-2015-papers), to enable and showcase analytical exploration on the NIPS data. I then then parsed the web for the number of citation recieved by each paper published in NIPS 2015, using [scholar](https://github.com/ckreibich/scholar.py) that extract citation information from Google Scholar. Combining the citaiton information and the topic modeling techniques, I could identify the most influencial papers/topics from NIPS 2015. 

NIPS is one of the top machine learning conferences in the world. According to [wikipedia](https://en.wikipedia.org/wiki/Conference_on_Neural_Information_Processing_Systems) some main topics covered at NIPS are: 1. Machine learning, 2. Statistics, 3. Artificial intelligence, 4. Computational neuroscience, etc. However, the topics are within the same domain which makes it more challenging to distinguish them as seperate topics (overlapping topics?). Here in this Kernel I will try to extract some topics using Latent Dirichlet allocation LDA. This repository features an end-to-end natural language processing pipeline, starting with raw data (full text of papers) and running through preprocessing, modeling and clustering papers based on their topics. I wrap-up by visualizing clusters of papers and their relative similarity using T-sne. We'll touch on the following points:

1. Topic modeling with LDA
2. Visualizing topic models with pyLDAvis
3. Visualizing LDA results with t-SNE and bokeh
4. Citation analysis

Note: Two major visualizations of this notebook are interactive graphs, which do not get loaded on the Github. To see them, go to this link: [Topic Modeling](http://nbviewer.jupyter.org/github/ykhorram/nips2015_topic_network_analysis/blob/master/NIP15_topics_citations1.ipynb#topic=4&lambda=0&term=)

Network analysis: Scientific collaboration Network
It's known that different scientists have different styles of working, some enjoy mentoring many pupils while others prefer working with fewer. Moreover, even for a given scientist, their pattern of interaction within the scientific community might change during the course of their career. In this kernel, I try to see if we can classify authors at NIPS'15 based on their collaboration, number and type of publication.
Here is the outline:

1. EDA
2. Network measures (Networkx)
3. KMeans clustering (scikit-learn)
4. KMeans visualization using PCA for dimensionality reduction
5. Network visualization (plotly and Networkx)

Note: Two major visualizations of this notebook are interactive graphs, which do not get loaded on the Github. To see them, go to this link: [Network analysis](http://nbviewer.jupyter.org/github/ykhorram/nips2015_topic_network_analysis/blob/master/nips_collaboration_network.ipynb)
