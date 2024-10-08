# QueryExplorer 
![](https://img.shields.io/badge/PRs-welcome-brightgreen) 
<img src="https://img.shields.io/badge/Version-1.0-lightblue.svg" alt="Version">
[![arXiv](https://img.shields.io/badge/arXiv-2311.11226-pink.svg)](https://arxiv.org/abs/2311.11226)
![Python version](https://img.shields.io/badge/lang-python-important)
<a href="https://colab.research.google.com/github/emory-irlab/query-explorer/blob/main/Query_Explorer.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
![License: Apache](https://img.shields.io/badge/License-Apache2.0-yellow.svg) 

## An Interactive Query Generation Assistant for Search and Exploration

[Paper](https://aclanthology.org/2024.naacl-demo.11.pdf)

Formulating effective search queries remains challenging, particularly when users lack expertise in a specific domain or are not proficient in the language of the content. Providing example documents of interest might be easier for a user. However, such query-by-example scenarios are prone to concept drift, and the retrieval effectiveness is highly sensitive to the query generation method, without a clear way to incorporate user feedback. To enable exploration and to support human-in-the-loop experiments we propose QueryExplorer -- an interactive query generation, reformulation, and retrieval interface with support for **HuggingFace 🤗** generation models and **🐕 PyTerrier's** retrieval pipelines and datasets, and extensive logging of human feedback. To allow users to create and modify effective queries, our demo supports complementary approaches of using LLMs interactively, assisting the user with edits and feedback at multiple stages of the query formulation process. With support for recording fine-grained interactions and user annotations, QueryExplorer can serve as a valuable experimental and research platform for annotation, qualitative evaluation, and conducting Human-in-the-Loop (HITL) experiments for complex search tasks where users struggle to formulate queries.

📹 Our demonstration video can be watched [here](https://www.youtube.com/watch?v=sXBU8-uWR3o)

### Colab Notebook
For the convenience of researchers and developers, QueryExplorer can be quickly launched in less than two minutes using a Google Colab notebook.
<a href="https://colab.research.google.com/github/emory-irlab/query-explorer/blob/main/Query_Explorer.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> To quickly run the demo from your browser, click "Runtime > Run All" in the [colab notebook](https://colab.research.google.com/github/emory-irlab/query-explorer/blob/main/Query_Explorer.ipynb) and you are all set.

To let us know how you've used QueryExplorer or for any inquires or collaboration, email us at kdhole -@- emory.edu

### Recorded Annotations and Logs
Researchers can look at the continuously recorded annotations consisting of – generated queries, post reformulation queries, query-document relevance annotations, feedback information – all with metadata of session and timestamps. These can be viewed in the user interface through the Settings tab or directly in their raw json format. Check out the [sample logs generated](https://github.com/emory-irlab/query-explorer/tree/main/sample_results).

### Citation
If you've used QueryExplorer, consider citing the following papers.

```bibtex
@inproceedings{dhole2024queryexplorer,
      author = {Kaustubh D. Dhole and Shivam Bajaj and Ramraj Chandradevan and Eugene Agichtein},
      title = {QueryExplorer: An Interactive Query Generation Assistant for Search and Exploration},
      booktitle={2024 Annual Conference of the North American Chapter of the Association for Computational Linguistics -- System Demonstration Track},
      year = {2024},
      abstract={Formulating effective search queries remains a challenging task, particularly when users lack expertise in a specific domain or are not proficient in the language of the content. Providing example documents of interest might be easier for a user. However, such query-by-example scenarios are prone to concept drift, and the retrieval effectiveness is highly sensitive to the query generation method, without a clear way to incorporate user feedback. To enable exploration and to support Human-In-The-Loop experiments we propose QueryExplorer– an interactive query generation, reformulation, and retrieval interface with support for Hug-gingFace generation models and PyTerrier’sretrieval pipelines and datasets, and extensivelogging of human feedback. To allow users to create and modify effective queries, our demo supports complementary approaches of using LLMs interactively, assisting the user with edits and feedback at multiple stages of the query formulation process. With support for recording fine-grained interactions and user annotations, QueryExplorer can serve as a valuable experimental and research platform for annotation, qualitative evaluation, and conducting Human-in-the-Loop (HITL) experiments for complex search tasks where users struggle to formulate queries.},
      url = {https://arxiv.org/pdf/2403.15667.pdf},
      note = {Video: \url{https://www.youtube.com/watch?v=sXBU8-uWR3o}, Code: \url{https://github.com/emory-irlab/query-explorer}}
}
@misc{dhole2023interactive,
      title={An Interactive Query Generation Assistant using LLM-based Prompt Modification and User Feedback}, 
      author={Kaustubh D. Dhole and Ramraj Chandradevan and Eugene Agichtein},
      year={2023},
      url={https://arxiv.org/pdf/2311.11226.pdf},
      eprint={2311.11226},
      archivePrefix={arXiv},
      primaryClass={cs.AI}
}
```
Also check [BETTERSearch](https://github.com/emory-irlab/better-search/tree/main).

Kaustubh Dhole, Shivam Bajaj, Ramraj Chandradevan, Eugene Agichtein (Emory IR Lab)

The project was partially funded by the Intelligence Advanced Research Projects Activity [IARPA](https://www.iarpa.gov/).
