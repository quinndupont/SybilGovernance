# SybilGovernance
Experimental Sybil Identification Method using Graph Deep Learning. Preprint available on [arXiv](https://arxiv.org/abs/2311.17929).

# March 2024 Update

Image of Wallet Fingerprint Vector Embeddings for Anonymous DAO Voters
![2dembeddings](https://github.com/quinndupont/SybilGovernance/blob/main/2dembeddings.png)

Image of Clustered (HDBSCAN) Wallet Fingerprints for Anonymous DAO Voters
![costofproposals](https://github.com/quinndupont/SybilGovernance/blob/fb09856f474404d706f4eda976657c0ec65fb5f9/costofproposals.png)

[Download Interactive 2D Plot of Clustered Anonymous Voters for Ten DAOs](https://github.com/quinndupont/SybilGovernance/blob/main/2d_embeddings_umap_plot.html)

[Download Interactive 2D Plot of Anonymous Voters for Ten DAOs](https://github.com/quinndupont/SybilGovernance/blob/main/2d_embeddings_umap_plot.html)

Unfortunately, these large HTML files do not display in Github. Download the HTML file and open in your browser to view the Bokeh plot locally.

# January 2024 Update
We are pleased to have received a $15,000 grant in [Covalent API](https://www.covalenthq.com/) credits and 12 months of Premium access which will allow us to continue our sybil research. We will continue to experiment with graph walking methods in an attempt to find direct validation methods for sybils. In our preliminary research, we used the Covalent API to construct external chain graphs (on ERC-20 tokens) that we explored using fast GPU BFS. With the possibility of calling and processing billions of transactions, the Covalent API offers a potentially transformational platform for further experimentation. Our first goal is to explore the graphs of individual DAOs and then to produce a new method for efficiently connecting and traversing these graphs. Additionally, we will continue to develop sybil detection methods, advancing the state of the art beyond motifs and heuristics. 

https://github.com/quinndupont/SybilGovernance/assets/6929744/5df91ed7-bba0-4f78-a450-ce6a06addfcb

This research is actively looking for additional sponsorship. If you can donate computing or other resources, please contact **quinndupont AT ieee.org**


# Graph Deep Learning
In decentralized governance systems, the presence of sybils poses substantial challenges for accurately measuring user influence, decision-making, and other aspects of community structure. These spurious identities can distort the representation of user roles, creating an inaccurate picture that also makes comparisons with other Online Communities literature problematic. This research seeks to address this challenge by developing a graph deep learning method tested against a popular DAO governance forum [Snapshot.org](https://snapshot.org). Specifically, the method involves a Graph Convolutional Neural Net (GCNN) with multiple engineered feature layers that learn vector node embeddings from a voting graph to construct a “similarity” subgraph, where similar nodes are identified using a fast vector search algorithm (Facebook AI Similarity Search, aka FAISS) and relabelled into clusters. The similarity graph is then reduced by combining predicted sybils.

## Experiments

See the preprint for details [arXiv](https://arxiv.org/abs/2311.17929).

E.g., cost to buy governance proposals: ![costofproposals](https://github.com/quinndupont/SybilGovernance/blob/fb09856f474404d706f4eda976657c0ec65fb5f9/costofproposals.png)

## Impact and results:

This research presents a significant and multifaceted contribution to addressing the issue of sybil attacks in decentralized governance systems. At its core, it offers an advanced method for sybil detection, crucial for enhancing the integrity and reliability of such systems. This methodology not only fortifies the security of decentralized networks but also paves the way for more democratic and equitable governance models within the Web3 space.

A key aspect of this project is its open-source nature, which creates a collaborative environment conducive to innovation and continuous improvement. This approach not only speeds up the advancement of sybil detection technologies but also nurtures a sense of transparency and trust among community members.

Moreover, the implications of this research extend beyond immediate technical applications. It holds the potential to shape future policies and practices in digital governance, particularly in the realm of digital identity verification, far beyond the confines of blockchain technology.

Practical applications of this method are vast. Social scientists and DAO researchers will find it invaluable for generating more precise evaluations of decentralized voting and governance. Additionally, system designers can leverage this method to transform graph signals for more effective modelling. Infrastructure engineers, too, stand to benefit, as they can develop and deploy automated, online versions of this method for proactive sybil defense—a significant step forward given the current gap between today’s sybil defense mechanisms and the advancements in deep learning and artificial intelligence that have emerged recently and are utilized by this method.

The method itself employs a multilayered, high-dimensional graph convolutional neural network (GCNN) alongside a rapid vector embeddings search and label propagation technique. This inductive, highly parameterized method has been tested extensively with the [Snapshot.org](http://snapshot.org/) dataset, proving its efficacy in identifying, labeling, clustering, and amalgamating sybil nodes using well-established and intuitive deep learning techniques. Although the method has shown promising results (~2-5% graph reduction), it requires further refinement, validation, and feedback from the wider community to reach its full potential. A visualization from the algorithm-in-progress shows the method’s ability to identify sybil nodes, label and combine them, and to construct a sub-graph of “true identities.” 

Example of size and distribution of sybil clusters:
![sybil clusters](https://github.com/quinndupont/SybilGovernance/blob/main/Cluster_distribution.png?raw=true)

Example of graph visualization of clustered graph with predicted sybils:
![predicted sybils](https://github.com/quinndupont/SybilGovernance/blob/main/185000_clustered_graph.png?raw=true)

## Risks and Disclosures

The foundational research is already complete and the primary methods have been developed. Due to the complex, inductive nature of this research, the experimental results may not validate and the method may prove ultimately unsuccessful in practical settings. 

Quinn DuPont’s public financial disclosure regarding crypto is available here: http://iqdupont.com (no investment in crypto).

# Thanks and Acknowledgements
We would like to thank [Donncha Kavanagah](https://people.ucd.ie/donncha.kavanagh) (UCD) for early feedback and [Covalent](https://www.covalenthq.com/) for sponsorship.
![Covalent](https://github.com/quinndupont/SybilGovernance/blob/main/covalent.png?raw=true)
