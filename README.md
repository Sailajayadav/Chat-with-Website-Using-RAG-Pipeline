
# Chat with Website Using RAG Pipeline

This project leverages the Retrieval-Augmented Generation (RAG) pipeline to enable conversational AI to interact with website content. It uses crawling, scraping, embedding, and semantic search techniques to process web data and generate meaningful responses based on user queries.

## Features

- **Website Crawling and Scraping**: Fetches website content dynamically.
- **Content Chunking and Embedding**: Breaks down large content into manageable chunks and generates embeddings for semantic understanding.
- **Semantic Search**: Quickly retrieves the most relevant chunks for a given user query.
- **RAG Integration**: Combines information retrieval with a generative model to produce human-like responses.
- **User Query Handling**: Supports natural language queries for real-time interaction with website data.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/chat-with-website-rag.git
   cd chat-with-website-rag
   ```

2. Create a virtual environment:
   ```bash
   python3 -m venv env
   source env/bin/activate  # For Windows, use `env\Scripts\activate`
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Start the Application**:
   Run the main script to initialize the pipeline.
   ```bash
   python main.py
   ```

2. **Interact with the System**:
   Enter queries in the terminal or web-based UI, and the system will return responses generated using the RAG pipeline.

## Workflow

1. **Crawling**: Retrieves HTML content from specified URLs.
2. **Scraping**: Extracts and cleans textual data from the HTML.
3. **Chunking**: Divides the content into smaller segments for efficient processing.
4. **Embedding**: Uses a pre-trained model (e.g., Sentence-BERT) to convert chunks into embeddings.
5. **Semantic Search**: Matches user queries with the most relevant embedded content.
6. **Response Generation**: Augments retrieved content with a language model (e.g., GPT) to generate human-readable answers.

## Technologies Used

- **Python**: Core programming language.
- **BeautifulSoup/Selenium**: For web crawling and scraping.
- **Sentence-BERT**: For embedding content.
- **FAISS**: For efficient semantic search.
- **Hugging Face Transformers**: For generative model integration.
- **Flask/FastAPI** (Optional): For creating a web-based user interface.

## Example

```text
Loading embedding model...
Crawling and scraping websites...
Chunking and embedding content...
Enter your query: What is Washington?
Searching content...
Generating response...
Response: "The University of Washington (UW) is a leading institution known for its achievements in biochemistry, astronomy, and marine science. It is based in Seattle, WA."
```

## Customization

1. **Add New Websites**: Update the `websites.txt` file with URLs to include in the crawling process.
2. **Change Embedding Model**: Modify the embedding function in `embedding.py` to use a different model.
3. **Enhance Search**: Experiment with FAISS configurations for improved semantic matching.

## Future Enhancements

- Add support for handling multimedia content.
- Integrate advanced summarization techniques.
- Enable multilingual support for global use cases.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve the project.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

- [Hugging Face](https://huggingface.co/) for pre-trained models.
- [FAISS](https://github.com/facebookresearch/faiss) for semantic search.
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) for web scraping.
```

