## WEB SCRAPPING
# Required Libraries
- Beautifulsoup
- Scrapy
## Scraping with BeautifulSoup
```Python
import requests
from bs4 import BeautifulSoup

def Get_it(){
    page = requests.get("url")
    soup = BeautifulSoup(page.content, 'html.parser')

    print soup.find_all('p')[0].get_text()
    print soup.find_all('p')[1].get_text()
    print soup.find_all('p')[2].get_text()
    print soup.find_all('p')[3].get_text()
}

if __name__ =="__main__":
Get_it()
```

## Scraping with scrapy


