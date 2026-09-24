# Pharmaceutical Document RAG Pipeline

An end-to-end Retrieval-Augmented Generation (RAG) pipeline for pharmaceutical PDF bundles.

## Features
- PDF text extraction with PyMuPDF
- Page-level pharmaceutical document classification
- Logical document-boundary detection
- Metadata tagging
- Sentence-aware chunking
- Local MiniLM embeddings
- LlamaIndex vector retrieval
- BM25 keyword retrieval
- Metadata-aware query routing
- Cross-encoder reranking
- Grounded Gemini answer generation
- Page/source citations
- Gradio interface

## Run in Google Colab
1. Open `Pharmaceutical_RAG_Full_Pipeline.ipynb` in Colab.
2. Add `GOOGLE_API_KEY` in Colab Secrets.
3. Run the installation cell.
4. Run the notebook top to bottom.
5. Upload a digital pharmaceutical PDF when prompted.
6. Test the included queries or use the Gradio interface.

## Security
Do not commit API keys. The notebook reads the Gemini key from Colab Secrets.

## Note
PyMuPDF extracts text from digital PDFs. Scanned/image-only PDFs require OCR before the RAG stage.


## Working Demo
Open `Pharmaceutical_RAG_Working_Demo.ipynb` in Google Colab for an end-to-end demonstration using the same pipeline as the full project.

The demo automatically creates a synthetic five-page pharmaceutical bundle containing a Certificate of Quality, Packaging Specification, BSE/TSE Declaration, and Supplier Qualification record. It then runs the complete classification, document-boundary detection, metadata tagging, chunking, MiniLM embedding, vector + BM25 retrieval, query routing, reranking, grounded Gemini generation, citations, and Gradio interface.

Add `GOOGLE_API_KEY` to Colab Secrets before running it. The API key is never stored in this repository.
