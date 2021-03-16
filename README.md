# Talkwall-Analysis

Talkwall is an educational app intended for use both in classrooms and virtual learning environments. It has been designed to get more people engaged in productive talk for learning. The technology in itself is not revolutionary; it is how the teacher uses Talkwall that matters. The main task of the teacher is to align educational practice and technology in the classroom. Working with subject content, Talkwall can help the teacher to encourage the dialogue that leads to learning in lessons.

This project analysises log data from students' use of Talkwall in dialogic lessons in England and Norway. There are two approaches to analysis: 

1) LDA: Latent Dirichlet Analysis which is a form of topic modelling or probabilistic latent semantic analysis (pLSA). LDA is a generative statistical model that allows sets of observations to be explained by unobserved groups that explain why some parts of the data are similar.
2) NA: Network analysis, described below. NA is used as a way to show teachers how the discussion progresses and to ensure all learners are paricipating equally and relevantly in the discussion.

In each notebook titled Network-Analysis, I use Dedupe to create clusters of text contributions that are the same or slight variations of one text statement. I then create unique id's for each participant (including students and teacher) and unique consecutive id's for each text clusters (so that there is no overlap between participant id's and text id's). 

I used these id's to create tuples of text and participant id's, which are entered as edges into a bipartite graph demonstrating the connections between students and ideas contributed to the Talkwall.

A bipartite graph consists of two groups of nodes. There are links between nodes of differing groups, but no links among nodes from the same group. The students and teachers together represent one group of nodes and the ideas/contributions represent another group of nodes.

After creating the bipartite graph, I identify nodes or links which have more importance for the network with centrality measures, namely degree distribution and betweenness centrality. 

I demonstrate the degree distribution of each network. The degree of a node indicates how many links it has. The degree distribution counts the number of nodes with a given degree. 

To explore betweenness centrality, I display projected graphs for both student/participant nodes and for the idea/contribution nodes independently. These graphs demonstrate the connectedness between students via ideas and the connectedness of ideas via students. These graphs are good indicators of which participants and ideas were centeral nodes and thus have a high importance within the network as a whole.

One notebook, called SWCHS_topicanalysis-Final demosntrates an initial exploration into topic analysis using a type of Natural language Processing called latent dirichlet analysis (LDA) with Gensim.  LDA is a generative statistical model using unsupervised classification of documents, similar to clustering on numeric data, which finds some natural groups of items (topics) without a clear idea of how many topics there are.
