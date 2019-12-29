# Soccer-Game-Analysis
The idea is to visualize and analyze a soccer game using Socnet Visualization tool.

## Socnet Visualization Tool ##
Social Network Visualizer (SocNetV) is a cross-platform, user-friendly free software application for social network analysis and visualization. 
With SocNetV we can draw social networks with a few clicks on a virtual canvas, load field data from a file in a supported format (GraphML, GraphViz, Adjacency, EdgeList, GML, Pajek, UCINET, etc) or crawl the internet to create a social network of connected webpages.
Edit actors and ties through point-and-click, analyse graph and social network properties, produce beautiful HTML reports and embed visualization layouts to the network.

#### Main features ####

1. Standard graph and network cohesion metrics, such as density, diameter, geodesics and distances, connectedness, eccentricity, clustering coefficient, reciprocity, etc.</br>
2. Matrix routines: Adjacency plot, Laplacian matrix, Degree matrix, Cocitation, etc</br>
3. Advanced measures for social network analysis such as centrality and prestige indices (i.e. eigenvector and closeness centrality, betweenness centrality, information centrality, power centrality, proximity and pagerank prestige).</br>
4. Fast algorithms for community detection, such as triad census, clique census,etc.</br>
5. Structural equivalence analysis, using hierarchical clustering, actor similarities and tie profile dissimilarities, Pearson coefficients.</br>
6. Layout models based either on prominence indices (i.e. circular, level and nodal sizes by centrality score) or on force-directed placement (i.e. Kamada-Kawai, Fruchterman-Reingold, etc) for meaningful visualizations of the social networks.</br>
7. Multirelational network loading and editing. Load a social network consisting of multiple relations or create a social network on your own and add multiple relations to it.</br>
8. Random network creation using various random network generation models (Barabási–Albert Scale-Free, Erdős–Rényi, Watts-Strogatz Small-World, d-regular, ring lattice, etc)</br>
9. Famous social network analysis datasets, i.e. Padgett's Florentine families.</br>
10. Built-in web crawler  to automatically create "social networks" from links found in a given initial URL.</br>
11. Comprehensive documentation, both online and inside the application, which explains each feature and algorithm of SocNetV in detail.</br>

## Possible Analysis ##
An example visualization of an EPL soccer game is shown below.
![Soccer Game Analysis](https://github.com/arvindsastha/Soccer-Game-Analysis/blob/master/socnet-soccer.PNG)
</br>

Once you visualize a soccer game as a social network in the form of a graph with players as nodes and passes as edges, it opens up a new dimension to the analysis of a game. There are various kinds of analysis that can be done on a social network as we know. Namely, finding churn in that network, investigating key player problem, discovering communities within a network and so on. Now, if we think about it, all these could be applied to a soccer game as well. If we can do a churn analysis on the crowd/fanbase on specific intervals of a game it could tell us a lot about how the game went on. If we can find out the set of key players in the field, it could benefit the team from understanding their nature and building the team around those players. If we can discover a strongly connected component within that network of passes, we can easily identify the midfield trio that most teams are struggling to crack. This is an example based on several works in the field of Social Network Analysis. But there are a lot more that can be done wih these type of stats.

## Analysis using Socnet ##
`Game in Discussion: Bayern vs Dortmund, March 5 2016`
`Score: 0-0`

The game totally had around 1100 passes approximately. With the help of Socnet Visualizer, we can easily obtain the network of passes. We can also state some obvious facts from looking at this network. On analysing the network of Bayern players, it was found that there were few offensive plays. This could be easily pointed out from the fact there were very few passes that were made to the offensive players from the midfield and also the network density was much larger between midfield and defence. 

If we do the key player investigation (KP-1), following are the scores that were obtained based on [Borgatti](https://pdfs.semanticscholar.org/ddfa/6c05380ae7af63ac68e0e6fe020c44d688c4.pdf).

| Player | KP-score based on fragmentation |
| ---- | ---- |
| P. Lahm | 0.8732 |
| D. Alaba | 0.4352 |
| J. Kimmich | 0.3451 |
| J. Bernat | 0.2341 |
| R. Lewandowski | 0.0987 |
| T. Muller | 0.3451 | 
| A. Robben | 0.1235 |
| D. Costa | 0.2341 |
| A. Vidal | 0.4531 |
| X. Alonso | 0.4123 |

Based on these scores, we can easily see the key players in the build-up play. It would help Pep to generate a mind map of game and would help him further investigate the draw.

On the other side, this data could also be used by opponent to stop bayern from building from the back. It could light up those key players who are responsible for offensive attacks. Even if one of them were neutralized, the network/team would lose it's shape and becomes disconnected.

This is just an example analysis with passing statistics.
