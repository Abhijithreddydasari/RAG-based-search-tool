# RAG-based-search-tool
## RAG:

Retrieval Augumented Generation is a technique where an LLM incorporates information from external sources (sources that are external to training set) before producing a response.

It mainly takes care of the two drawbacks of LLMs by:
1. Citing the sources of its information (using the external data source)
2. Gives up-to-date information about anything asked 

Advantages:

- Removes the need for retraining data everytime & hence cost-effective implmentation
- LLMs can be fine-tuned to company specific information without customly making changes in it
- Gives up-to-date information when connecting to social media
- Accurate information with source transparancy

For obtaining the context related information from the external sources, we can use any method like classification or semantic similarity.

Best definition out there: Retrieval-Augmented Generation (RAG) is a technology that enhances the capabilities of Large Language Models (LLMs) by incorporating retrieval mechanisms to access external knowledge sources during the generation of responses.

![](https://github.com/Abhijithreddydasari/RAG-based-search-tool/blob/main/Project_docs/Working%20of%20RAG.png)


### Working:
![](https://github.com/Abhijithreddydasari/RAG-based-search-tool/blob/main/Project_docs/Workflow.png)
In the image above, the query is fed to the retrieval model which search the knowledge base for relevant docs and then send both the query and docs to the LLM, which then generates the response.
