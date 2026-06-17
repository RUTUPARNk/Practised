# Practised

A grab-bag of ML / AI practice projects and small tools — mostly Colab notebooks
plus a few standalone scripts (Oct 2025). Each is a self-contained experiment;
there's no single app here.

## Notebooks

| Notebook | What it explores |
|----------|------------------|
| `Trading_OCr.ipynb` | OCR pipeline for invoices/receipts — the most built-out one, see [INVOICE_EXTRACTION.md](INVOICE_EXTRACTION.md) (EasyOCR + FLAN-T5 + regex, ~2,477 RVL-CDIP invoices, Groq API for totals) |
| `pneumonia_detection.ipynb` | Medical image classification (chest X-rays) |
| `face_mask_detection.ipynb` | Mask / no-mask image classification |
| `G_landmark_detcn.ipynb` | Google-landmark-style image recognition |
| `earthquake_pred.ipynb` | Earthquake prediction on tabular/seismic data |
| `chatbot.ipynb` | Deep-learning chatbot |
| `title_generator.ipynb` | Text generation — title/headline generation |
| `vllm.ipynb` | vLLM inference experiments |

## Scripts & extras

- `searchengine.py` — TF-style inverted-index search engine (Redis-backed). *Note:
  a scratch/practice file, not all of it runs cleanly.*
- `texteditor.py` — a Tkinter text editor.
- `tokenizer_test/` — multi-head self-attention + single-layer perceptron from
  scratch (also lives in [`ai-bootcamp`](../ai-bootcamp/PROJECT.md)).
- `gpt-notebook-start/` — a GPT-from-scratch notebook starting point.
- `mid_eng_stack.md` — a research/reference dump (Perplexity output) of
  beginner-friendly data-engineering project ideas; reference material, not my code.
- `1.csv` — sample data.

See [INVOICE_EXTRACTION.md](INVOICE_EXTRACTION.md) for the one project written up
in depth.
