# Analysis-of-who-trust-whom-online-social-network-using-Page-Rank
Exploring the structure of a directed social network, namely the Epinions
Social Network. This is a who-trust-whom online social network of a general
consumer review site Epinions.com. Members of the site can decide whether to ''trust'' each other.
All the trust relationships interact and form the Web of Trust which is then combined with review
ratings to determine which reviews are shown to the user.
# Problem 1
In this problem, we will try to inquire the similar structure the ones Broder et al. employed in their
seminal paper where they determined that the web graph is structured like a bowtie. The authors
discovered that the web graph had a large strongly connected component (SCC) which could be
reached from any node in IN, and could go to any node of OUT. There were also TENDRILS
hanging off IN and OUT, containing nodes reachable from portions of IN or nodes going to
portions of OUT. TENDRILS going from IN to OUT without touching SCC formed TUBES.
There are also some DISCONNECTED components isolated from the rest of the graph.
We will try to determine whether bowtie structure exists in Epinions network or not. For that we
will compute the sizes of each region in the Epinions network. How many nodes are in the SCC,
IN, OUT, TENDRILS+TUBES (referring to TENDRILS and TUBES combined), and
DISCONNECTED regions? Write a python program to calculate the size of each of the above
components in Epinions network(both number of nodes and fraction of total nodes) (Hint: You
may want to use the SNAP functions GetMxWcc and GetMxScc along with BFS.)
Broder et al. found in their paper that given a pair of randomly chosen start and finish webpages,
one can get from the start page to the finish page by traversing links only approximately 25% of
the time. For the Epinions network, what is the probability that a path exists between two nodes
chosen uniformly from the graph?
# Problem 2
Page rank algorithm can be used to determine the ranks/importance of nodes in
the network. Apply page rank algorithm to the Epinions network. 
