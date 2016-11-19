# vldb2010data

A description of the datasets associated with: [Hay et al. Boosting the Accuracy of Differentially Private Histograms Through Consistency. In PVLDB 2010.](http://dl.acm.org/citation.cfm?doid=1920841.1920970)  

Please cite above paper when using this data.  Also, please do not distribute the data to other parties.


## Search Logs

- Filename: `search_logs.txt`
- Synthesized dataset, derived from interpolating Google Trends data and released AOL search logs.  Data reports frequency of search term "obama" over time.  Time period stretches from january 1, 2004 until august, 9, 2009 (2048 days).
- Each day is divided into 16 units.  A total of 2048*16=32,768 units.  this set up was chosen to have total number of units be a power of 2, which makes building hierarchical tree more convenient.
- File format: on each line, the number of searches in given unit of time, with time increasing with line number.
	
	
## NetTrace

- Filename: `nettrace.txt`
- See description in paper.
- File format: each line reports the number of external hosts connected to an internal host.  The lines are sorted based on IP address of internal host (but IP address has been omitted).
	

## SocialNetwork

- Filename: `social_network.txt`
- The degree distribution of *undirected* graph derived from UCSD Facebook crawl.  
- File format: each line is a node's degree.  
- The original data source for the directed graph was online at this URL [http://michaelkelly.org/projects/fb/graph.txt](http://michaelkelly.org/projects/fb/graph.txt) but it appears to be defunct.

	
