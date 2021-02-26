# Talkwall-Analysis

In each notebook, I use Dedupe to create clusters of text contributions that are the same or slight variations of one text statement. I then create unique id's for each participant (including students and teacher) and unique consecutive id's for each text clusters (so that there is no overlap between participant id's and text id's). 

I used these id's to create tuples of text and participant id's, which are entered as edges into a bipartite graph demonstrating the connections between students and ideas contributed to the talkwall.

A bipartite graph consists of two groups of nodes. There are links between nodes of differing groups, but no links among nodes from the same group. 

I then identify nodes or links which have more importance for the network with centrality measures, namely degree distribution and betweenness centrality. 

In a network, we can determine the shortest path between any two nodes and count how many of these paths run through each node or link. This number gives the vertex or edge betweenness. 

The degree of a node indicates how many links it has. The degree distribution counts the number of nodes with a given degree. 

To explore betweenness centrality, I display projected graphs for both student/participant nodes and for the idea/contribution nodes independently. These graphs demonstrate the connectedness between students via ideas and between ideas via students. These graphs are a good indicator of which participants and ideas were centeral nodes thus have a high importance within the network as a whole.
