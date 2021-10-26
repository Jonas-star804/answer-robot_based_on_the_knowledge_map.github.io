## Background
Knowledge map (Knowledge Graph), in the field of book intelligence community called domain Knowledge visualization or Knowledge map, is to display Knowledge development process and the structure relation of a series of different kinds of graphics, Knowledge resources and its carrier is described by using visualization technology, mining, analysis, building, drawing and display Knowledge and the connection between them.Knowledge map is through the applied mathematics, graphics, information visualization technology, theory and method of information science disciplines and metrology method such as citation analysis, co-occurrence analysis, and using the visualization of the image of the map to show discipline core structure, development history, the frontier and the overall knowledge structure to achieve a multidisciplinary integration of modern theories.It can provide practical and valuable reference for subject research.
To put it simply, a knowledge graph is a network of knowledge structures formed through the association of different knowledge, and this knowledge structure happens to be the cornerstone of artificial intelligence AI.Computer images, speech recognition and even NLP, which are currently popular in the FIELD of AI, are actually AI's 'perception' ability. The real 'cognitive' ability of AI depends on the knowledge graph.
At present, the application of knowledge graph is mainly in search, intelligent question answering, recommendation system and so on.The construction of knowledge graph generally includes data acquisition, entity recognition and relation extraction, data storage and application of knowledge graph.
This project will build a small medical knowledge map based on graph database Neo4j and a real medical data, and build a question and answer system based on the knowledge map to realize the automatic question and answer service of medical knowledge. The data used in this project is in JSON format, and the data is related to questions and answers in the medical field crawled by crawlers.
The data contains the following information:
- name: the disease name
- desc: specifies the disease description
- prevent: prevention
- cause: the cause
- get_prob:to get sick
- easy_get: people at risk of getting sick
- cure_way: the method to get cured
- cure_lasttime: cure timetable
- cure_prob: the probability to get cured
- symptom: symptoms
- acompany: complications
- cure_department: department to get cured
- common_drug: common drug
- recommand_drug: recommanded drug
- not_eat: should not eat
- check: check method
- drug_detail: the details of drug
The objective of the question answering system based on the rules matching completely achieved, through the key words matching, intention of question classification, medical problem belongs to the closed domain class scene, exhaustive and classification, the problems of the field and then use of cypher match to match to find secondary, according to the data returned by the template assembly question answer, finally to return the result.

## Technique
- Building knowledge graph based on py2Neo and Neo4j.
- Lent based on feature word intent recognition;
- Confer based problem resolution on CYPher.
- Knowledge retrieval based on Neo4j;
- Automatically generates text based on templates

## Env
- CentOs；
- neo4j
- Pycharm
- Python3.6
- tqdm
- py2neo
- ahocorasick

