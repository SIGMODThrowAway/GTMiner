# GTMiner
SIGMOD 2023 Submission


### Requirements

* Python 3.7.7
* PyTorch 1.9
* HuggingFace Transformers 4.9.2
* wget 3.2

Install required packages
```
pip install -r requirements.txt
```

### Data
* Knowledge Graph Completion data files are stored in /data/KGC
Triple are represented as follows:

```
<entity:head> \t <entity:tail> \t <relation:r>
```

Relations with corresponding ID are stored in config.py

* AOI Search data files are stored in /data/Classification
Data points are represented as follows:
```
<entity:e> \t <label:0/1>
```
