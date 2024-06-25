# India News Headlines with Polarities

This repository contains a dataset of news headlines from India with sentiment polarities. The original dataset, provided by The Sparks Foundation, was not labeled and did not include polarity scores.

## Dataset Description

The dataset consists of news headlines collected from times of india by Harvard Dataverse. The original dataset did not have any sentiment labels. Using nlptown's pretrained bert-base-multilingual-uncased-sentiment model (known as BERT), I extracted polarity scores for each headline, indicating whether the sentiment is positive, negative, or neutral.

## Accessing the Dataset

Due to the large size of the dataset, it is hosted on tow plateforms: inside the [lfs directory](../lfs), and Google Drive. You can load the dataset from both: this project lfs dir, or directly from Google Drive. Regarding Google Drive, there are two approaches, that can be used to load data: through direct links, visiting drive and downloading the files, OR using gdown python's module.

1. The direct download links are given below:
   - [Google Drive: Original Dataset Link](https://drive.google.com/file/d/1Pl5_1iRbdcZTgzN21fPEZmwXmf4eZVOJ/view?usp=sharing)
   - [Google Drive: Sentiment Extracted Dataset Link](https://drive.google.com/file/d/1O9WWweR7BD6REPqFPznMNkTtanBrX2e5/view?usp=sharing)

2. An example of python code (using gdown module) for downloading file from code notebook:
   ```python

   # importing necessary libraries.
   import gdown
   import pandas as pd

   # Defining Google Drive file ID.
   file_id = "1O9WWweR7BD6REPqFPznMNkTtanBrX2e5"

   # Defining the destination file path (including file name and extension).
   # Two file: india-news-headlines.csv, and india-news-headlines-with-polarities.csv
   destination = "india-news-headlines-with-polarities.csv"

   # Creating the download URL.
   download_url = f"https://drive.google.com/uc?id={file_id}"

   # Downloading the file.
   gdown.download(download_url, destination, quiet=False)

   # Reading the file using pandas.
   newsData = pd.read_csv(destination)

   # Loading dataset into a DataFrame.
   news_df = pd.DataFrame(newsData)

   # Displaying the DataFrame.
   print(news_df.head())

   ```

## Usage

1. Download the dataset from the above links, or directly load from your code script.
2. Load the dataset into your preferred data analysis tool (e.g., Python, R, Excel).
3. Analyze the data as needed for your project or research.

## Example Code

Here is an example of how to load the dataset using Python, inside your notebook or code script:

```python
# Import necessary libraries.
import pandas as pd

# Replace 'your-file-path' with the actual path to the downloaded file.
file_path = 'path/to/india-news-headlines-with-polarities.csv'

# Load the dataset.
newsData = pd.read_csv(file_path)

# Convert into a DataFrame.
news_df = pd.DataFrame(newsData)

# Display the first few rows.
print(news_df.head())
```


## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

If you have any questions or need further assistance, please feel free to contact me through [my Linked-in profile](https://www.linkedin.com/in/khairullah-hamsafar), OR drop a mail to me at <a href="mailto:khairullahhamsafar@gmail.com">khairullahhamsafar@gmail.com</a>.
