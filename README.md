# SybilGovernance
Experimental Sybil Identification Method using Graph Deep Learning

# Proposal
This innovative project aimed at advancing and sharing a deep learning-based method for detecting sybils in Web3 governance voting. Initially funded by York University for one year, this project has successfully led to the creation of a unique method for sybil identification. While sybils, or fabricated identities, support user privacy they come at the cost of obscuring true voting patterns, which frustrates attempts at decentralized, polycentric governance.

The current stage of research focuses on refining, scaling, and validating the technique, with an emphasis on making it robust, reliable, and practically useful. Additionally, the project seeks to engage with and gather insights from Web3 and academic communities. This feedback will be crucial for further improvement and ensuring the method's applicability in real-world scenarios. The end goal is to open-source this refined method, contributing a valuable tool to the field of decentralized governance.

## Benefits to Web3 Community:

This research is theoretically grounded in a model of polycentric, decentralized governance of digital assets, which requires careful management of commonly held resources (aka “public goods”) for successful governance. As identified in “Open Problems in DAOs,” a persistent challenge facing fair and democratic implementation of polycentric, decentralized governance are sybils. In this context, sybils are defined as voting nodes that behave similarly because they share a common source (a unique person). In most traditional voting settings, one-person one-vote voting is easily accomplished by physically restricting repeat voting, however, in decentralized online settings, it is trivially easy to construct a new persona for every new vote and defeat controls on governance voting. Indeed, in crypto, creating a new (derived) wallet address for every new transaction is considered a privacy maximizing best practice. So, while the easy construction of sybils is a privacy benefit for users, the proliferation of sybils frustrates community managers, system designers and modellers, and social scientists, who are unable to accurately or meaningfully measure or model a governance system with sybils. My research over the last year offers a novel method to identify, label, and combine sybils into predicted ‘true identities’. 

## Impact and results:

This research presents a significant and multifaceted contribution to addressing the issue of sybil attacks in decentralized governance systems. At its core, it offers an advanced method for sybil detection, crucial for enhancing the integrity and reliability of such systems. This methodology not only fortifies the security of decentralized networks but also paves the way for more democratic and equitable governance models within the Web3 space.

A key aspect of this project is its open-source nature, which creates a collaborative environment conducive to innovation and continuous improvement. This approach not only speeds up the advancement of sybil detection technologies but also nurtures a sense of transparency and trust among community members.

Moreover, the implications of this research extend beyond immediate technical applications. It holds the potential to shape future policies and practices in digital governance, particularly in the realm of digital identity verification, far beyond the confines of blockchain technology.

Practical applications of this method are vast. Social scientists and DAO researchers will find it invaluable for generating more precise evaluations of decentralized voting and governance. Additionally, system designers can leverage this method to transform graph signals for more effective modelling. Infrastructure engineers, too, stand to benefit, as they can develop and deploy automated, online versions of this method for proactive sybil defense—a significant step forward given the current gap between today’s sybil defense mechanisms and the advancements in deep learning and artificial intelligence that have emerged recently and are utilized by this method.

The method itself employs a multilayered, high-dimensional graph convolutional neural network (GCNN) alongside a rapid vector embeddings search and label propagation technique. This inductive, highly parameterized method has been tested extensively with the [Snapshot.org](http://snapshot.org/) dataset, proving its efficacy in identifying, labeling, clustering, and amalgamating sybil nodes using well-established and intuitive deep learning techniques. Although the method has shown promising results (~5-15% graph reduction), it requires further refinement, validation, and feedback from the wider community to reach its full potential. A visualization from the algorithm-in-progress shows the method’s ability to identify sybil nodes, label and combine them, and to construct a sub-graph of “true identities.” 

Example of size and distribution of sybil clusters:
![sybil clusters](https://github.com/quinndupont/SybilGovernance/blob/main/Cluster_distribution.png?raw=true)

Example of graph visualization of clustered graph with predicted sybils:
![predicted sybils](https://github.com/quinndupont/SybilGovernance/blob/main/185000_clustered_graph.png?raw=true)




## Risks and Disclosures

The foundational research is already complete and the primary methods have been developed. Due to the complex, inductive nature of this research, the experimental results may not validate and the method may prove ultimately unsuccessful in practical settings. 

Quinn DuPont’s public financial disclosure regarding crypto is available here: http://iqdupont.com (no investment in crypto).
