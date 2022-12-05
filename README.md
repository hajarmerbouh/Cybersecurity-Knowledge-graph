The repository contains the following tasks : Construction of the corpus, Named Entity Recognition , Relationship Extraction , Construction of knowledge graph using py2neo , Analysis on the constructed KG with cypher query

**Conceptual model of the knowledge graph :**

![image](https://user-images.githubusercontent.com/77699359/205594664-66976e6e-9034-445a-95c0-d969bb658b81.png)

In general, it is essential to build beforehand an idea on the usefulness and the types of information that we need to access at the level of our knowledge graph, given that the field of cybersecurity is wide. This will make it easier for us to choose the documents on which we will base the creation of the graph. 

First of all, we will have to build the corpus: we can either base ourselves on a single collection of reports bearing the same type of information, or expand the field of knowledge by adding other types of information, from various sources, deemed to be useful during the analysis, while ensuring the homogeneity of the corpus built. Before starting the step of extracting the entities, it will have to carry out a preprocessing on the documents contained in the corpus in order to prepare the data or the data set that will be suitable for the application of the REN approach. 

By trying different models and different types of architecture, we will have a better chance of obtaining an efficient model that allows the extraction of entities. After obtaining the entities, we will need to know the context in which they are located. In order to contextualize the entities, we will first have to prepare the data so that it is adequate for the task of extracting the relationships and then to train a model that can predict the existing relationships between the entities as accurately as possible. 

Once we succeed in having a model that performs well in recognizing named entities and another model that performs well in extracting relationships. We can extract the triples from a collection of reports: entities and relations that contextualize them, and then build our knowledge graph. 

Since the objective is not only based on the construction of the graph but rather on its usefulness rather on its usefulness and efficiency in countering a cyber-attack. An analysis step is added towards the end, which consists of analyzing and querying the knowledge graph constructed. The figure above illustrates the approach followed.

**Overall design of the solution :**

![image](https://user-images.githubusercontent.com/77699359/205593799-b33e8936-6da4-481a-a02e-5e48bd7b52cb.png)

**Detailed design of the solution :**

![image](https://user-images.githubusercontent.com/77699359/205594972-7cfc9dd3-a9cd-4409-80b0-fd58e82ff6ba.png)

**Model Performance for the NER task**

![image](https://user-images.githubusercontent.com/77699359/205599401-dc4d6fbc-706d-4af1-aaff-9840b448f114.png)

**Model Performance for the Relation-Extraction task**

![image](https://user-images.githubusercontent.com/77699359/205599828-dea66006-f39b-432f-a7cf-fdcb916fd763.png)

**Small Overview of the constructed graph**

![image](https://user-images.githubusercontent.com/77699359/205599934-a3238a63-029e-4084-afc2-a10bafe0241a.png)




