# CS336 Self-Study: Language Modeling from Scratch

My independent work through **Stanford CS336: Language Modeling from Scratch**, following the public course materials. I am not enrolled at Stanford.

- Course site: https://stanford-cs336.github.io
- Official assignment starter code: https://github.com/stanford-cs336

The goal is to build every piece of a modern language model myself, from the tokenizer to training, systems optimization, data, and alignment, and to understand why each piece works.

## Progress

| # | Assignment | What gets built | Status |
|---|---|---|---|
| 1 | [Basics](https://github.com/stanford-cs336/assignment1-basics) | BPE tokenizer, Transformer LM, AdamW, training loop | 🚧 In progress |
| 2 | [Systems](https://github.com/stanford-cs336/assignment2-systems) | Profiling, FlashAttention-2 in Triton, distributed data parallel | ⏳ Not started |
| 3 | [Scaling](https://github.com/stanford-cs336/assignment3-scaling) | Scaling-law experiments and fits | ⏳ Not started |
| 4 | [Data](https://github.com/stanford-cs336/assignment4-data) | Filtering, deduplication, quality classifiers | ⏳ Not started |
| 5 | [Alignment](https://github.com/stanford-cs336/assignment5-alignment) | SFT and GRPO for math reasoning | ⏳ Not started |

### Assignment 1 checklist
- [ ] Byte-level BPE tokenizer (training + encode/decode)
- [ ] Transformer building blocks (Linear, Embedding, RMSNorm, SwiGLU, RoPE, attention)
- [ ] Transformer LM
- [ ] Cross-entropy loss, AdamW, learning-rate schedule, gradient clipping
- [ ] Training loop and checkpointing
- [ ] Train on TinyStories and report validation loss

## Layout

```
cs336_self_study/
├── notes/        # lecture notes and write-ups
└── README.md
```

Each assignment will get its own folder as I start it.

## Results

Results will be added here as each assignment is completed.
