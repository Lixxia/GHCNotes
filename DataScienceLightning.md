# Data Science Lightning Talks

### Trusting User Annotations on the Web for Cultural Heritage Domains
- Crowdsourcing is very efficient for gathering data
- cultural heritage insitutions have millions of poorly annotated artefacts
- cultural heritage institutions are employing crowdsourcing to annotate their collections with specific details, but how do you trust this information
- try to solve this problem using machine learning, we train on features of the user and test the quality of the annotations, we also track user reputation
- model this information using probalistic techniques
- we train on features of the annotation and test on quality of annotations.
- quality of information is determined by the institutions
- provenance: determine when it was posted, typing time, country posted from
- apply machine learning to train on user, data and provenance features to determine trust of information!

<hr> 

### Only trust your data: experiment, measure and ship!
- most software changes are believed to be positive to the user experience, but are often flat or negative!
- we are terrible at correctly assessing the value of our own ideas/designs
- stop debating, just get the data
- don't let the HIPPO decide (highest paid person's opinion)
- concept is trivial
	- randomly split traffic between two or more versions
		A control
		B treatments
	- collect metrics of interest
	- analyze
	- measure quickly and abort fast if needed (fail fast)
- trust your data
	- experiment on a large portion of your customers
	- continuously run A/A tests in parallel with other A/B tests
	- OFAT: one factor at a time, don't tewak too many things at once
- measure multiple metrics
- early on in the project define key metrics you will be optimizing for 
- avoid the temptations to try and build optimal features through extensive planning without early testing of ideas

<hr>

### Big data graph mining as a tool for fraud detection
- fraud is a big problem, especially in the health care industry
- lots of data, what to do with it?
	- patterns
	- new pathways
	- association prediction
- organize data as a graph
	- helpful construct for representing and organizing data, can use well developed mathematical theory (graph theory)
- approach: transform data into a graph, then do analytics and algorithms
	- 3 fold approach (data->rdf graph -> analytics -> discovery->new patterns)
- difficulties:	
	- infrastructure: scaling for data volume
	- analytics: speed, scaling
	- discovery: pattern disvovery is challenging
	- unrealistic assumptions about data structure
- hardware approach: use bigger and faster computers
- software approach: create new algorithms or improve existing ones
- big hammer approach (uRiKA)
- implemented many existing graph algorithms (speed imrpovement for pattern search)
- development of new scalable methods, statistics and algorithms for heterogeneous graphs 
