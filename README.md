# CS336 Self-Study: Language Modeling from Scratch

My independent work through **Stanford CS336: Language Modeling from Scratch**, following the course's public lectures and assignments. I am not enrolled at Stanford; I am a Northeastern University MSCS student doing this on my own to understand how modern language models are built, from the tokenizer up.

- Course site: https://stanford-cs336.github.io
- Official assignments: https://github.com/stanford-cs336

## Why

I build LLM applications (see [Xticket](https://github.com/xungirl/Xticket), a RAG assistant with a retrieval and latency benchmark). This project goes one level down: instead of calling a model, I implement one. The goal is to be able to explain every component, including why RoPE, why RMSNorm, and why AdamW decouples weight decay, not just to make the tests pass.

## Progress

| # | Assignment | What I build | Status |
|---|---|---|---|
| 1 | [Basics](https://github.com/stanford-cs336/assignment1-basics) | Byte-level BPE tokenizer, Transformer LM, AdamW, training loop | 🚧 In progress |
| 2 | [Systems](https://github.com/stanford-cs336/assignment2-systems) | Profiling, FlashAttention-2 in Triton, distributed data parallel | ⏳ Not started |
| 3 | [Scaling](https://github.com/stanford-cs336/assignment3-scaling) | Scaling-law experiments and fits | ⏳ Not started |
| 4 | [Data](https://github.com/stanford-cs336/assignment4-data) | Filtering, deduplication, quality classifiers | ⏳ Not started |
| 5 | [Alignment](https://github.com/stanford-cs336/assignment5-alignment) | SFT and GRPO for math reasoning | ⏳ Not started |

### Assignment 1 checklist
- [ ] Byte-level BPE tokenizer: training, encode, decode
- [ ] Transformer components: Linear, Embedding, RMSNorm, SwiGLU, RoPE, scaled dot-product attention
- [ ] Causal multi-head self-attention and Transformer block
- [ ] Transformer LM
- [ ] Cross-entropy loss, AdamW, cosine learning-rate schedule, gradient clipping
- [ ] Data loader, training loop, checkpointing
- [ ] Train on TinyStories and report validation loss
- [ ] Text generation with temperature and top-p sampling

## Results

Filled in as each assignment is completed, with the exact settings used.

| Assignment | Metric | Result |
|---|---|---|
| 1 | TinyStories validation loss | — |

## Repository layout

```
cs336_self_study/
├── assignment1-basics/   # official starter code + my implementation (cs336_basics/)
├── notes/                # lecture notes and write-ups
└── README.md
```

## Running

Each assignment uses [uv](https://github.com/astral-sh/uv) and targets Python 3.12–3.13.

```bash
cd assignment1-basics
uv run pytest        # unit tests; all fail with NotImplementedError until implemented
```

## Learning log

| Date | Progress |
|---|---|
| 2026-09-25 | Set up repository and Assignment 1 environment |

## Acknowledgements and academic integrity

Starter code, tests, and handouts belong to the Stanford CS336 course staff and are used under their license. All implementation code in this repository is my own. Following the course's AI policy, I use AI tools only for conceptual explanations and code review, not to write assignment solutions.
