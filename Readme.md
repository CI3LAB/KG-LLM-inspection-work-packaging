This is the repository of article *A KG-LLM enabled inspection work packaging approach in module prefabrication*
# Requirements
- openai
- numpy
- matplotlib
- seaborn
- pandas
- gower
- copy
- scipy
- sklearn
# Structure

- The .csv file in data folder can be imported into Neo4j to get the knowledge graph(KG). The KG-export.zip is exported from Neo4j.
- product2inspection mapping.ipynb shows the framework of leveraging LLM as the mapper in the multi-classification problem. The function of KG serves:  If we need some data as context or few-shot examples from the KG, langchain could seamlessly bridge the KG and the LLM. 
- PSO_HAC.ipynb is the code where PSO is applied for optimizing the number of clusters and feature weights. The function of KG serves: if we have some inspection tasks from the project but we don't know the detailed information about them, we can extract the features of the tasks from the KG using Cypher statements and do the work packaging.
- Results folder stores the work packaging results in the article. Each sheet in the .xlsx file represents a package
# Notes
- Please be aware that the authors try to improve and evolve the KG as time goes to make it more accurate and comprehensive. So the KG may not be exactly the same with  that documented in the paper.
- Please be aware that the LLMs especially the close-source ones are usually fully controlled by commercial companies. They could update the configurations without publicly noticing the users. So as time goes, the performance of the LLMs on the specific task in the article may be different. 
- If you have any comments/questions/want to contribute to the data or code, please email dong_qing@connect.hku.hk. I'm happy to chat and your concrete advice and criticism is welcomed.