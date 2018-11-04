### How to train a baseline model with Sockeye

Create a directory `data/` and put parallel files for training (`hy-Latn.txt`, `hy.txt`) and validation (`hy-Latn.val.txt`, `hy.val.txt`).  We start with 100K training examples and 100 validation examples.

```
pip install sockeye
```

There is an optional data preparation step, we will skip it for now.

```
python -m sockeye.train --use-cpu \
            -s data/hy-Latn.txt -t data/hy.txt \
            -vs data/hy-Latn.val.txt -vt data/hy.val.txt \
            -o models/
```

This will take 15 hours or so.

See also: [https://aws.amazon.com/de/blogs/machine-learning/train-neural-machine-translation-models-with-sockeye/](https://aws.amazon.com/de/blogs/machine-learning/train-neural-machine-translation-models-with-sockeye/)
