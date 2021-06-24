# my-first-work
web scraping 
import requests
from bs4 import BeautifulSoup
url = input("Enter the URL:"  )
req = requests.get(url)
soup = BeautifulSoup(req.content, "html.parser")


print(soup.get_text())
