# GenAI Course Data Repository

Public repository containing datasets, images, pretrained models, and other resources for my Generative AI and Deep Learning courses.

## Repository structure

- `datasets/` — datasets used in lectures, assignments, and examples.
- `images/` — diagrams and figures used in the course notebooks.
- `pretrained_models/` — small pretrained models or weights (when applicable).
- `notebooks/` — demo notebooks illustrating how to load files directly from this repository.

## How to load files from notebooks

You can directly load any file using raw GitHub URLs. Example:

### Load dataset

```python
import pandas as pd

url = "https://raw.githubusercontent.com/YOUR_USERNAME/genAI-course-data/main/datasets/your_dataset.csv"
df = pd.read_csv(url)
```

### Load image

```python
from PIL import Image
import requests
from io import BytesIO

url = "https://raw.githubusercontent.com/YOUR_USERNAME/genAI-course-data/main/images/your_image.png"
response = requests.get(url)
img = Image.open(BytesIO(response.content))
img.show()
```

This structure allows you to load resources both in Google Colab and in local Jupyter setups with minimal configuration.

#### Notes
- This repository only contains public data used for educational purposes.
- For course notebooks and private teaching material, a separate repository is used.

