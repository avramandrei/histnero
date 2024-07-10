# HistNERo
This repository contains the Historical Romanian Named Entity Recognition (HistNERo) dataset.

The dataset has 10,026 sentences (i.e. 8,020 train, 1,003 valid and 1,003 train) annotated with five named entities: PERSON, ORGANIZATION, LOCATION, PRODUCT and DATE.

You can read more about the dataset in the following paper: [*HistNERo: Historical Named Entity Recognition for the Romanian Language*](https://arxiv.org/abs/2405.00155)

## Loading

To load the dataset, simply install the `datasets` library and run:

```Python
from datasets import load_dataset

dataset = load_dataset("avramandrei/histnero")
```

Each sample respects the following format:
```json
{
  "id": "528",
  "ner_tags": [0, 0, 0, 0, 0, 0, 0, 0, 5, 0, 0, 0, 3, 4, 4, 4, 4, 0],
  "tokens": ["maĭ", "incóce", "vidu", "locuitoriĭ", "suburbiilorŭ", ",", "iar", "la", "riul", "Sabiĭului", "de", "càtrâ", "bisericâ", "romanéscâ", "gr.", "unitá", "Mai", "."],
  "doc_id": "Brasov_20-_20Gazeta_20Transilvaniei_201852.ann",
  "region": "Transylvania"
}
``` 

## Citation
```
@article{avram2024histnero,
  title={HistNERo: Historical Named Entity Recognition for the Romanian Language},
  author={Andrei-Marius Avram and Andreea Iuga and George-Vlad Manolache and Vlad-Cristian Matei and Răzvan-Gabriel Micliuş and Vlad-Andrei Muntean and Manuel-Petru Sorlescu and Dragoş-Andrei Şerban and Adrian-Dinu Urse and Vasile Păiş and Dumitru-Clementin Cercel},
  journal={arXiv preprint arXiv:2405.00155},
  year={2024}
}
```
