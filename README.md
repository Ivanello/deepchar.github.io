# deepchar

[github.com/deepchar](https://github.com/deepchar) *Transliteration with sequence-to-sequence models and transfer learning*

<img src="/favicon.ico" align="left"/>

### What is transliteration?

About half of the billions of internet users speak languages written in non-Latin alphabets, like Russian, Arabic, Hebrew, Chinese, Greek, Armenian and Hindi.  Very often, they haphazardly use the Latin alphabet to write those languages.

`Привет`: `Privet`, `Privyet`, `Priwjet`, ...  
`كيف حالك`: `kayf halk`, `keyf 7alek`, ...  
`Բարև Ձեզ`: `Barev Dzez`, `Barew Dzez`, ...  

So a growing share of user-generated text content is in these "Latinized" or "romanized" formats that are difficult to parse, search or even identify.

Transliteration is the task of automatically converting this content back into the native canonical format.

`Aydpes aveli sirun e.`: `Այդպես ավելի սիրուն է:`

You can read more about what makes this problem non-trivial at [*Automatic transliteration with LSTM*](http://yerevann.github.io/2016/09/09/automatic-transliteration-with-lstm/) and [*Interpreting neurons in an LSTM network*](https://yerevann.github.io/2017/06/27/interpreting-neurons-in-an-LSTM-network/).

### Our approach

Our baseline approach is to train **character-level sequence-to-sequence** models on generated data.

Besides our modification to character-level, [Fairseq](https://github.com/pytorch/fairseq) is standard modern reference implementation of sequence-to-sequence, developed primarily for machine *translation* but in principle applicable to a wide range of tasks with sequence input and sequence output

Fairseq was developed by Facebook AI Research on PyTorch, and  Fairseq models can be launched and scaled in production with [pytorch/translate](https://github.com/pytorch/translate).

### Transfer learning

TODO

### Datasets

Constrained by lack of parallel corpora, and inspired by similar approaches to transliteration and other sequence-to-sequence tasks like grammar correction, we rely primarily on **data generation**.

See the [deepchar/data](https://github.com/deepchar/data) repo

### Benchmarks

See the [deepchar/benchmarks](https://github.com/deepchar/benchmarks) repo

### Results

TODO

### References

TODO
