# Talkwall-Analysis

In each notebook titled Network-Analysis, I use Dedupe to create clusters of text contributions that are the same or slight variations of one text statement. I then create unique id's for each participant (including students and teacher) and unique consecutive id's for each text clusters (so that there is no overlap between participant id's and text id's). 

I used these id's to create tuples of text and participant id's, which are entered as edges into a bipartite graph demonstrating the connections between students and ideas contributed to the Talkwall.

A bipartite graph consists of two groups of nodes. There are links between nodes of differing groups, but no links among nodes from the same group. The students and teachers together represent one group of nodes and the ideas/contributions represent another group of nodes.

After creating the bipartite graph, I identify nodes or links which have more importance for the network with centrality measures, namely degree distribution and betweenness centrality. 

I demonstrate the degree distribution of each network. The degree of a node indicates how many links it has. The degree distribution counts the number of nodes with a given degree. 

To explore betweenness centrality, I display projected graphs for both student/participant nodes and for the idea/contribution nodes independently. These graphs demonstrate the connectedness between students via ideas and the connectedness of ideas via students. These graphs are good indicators of which participants and ideas were centeral nodes and thus have a high importance within the network as a whole.

One notebook, called SWCHS_topicanalysis-Final demosntrates an initial exploration into topic analysis using a type of Natural language Processing called latent dirichlet analysis (LDA) with Gensim.  LDA is a generative statistical model using unsupervised classification of documents, similar to clustering on numeric data, which finds some natural groups of items (topics) without a clear idea of how many topics there are.
