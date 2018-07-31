# database-entity-name-pairs
These databases have entity names. The pairs formed from the combination of these entity names and a label indicating the similarity between each pair.

This repository has two data collections containing: Publication Venues names (conferences and journals) and Scientific Papers names.

The names were randomly selected from several areas, such as: Artificial Intelligence, Machine Learning, Knowledge Discovery, Computer Networks, Optimization, Human-Computer Interaction, Virtual Reality, Internet of Things, Smart Cities, Natural Language Processing, Standards Engineering, Semantic Web, Bioinformatics, Civil Engineering, Biology, Health, Agriculture, Education and Chemistry, resulting in 150 names for each data collection. These names were then combined and compared two by two, generating the pairs to be verified.

For the collection of data from the Scientific Papers entity, a group of three people evaluated the pairs to check for any similarity between them, following the same criteria. The final label of the pair is the information provided by the majority, generating for each data set two subsets, called in this work of similar (have some relation between them) and not similar (there is no relation between them).

For the data collection of the Publication Venue entity, the category information provided on a call for papers webpage (www.wikicfp.com) was used. Usually each publication venue is assigned to 4 categories (large areas). If two publication venues have more than 3 categories in common, they are labeled as similar. If they do not share any category, they are labeled as not similar. And the pairs that have 1 or 2 categories in common, were labeled manually by the group of 3 people.

The entity-names.txt file has the 150 names selected for the entity. The first column is your ID and the second column is the name of the entity.

id; entity-name
1; the big data architecture for security data and its application to phishing characterization
2; a capacitated plant model for reverse logistics activities
3 case study of software process improvement implementation
...

The entity-name-pairs.txt file contains the pairs formed with the 150 entity names. The first column is the similarity between the pair. A similar pair has a label equal to 1 and a non-similar pair has a label equal to 0. The second and third columns refer to the IDs of the names being compared.

similarity-label; id-entity-name-1; id-entity-name-2
0; 1; 2
0, 1, 3
0; 1; 4
...
