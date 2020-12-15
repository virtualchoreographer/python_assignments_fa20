# python_assignments_fa20
# Project 1 
# reads in a segmentation map (png file)
# connects with server provided by Nvidia to translate said map into a photorealistic image based on AI
# base64 encoding that is involved relates back to my Thesis project: to highlight connections between ancient forms of binary counting today's tech 
# the missing piece: how to automate this process of translating through a series of png files 

## Installation
# pip install gaugan

##### Process image and save it to disk
```
import gaugan

with open('input.png', "rb") as fh:
    image = gaugan.processImage(fh.read())

with open('output.jpg', "wb") as fh:
    fh.write(image)
```

####### Code manipulated from original: erikKeresztes
