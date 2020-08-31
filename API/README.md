# News Bias Detection Chrome Extention

## Deployed API endpoint

https://news-bias-detection-api.herokuapp.com

## Usage

```python
import requests

inputText = 'https://www.cnn.com/2020/08/31/politics/election-2020-senate-races/index.html' #This is the URL of the website you are trying to access

response = requests.post('https://news-bias-detection-api.herokuapp.com/', json={'url': inputText}) #This sends the request

print("Status code: ", response.status_code)
print("Printing Entire Post Request")
print(response.json())
```
