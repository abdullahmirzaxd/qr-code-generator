```python
#SIMPLE QRDODE GENERATING

import qrcode as qr

img = qr.make("https://www.netflix.com/pk/") #give your own url which you want to make qrcode

file_path = ("D:/users/netflix_home_page.png") #give path and name of your own folder

img.save(file_path)

```
