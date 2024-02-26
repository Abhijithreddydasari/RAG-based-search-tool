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

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/475e7b3c-dace-4b7c-97f4-4d32707d0da5/1b317038-eacc-4120-83a6-e26fc27f796b/Untitled.png)

### Working:
