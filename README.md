# Summer2024
Coding materials for Summer 2024

Click this button to open these coding materials in Google Colab 

# Open in Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/STARTneuro/Summer2024)


Function you may need for 05_Functions:

```
def gc_content_4(DNA):
  counter = 0
  for i in range(len(DNA)):
    if DNA[i] == 'G' or DNA[i] == 'C':
     counter += 1
  gc_content = counter / 4
  gc_content_percent = gc_content * 100
  return gc_content_percent
```
```
import os
import urllib.request

# Create the directory if it doesn't exist
os.makedirs('./Data', exist_ok=True)

# Get the data and save it as "sleep_data.txt"
data_url = 'https://raphaelvallat.com/images/tutorials/bandpower/data.txt'
sleep_data, headers = urllib.request.urlretrieve(data_url, './Data/sleep_data.txt')

```
