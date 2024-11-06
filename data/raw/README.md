# How to download

To download the kaggle dataset, https://www.kaggle.com/datasets/ismailnasri20/driver-drowsiness-dataset-ddd version 1, use one of these methods



## kagglehub via Python
```py
import kagglehub

# Download version 1
path = kagglehub.dataset_download("ismailnasri20/driver-drowsiness-dataset-ddd")

print("Path to dataset files:", path)

```

## Kaggle cli

```sh
#!/bin/bash
kaggle datasets download ismailnasri20/driver-drowsiness-dataset-ddd
```

## cURL

```sh
#!/bin/bash
curl -L -o ~/Downloads/archive.zip \
https://www.kaggle.com/api/v1/datasets/download/ismailnasri20/driver-drowsiness-dataset-ddd
```

## mlcroissant via Python

```py
import mlcroissant as mlc
import pandas as pd

# Fetch the Croissant JSON-LD for version 1
croissant_dataset = mlc.Dataset('www.kaggle.com/datasets/ismailnasri20/driver-drowsiness-dataset-ddd/croissant/download')

# Check what record sets are in the dataset
record_sets = croissant_dataset.metadata.record_sets
print(record_sets)

# Fetch the records and put them in a DataFrame
record_set_df = pd.DataFrame(croissant_dataset.records(record_set=record_sets[0].uuid))
record_set_df.head()
```