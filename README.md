# citations_predictions
Predict missing links in research papers citation networks

The goal is to identify missing citations in a citation network of research articles. 
A citation network is represented as a graph G=(V, E), where the nodes correspond to scientific articles and the existence of a directed edge between nodes u and v, indicates that paper u cites paper v.  
Each node (i.e., article) is also associated with information such as the title of the paper, publication year, author names and a short abstract. 

A number of edges have been randomly removed from the original citation network.  The goal is to accurately reconstruct the initial network using graph-theoretical and textual features, and possibly other information. 
The key metric is F1 score.

The algorithm uses a combination of graph theory (degree centrality, Jaccard similarity) and natural language processing such as Word Embedding to analyze pairwise titles distance or abstracts distance.

The best model manages to reach 0.96702 F1 score.

