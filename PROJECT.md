# Practised — portfolio notes

See [README.md](README.md) for the full index and
[INVOICE_EXTRACTION.md](INVOICE_EXTRACTION.md) for the deep-dive.

## What it is

A second practice collection (alongside [`ai-bootcamp`](../ai-bootcamp/PROJECT.md)),
this one weighted toward **applied ML notebooks** rather than from-scratch
primitives. ~12 self-contained experiments, mostly built in Colab, Oct 2025.

## Highlights

- **Invoice / receipt OCR** (`Trading_OCr.ipynb`) — the most complete piece: an
  end-to-end pipeline over the RVL-CDIP dataset (~2,477 invoice images), comparing
  OCR engines (EasyOCR vs PaddleOCR vs SuryaOCR), then regex + FLAN-T5 + a Groq
  LLM to pull out totals; reports ~85% extraction success. Tracked metrics with
  Weights & Biases. Full writeup in `INVOICE_EXTRACTION.md`.
- **Image classification** — pneumonia (X-rays), face-mask, Google-landmark.
- **Other ML** — earthquake prediction, a DL chatbot, title generation, vLLM
  inference experiments.
- **Tools** — a Redis-backed TF inverted-index search engine and a Tkinter text
  editor.

## Cleanup done in this pass (2026)

- The repo's README documented only the invoice project, making the whole grab-bag
  look like one app. Moved that content to `INVOICE_EXTRACTION.md` and wrote a new
  `README.md` that indexes every notebook/script.
- Labeled `mid_eng_stack.md` as reference material (a Perplexity research dump),
  not original code, and flagged `searchengine.py` as an incomplete scratch file.

## Note

Practice repo — breadth over polish, like ai-bootcamp. `tokenizer_test/` overlaps
with ai-bootcamp. The invoice OCR pipeline is the one piece substantial enough to
stand on its own.
