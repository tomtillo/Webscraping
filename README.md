# Webscraping
web scraping using Selenium+Beautiful Soup in python

Webscraping certain sites is not permitted with just Beautiful Soup ( server restrictions/prohibitions on scrits ) .
Even with adding a header 
```python
            request_object.add_header('User-Agent',
                                      'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/33.0.1750.117 Safari/537.36')
```
would not help .

Selenium can open a browser object using a WebDriver call and navigate to the pages real time. BeautifulSoup runs as usual in the background. 
```python
driver = webdriver.Chrome(chrome_path)
```
