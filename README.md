# Financial Report Retrieval-Augmented Generation (RAG)

**Financial Report RAG** is a Python-based application that leverages Retrieval-Augmented Generation (RAG) techniques to analyze and extract insights from financial reports. By integrating advanced language models with document retrieval methods, this tool aims to facilitate efficient and accurate financial analysis.

## Features

- **PDF Parsing**: Extracts textual data from financial report PDFs.
- **Vector Store Integration**: Utilizes ChromaDB for efficient document indexing and retrieval.
- **LLM Integration**: Employs large language models to generate contextual answers based on retrieved data.
- **Interactive Notebooks**: Provides Jupyter notebooks for step-by-step execution and experimentation.

## Getting Started

### Prerequisites

- Python 3.8 or higher
- Virtual environment tool (e.g., `venv` or `conda`)

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/avizyt/financial-report-rag.git
   cd financial-report-rag
   ```

2. **Set Up a Virtual Environment (Optional but Recommended)**

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Dependencies**

   *(Note: A `requirements.txt` file is not present. Please ensure necessary packages are installed as per your environment.)*

   ```bash
   pip install -r requirements.txt
   ```

   *If `requirements.txt` is unavailable, manually install required packages.*

4. **Set Up Environment Variables**

   Create a `.env` file in the root directory and add your API keys:

   ```env
   OPENAI_API_KEY=your_openai_api_key
   GEMINI_API_KEY=your_gemini_api_key
   ```

   Replace `your_openai_api_key` with your actual OpenAI API key.

## Usage

1. **PDF Extraction**

   Use the `pdf_extraction.ipynb` notebook to extract text from financial report PDFs. Place your PDF files in the `data/` directory.

2. **Financial Analysis**

   Run the `financial_report.ipynb` notebook to perform analysis on the extracted data. This notebook demonstrates how to query the data using RAG techniques.

   Ensure that the necessary configurations and data files are in place before running the script.

## Project Structure

```
financial-report-rag/
├── chroma_db/                 # Directory for ChromaDB vector store
├── data/                      # Contains financial report PDFs
│   └── NASDAQ_MSGM_2023.pdf   # Sample financial report
├── fin_rep.py                 # Main script for financial analysis
├── financial_report.ipynb     # Jupyter notebook for analysis
├── pdf_extraction.ipynb       # Jupyter notebook for PDF text extraction
└── .env                       # Environment variables file
```

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to fork the repository and submit a pull request.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

MIT