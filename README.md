# QueryExplorer 
## An Interactive Query Generation Assistant for Search and Exploration

Formulating effective search queries remains challenging, particularly when users lack expertise in a specific domain or are not proficient in the language of the content. Providing example documents of interest might be easier for a user. However, such query-by-example scenarios are prone to concept drift, and the retrieval effectiveness is highly sensitive to the query generation method, without a clear way to incorporate user feedback. To enable exploration and to support human-in-the-loop experiments we propose QueryExplorer -- an interactive query generation, reformulation and retrieval interface with support for HuggingFace 🤗 generation models and PyTerrier's retrieval pipelines and datasets, and extensive logging of human feedback. To allow users to create and modify effective queries, our demo supports complementary approaches of using LLMs interactively, assisting the user with edits and feedback at multiple stages of the query formulation process. With support for recording fine-grained interactions and user annotations, QueryExplorer can serve as a valuable experimental and research platform for annotation, qualitative evaluation, and conducting Human-in-the-Loop (HITL) experiments for complex search tasks where users struggle to formulate queries.

Out demonstration video can be watched [here](https://www.youtube.com/watch?v=sXBU8-uWR3o)

### Colab Notebook
For the convenience of researchers and developers, QueryExplorer can be quickly launched in less than two minutes using a Google Colab notebook.
<a href="https://colab.research.google.com/github/emory-irlab/query-explorer/blob/main/Query_Explorer.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> To quickly run the demo from your browser, click "Runtime > Run All" in the [colab notebook](https://colab.research.google.com/github/emory-irlab/query-explorer/blob/main/Query_Explorer.ipynb) and you are all set.

To let us know how you've used QueryExplorer or for any inquires or collaboration, email us at kdhole -@- emory.edu

### Recorded Annotations and Logs
Researchers can look at the continuously recorded annotations consisting of – generated queries, post reformulation queries, query-document relevance annotations, feedback information – all with metadata of session and timestamps. These can be viewed in the user interface through the Settings tab or directly in their raw json format. Check out the [sample logs generated](https://github.com/emory-irlab/query-explorer/tree/main/sample_results).

### Citation
If you've used QueryExplorer, consider citing our previous paper:

```bibtex
@misc{dhole2023interactive,
      title={An Interactive Query Generation Assistant using LLM-based Prompt Modification and User Feedback}, 
      author={Kaustubh D. Dhole and Ramraj Chandradevan and Eugene Agichtein},
      year={2023},
      eprint={2311.11226},
      archivePrefix={arXiv},
      primaryClass={cs.AI}
}
```
Also check [BETTERSearch](https://github.com/emory-irlab/better-search/tree/main).

Kaustubh Dhole, Shivam Bajaj, Ramraj Chandradevan, Eugene Agichtein (Emory IR Lab)

The project was partially funded by the Intelligence Advanced Research Projects Activity [IARPA](https://www.iarpa.gov/).
