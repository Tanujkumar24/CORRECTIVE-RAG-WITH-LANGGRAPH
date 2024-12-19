
# Corrective RAG System

## Overview

This repository contains an implementation of a Corrective Retrieval-Augmented Generation (RAG) system. The project integrates multiple nodes to optimize information retrieval and response generation using advanced query evaluation and refinement techniques. The workflow dynamically assesses the relevance of retrieved documents and enhances queries when needed.

The project is ideal for anyone looking to explore advanced RAG systems that involve document grading, query rewriting, and leveraging external web searches for optimal answers.

---

## Workflow Explanation

### Workflow Overview

The system follows these steps:

1. **Retrieve Node:** The initial question/query is passed through a retrieval node to fetch relevant documents.
2. **Grade Node:** Retrieved documents are graded to evaluate their relevance.
3. **Relevance Check:** A decision is made based on the graded documents:
   - If all documents are relevant, generate an answer directly.
   - If any document is irrelevant, rewrite the query and perform a web search for better results.
4. **Rewriting Node:** The query is refined for better retrieval.
5. **Web Search Node:** Additional information is fetched from the web using the rewritten query.
6. **Answer Generation:** The retrieved information is processed to generate the final response.

### Workflow Diagrams

#### High-Level Workflow
![Corrective Workflow](https://github.com/Tanujkumar24/CORRECTIVE-RAG-WITH-LANGGRAPH/blob/main/graph/corrective.png)

#### Detailed Node Execution
![Detailed Graph](https://github.com/Tanujkumar24/CORRECTIVE-RAG-WITH-LANGGRAPH/blob/main/graph/graph.jpg)

These diagrams illustrate the step-by-step processing and decision-making in the pipeline, ensuring the system generates high-quality responses.

---

## Features

- **Document Relevance Evaluation:** Dynamically grades documents for accuracy.
- **Query Refinement:** Automatically rewrites queries to enhance retrieval performance.
- **Web Search Integration:** Leverages external resources for comprehensive information.
- **Modular Workflow:** Each step is implemented as an independent node for flexibility.

---

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Python 3.8+
- Jupyter Notebook
- Required Python libraries (install via `requirements.txt`)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/corrective-rag.git
   ```
2. Navigate to the project directory:
   ```bash
   cd corrective-rag
   ```
3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook corrective_rag.ipynb
   ```
2. Follow the instructions in the notebook to execute the pipeline step by step.
3. Use the diagrams provided to understand the workflow visually.

---

## Files

- **`corrective_rag.ipynb`**: Main Jupyter Notebook containing the code and explanations.
- **`README_corrective.png`**: High-level workflow diagram.
- **`README_graph.jpg`**: Detailed execution graph.
- **`requirements.txt`**: List of dependencies.

---

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

---

## License

This project is licensed under the MIT License.

---

## Contact

For further queries, contact [tanujkumar](mailto:tanuj.mangalapally@gmail.com).
**Portfolio**: [tanujkumar-portfolio](https://tanujkumar24.github.io/Tanujkumar-portfolio/)
