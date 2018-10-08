# deepchar

Transliteration with sequence-to-sequence models and transfer learning

[github.com/deepchar](https://github.com/deepchar)

### What is transliteration?

### Our approach

Our baseline approach is to train **character-level sequence-to-sequence** models.  Besides our modification to character-level, [Fairseq] is standard modern reference implementation of sequence-to-sequence, developed primarily for machine *translation* but in principle applicable to a wide range of tasks with sequence input and sequence output

Fairseq was developed by Facebook AI Research on PyTorch, and  Fairseq models can be launched and scaled in production with [pytorch/translate](https://github.com/pytorch/translate).

### Transfer learning

### Datasets

Constrained by lack of parallel corpora, and inspired by similar approaches to transliteration and other sequence-to-sequence tasks like grammar correction, we rely primarily on **data generation**.

### Benchmarks

See the [deepchar/benchmarks](https://github.com/deepchar/benchmarks) repo

### Results


### References

