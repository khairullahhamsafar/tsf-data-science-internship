# India News Headlines with Polarities

This repository contains a dataset of news headlines from India with sentiment polarities. The original dataset, provided by The Sparks Foundation, was not labeled and did not include polarity scores.

## Dataset Description

The dataset consists of news headlines collected from various sources. The original dataset did not have any sentiment labels. Using nlptown's pretrained bert-base-multilingual-uncased-sentiment model (known as BERT), I extracted polarity scores for each headline, indicating whether the sentiment is positive, negative, or neutral.

## Accessing the Dataset

Due to the large size of the dataset, it is hosted on Google Drive. You can download the dataset from the following link:

1. [Google Drive: Original Dataset Link](https://drive.google.com/file/d/1Pl5_1iRbdcZTgzN21fPEZmwXmf4eZVOJ/view?usp=sharing)
2. [Google Drive: Sentiment Extracted Dataset Link](https://drive.google.com/file/d/1O9WWweR7BD6REPqFPznMNkTtanBrX2e5/view?usp=sharing)

## Usage

1. Download the dataset from the above link.
2. Load the dataset into your preferred data analysis tool (e.g., Python, R, Excel).
3. Analyze the data as needed for your project or research.

## Example Code

Here is an example of how to load the dataset using Python:

```python
import pandas as pd

# Replace 'your-file-path' with the actual path to the downloaded file.
file_path = 'path/to/india-news-headlines-with-polarities.csv'

# Load the dataset.
data = pd.read_csv(file_path)

# Convert into a DataFrame.
df = pd.DataFrame(data)

# Display the first few rows.
print(df.head())
```


## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

If you have any questions or need further assistance, please feel free to contact me at [khairullahhamsafar@gmail.com].
