# Blast-python

A python package utilizing the command-line blastn utility. Blast queries run through an API can often be time-consuming due to limited service by the provider, and subject to network errors. This package aims to be a simple command-line wrapper for executing blast queries in python. 

## Example
```python
from Blastn import Blastn, OutFmt

Blastn(
    db="db/NC_000001", 
    query="gallus_gallus/vtg1.fasta", 
    word_size=11, 
    num_threads=4, 
    out="123456.json", 
    outfmt=OutFmt.JSON_SEQALIGN
).run()
```
