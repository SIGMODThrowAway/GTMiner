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
<entity:e> \t <label:{0,1}>
```

### Training
To train the GTMiner Link Prediction system, please use the following command:
```
python train_GTMiner.py \
  --city sin \
  --lm bert \
  --lr 3e-5 \
  --n_epochs 10 \
  --batch_size 32 \
  --max_len 128 \
  --device cuda \
  --finetuning \
  --do_extend \
  --do_repair \
  --save_model
```

* ``--city``: Specify which city's data you wish to use for training. Possible values are ``sin``, ``tor``, ``sea``, ``mel``.
