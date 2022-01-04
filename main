import os
from PIL import Image

directory = os.getcwd()
child_directory = os.path.join(directory, "WEBP")
os.mkdir(child_directory)
 
for filename in os.listdir(directory):
    f = os.path.join(directory, filename)

    # checking if it is a file
    if os.path.isfile(f):
        if filename.endswith('.webp'):
            new_file = filename + '.jpg'
            im = Image.open(filename).convert("RGB")
            im.save(new_file, "jpeg")
            os.rename(f, os.path.join(child_directory, filename))
