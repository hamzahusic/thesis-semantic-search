# Semantic Search over Thesis Abstracts

**Course:** IT 3004 – Introduction to Natural Language Processing, International Burch University
**Topic:** #11 – Semantic search over theses

## Team

| Name | GitHub |
|---|---|
| Hamza Husic | @hamzahusic |
| Nedim Smajic | @nedimsmajic |
| Benjamin Mahmutovic | @MahmutovicB |

## Project Description

Keyword search often misses relevant theses that describe the same idea with different words
(for example, "opinion mining" vs. "sentiment analysis"). This project builds a search system
that finds theses and papers by **meaning**, not only by matching keywords.

We compare three approaches:

1. **Baseline:** BM25 keyword search
2. **General embeddings:** a pretrained multilingual sentence-embedding model used without changes
3. **Main method:** the same embedding model **fine-tuned by our team** on thesis abstracts

## Research Question

Does fine-tuning embeddings on thesis abstracts beat general embedding models and BM25?

## Data (planned)

- IBU thesis and paper abstracts (subject to the repository's terms of use)
- arXiv abstracts (arXiv metadata dataset, CC0)
- Our own test set: at least 100 queries with manually labelled relevant documents

Raw data that cannot be redistributed is not stored in this repository; access instructions will be provided in `data/README.md`.

## Evaluation (planned)

nDCG@10, MRR@10 and Recall@10 on the team-built test set.

## Planned Repository Structure

```
├── data/            # data or data access instructions
├── notebooks/       # data analysis
├── src/             # preprocessing, baseline, embedding model, evaluation
├── results/         # saved results and figures
├── docs/
│   └── AI_LOG.md    # record of AI tool use
├── CONTRIBUTIONS.md
├── requirements.txt
└── README.md
```

## Installation and Usage

_To be added once the first implementation is ready._

## Status

Milestone 2: proposal and repository setup.
