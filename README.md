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
