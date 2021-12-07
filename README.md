# Webscrapping
web automation
import requests
import bs4

wsc = requests.get('https://www.zbcnews.co.zw')

type(wsc)
wsc.text
soup = bs4.BeautifulSoup(wsc.text, 'lxml')
type(soup)
ws = soup.select('title')
ws[0].getText()
