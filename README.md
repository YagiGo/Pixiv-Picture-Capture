# Pixiv-Picture-Capture
抓取P站图片然后保存在指定的文件夹内,图片名称为p站id
目前功能不完善，仅仅能够做到在已经登陆的pixiv网页中抓取规定页数内指定的关键字的单张图片。动图，组图会直接跳过，所以有时候找到了多少张图
片不一定会下载多少张图片。
高清原图目前无法抓取，可能和没有做login功能有关。

暂时无法做到只抓取评分高的图片的功能，可能和没有做login功能有关。

最终的功能希望能够抓取在指定的页数内，指定关键字的，评价高于指定值的所有图片（单张，组图，gif）。能够直接login。

基于python3.5
import urllib
import urllib.request
from bs4 import BeautifulSoup
import requests
import re
