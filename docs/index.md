### How to train a baseline model with Sockeye

Create a directory `data/` and put parallel files for training and validation into it:`hy-Latn.txt`, `hy.txt`, `hy-Latn.val.txt`, `hy.val.txt`

```
pip install sockeye
```

```
python -m sockeye.prepare_data -s data/hy-Latn.txt -t data/hy.txt -o data/
```

```
python -m sockeye.train -s data/hy-Latn.txt -t data/hy.txt -vs data/hy-Latn.val.txt -vt data/hy.val.txt -o models/ -pd data/
```
