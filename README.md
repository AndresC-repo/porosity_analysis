# porosity_analysis


**Table of Contents**
 * [Installation](#installation)
 * [Project Structure](#Project Structure)

## Installation
Packages used:
-pillow
-albumentations
-cv2
-numpy
-matplotlib.pyplot



## Project Structure

```
├── root_images/                    <<  
│   └── image.tif                   <<  Raw images
│
├── [main.py]/                       <<  Main code of the project
│
├── ---results/                       <<  Creates individual folders for every image
|    └── Original.jpg                     <<  Original image with the useless bottom cut
|    └── median_filter.jpg                <<  Original - median filter
|    └── THRESH_BINARY.jpg                <<  median filter -> Otsu  *** USED
|    └── Adaptive Gaussian Thresh.jpg     <<  median filter -> adaptive guass trsh
|    └── Adaptive Mean Thresh.jpg         <<  median filter -> adaptive mean trsh
|    └── Distance Transform.jpg           <<  THRESH_BINARY -> distance_transform
|    └── overlay.jpg                      <<  Tresh_binary + original
|    └── bin_cirlces.jpg                <<  Sets circles on the inverse of the Binary_image using the distance transform as reference
|    └── support_bin_circles.jpg                <<  Support image to show how it works
|    └── histogram media_filter.png                <<  Pixel histogram of median filter img
|    └── histo_rad_circles.png                <<  Creates individual folders for every image
|    └── radius.txt                    <<  list of radius of cicles created
|
└── .gitignore                      <<  To personalize what is uploaded into the Git
