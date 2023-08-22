# Semantic Kernel vs LangChain

The repo tries to compare Semantic Kernel and LangChain to show the difference and similarity between them.

| Semantic Kernel                                | LangChain | Note                                                       |
| ---------------------------------------------- | --------- | ---------------------------------------------------------- |
| Kernel                                         | Chains    | Construct sequences of calls                               |
| Planner                                        | Agents    | Auto create chains to address novel needs for a user       |
| Plugins (semantic functions + native function) | Tools     | Custom components that can be reused across different apps |
| Memory                                         | Memory    | Store context and embeddings in memory or other storage    |

## Supported languages

| Language   | Semantic Kernel | LangChain |
| ---------- | --------------- | --------- |
| Python     | ✅              | ✅        |
| JavaScript | ❌              | ✅        |
| C#         | ✅              | ❌        |
| Java       | ✅              | ❌        |

## Data connection

| Building block                                                                                  | Semantic Kernel | LangChain                                                  |
| ----------------------------------------------------------------------------------------------- | --------------- | ---------------------------------------------------------- |
| Document loaders: Load documents from many different sources                                    |  [File Loaders](https://js.langchain.com/docs/modules/data_connection/document_loaders/integrations/file_loaders/) (CSV, Docx, EPUB, JSON, PDF, Markdown...) and [Web Loaders](https://js.langchain.com/docs/modules/data_connection/document_loaders/integrations/web_loaders/) (Azure Storage, S3, GitHub, Figma...)   | Word |
| Document transformers: Split documents, drop redundant documents, and more                      | Multiple Split methods          | ❌       |
| Text embedding models: Take unstructured text and turn it into a list of floating point numbers | OpenAI, Azure OpenAI, Hugging Face, Cohere, Google PaLM, Google Vertex AI, TensorFlow    | OpenAI, Azure OpenAI, Hugging Face |
| Vector stores: Store and search over embedded data  |  Over 50 vector stores        |  About 10 vector stores   |
| Retrievers: Query your data  | Simple semantic search, Contextual compression, Time-weighted vector store retriever, Parent Document Retriever, Self Query Retriever, Ensemble Retriever, and more.     | Simple semantic search    |