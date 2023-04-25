# UpscalingImages
Image Upscaling and Similarity Comparison
This program demonstrates various image upscaling methods using OpenCV and compares the similarities of the upscaled images using the CLIP-ViT-B-32 Sentence Transformer model. The program uses different interpolation methods to upscale the input image, including Nearest Neighbor, Bilinear, Bicubic Spline, Generalized Bicubic (Lanczos4), and a combination of all methods.

Dependencies
OpenCV
matplotlib
numpy
sentence-transformers
Pillow
You can install these dependencies using pip:

Copy code
pip install opencv-python matplotlib numpy sentence-transformers Pillow
Usage
Place your input image file in the same directory as the script and update the input_image_path variable with the file name.
python
Copy code
input_image_path = 'uk.jpg'
Run the script to perform the upscaling and similarity comparison:
bash
Copy code
python main.py
The upscaled images will be saved in the current directory with the following file names:

nearest_neighbor.jpg
bilinear.jpg
bicubic_spline.jpg
generalized_bicubic.jpg
all.jpg
The script will display a plot comparing the original and upscaled images.

The program will use the CLIP-ViT-B-32 Sentence Transformer model to compute the embeddings of the images and find similar images based on cosine similarity scores. The scores and image pairs will be printed in the console.

Example Output
less
Copy code
Finding near duplicate images...

Score: 79.593%
all.jpg
generalized_bicubic.jpg
In this example output, the program finds that the all.jpg and generalized_bicubic.jpg images are near duplicates with a cosine similarity score of 79.593%.




