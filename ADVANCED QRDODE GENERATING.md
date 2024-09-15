```python
#ADVANCED QRDODE GENERATING

import qrcode
from PIL import Image

qr = qrcode.QRCode(
    version=1,  # Controls the size of the QR code (1 to 40)
    error_correction=qrcode.constants.ERROR_CORRECT_H,  # Error correction level
    box_size=10,  # Size of each box (pixel size)
    border=4,  # Thickness of the border
    )
    
qr.add_data("https://www.netflix.com/pk/") #give your own url which you want to make qrcode

qr.make(fit=True)

img = qr.make_image(fill_color="blue", back_color="red") #you can choose any color and size you want

file_path = ("D:/users/netflix_color.png") #give path and name of your own folder

img.save(file_path)
```
