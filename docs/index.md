### How to train a baseline model with Sockeye

Create a directory `data/` and place `hy-Latn.txt` and `hy.txt` in it

```
pip install sockeye
```

```
python -m sockeye.prepare_data -s data/hy-Latn.txt -t data/hy.txt -o data/
```

