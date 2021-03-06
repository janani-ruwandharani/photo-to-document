# Photo to document
Convert images to documents (PDF) including Perspective Transformation. There is a HTTP API implemented with Flask, for feeding image files.

## Installation and running
- Clone the repo and open 'photo-to-document' directory
- Create and activate the virtual environment
- run `pip install -r requirements.txt`
- _(Optional) Set env variables IMAGE_DIR, TF_IMAGE_DIR, and PDF_DIR_
- Run `python app.py`
- Upload an array of image files to localhost:5000/images with a POST request with 'files' as the key name

## Results
Contour finding fail 1:
![No countour 1](documentation/no-contour.png)

Contour finding fail 2:
![No countour 2](documentation/no-contours-1.png)

Success 1:
![Success](documentation/success-1-bnw.png)

Success 2:
![Success](documentation/success-02.png)

Success 3:
![Success](documentation/success-03-color.png)

Success 4 - PDF converted:
![Success](documentation/pdf.png)

## Acknowledgement:
Initial code for identifying margins and transformation was based on https://www.pyimagesearch.com/2014/08/25/4-point-opencv-getperspective-transform-example/
