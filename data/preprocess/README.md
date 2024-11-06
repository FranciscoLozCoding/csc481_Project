# How to download

To download the kaggle dataset, https://www.kaggle.com/datasets/franciscolozdatasci/csc481-project-dataset version 2, use one of these methods



## kagglehub via Python
```py
import kagglehub

# Download latest version
path = kagglehub.dataset_download("franciscolozdatasci/csc481-project-dataset")

print("Path to dataset files:", path)

```

## Kaggle cli

```sh
#!/bin/bash
kaggle datasets download franciscolozdatasci/csc481-project-dataset
```

## cURL

```sh
#!/bin/bash
curl -L -o ~/Downloads/archive.zip\
https://www.kaggle.com/api/v1/datasets/download/franciscolozdatasci/csc481-project-dataset
```

## mlcroissant via Python

```py
import mlcroissant as mlc
import pandas as pd

# Fetch the Croissant JSON-LD
croissant_dataset = mlc.Dataset('www.kaggle.com/datasets/franciscolozdatasci/csc481-project-dataset/croissant/download')

# Check what record sets are in the dataset
record_sets = croissant_dataset.metadata.record_sets
print(record_sets)

# Fetch the records and put them in a DataFrame
record_set_df = pd.DataFrame(croissant_dataset.records(record_set=record_sets[0].uuid))
record_set_df.head()
```