# Summer2024
Materials from week 3 of STARTneuro: Intro to Extracellular Recording and Python
 

## Open in Google Colab
Click this button to open these coding materials in Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/STARTneuro/Summer2024)


```
import os
import urllib.request

# Create the directory if it doesn't exist
os.makedirs('./Data', exist_ok=True)

# Get the data and save it as "sleep_data.txt"
data_url = 'https://raphaelvallat.com/images/tutorials/bandpower/data.txt'
sleep_data, headers = urllib.request.urlretrieve(data_url, './Data/sleep_data.txt')
loadtxt = np.loadtxt(fname='./Data/sleep_data.txt', delimiter=',')
data = loadtxt
```

For notebook 9:
```
import urllib.request
url = 'https://raw.githubusercontent.com/STARTneuro/Summer2024/main/data/inflammation-01.csv'

# Load the data using numpy
response = urllib.request.urlopen(url)
data = np.loadtxt(response, delimiter=',')

```

## Resources for next steps in your coding journey

