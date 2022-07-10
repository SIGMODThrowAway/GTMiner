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
Knowledge Graph Completion data files are stored in /data/KGC
Triple are represented as follows:

```
<entity:head> \t <entity:tail> \t <relation:r>
```
