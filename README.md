# JICE
Joint Image Compression and Encryption algorithms

The project implements an image encryption process that involves compressing an image using K-means clustering, applying encryption techniques, and analyzing various metrics such as compression ratio, NPCR (Number of Pixel Changing Rate), and UACI (Unified Average Changing Intensity). Let's summarize the key components and processes involved:

## Image Loading and Preprocessing:

The code starts by loading the original compressed image and extracting its pixel data. The image is then preprocessed to initialize variables and arrays for further processing.
Compression using K-means Clustering:

K-means clustering is applied to compress the image by reducing the number of colors. The algorithm clusters similar colors together and represents each cluster by its centroid color. This reduces the number of colors in the image while preserving its visual quality.
Encryption Process:

The encryption process involves modifying pixel values based on specific patterns and shuffling the pixels using a predefined algorithm and RC4 key. While the exact implementation of RC4's PRGA and KSA is not explicitly present, the code performs a permutation of pixel indices based on the provided key and specific patterns within the image data.
Analysis and Metrics Calculation:

## After encryption, various metrics are calculated to evaluate the effectiveness of the encryption process:
Compression Ratio: The ratio of the original image size to the compressed image size is calculated to measure the level of compression achieved.
NPCR (Number of Pixel Changing Rate): This metric compares the pixel values of the original image with the encrypted image. A high NPCR value indicates a significant change in pixel values, which is desirable for encryption.
UACI (Unified Average Changing Intensity): This metric measures the average intensity change between corresponding pixels of the original and encrypted images. It provides insight into the overall level of encryption achieved.
Visualization and Comparison:

The code visualizes the original, compressed, encrypted, and decrypted images using matplotlib. This allows for a visual comparison of the image quality and encryption effectiveness.
Size Calculation and File Saving:

The code calculates the sizes of the original, compressed, encrypted, and decrypted images and prints them for analysis.
The encrypted and decrypted images are saved to files for further examination.
In summary, the provided code implements an image compression and encryption process using K-means clustering and custom encryption techniques. It evaluates the effectiveness of encryption using various metrics and provides visual comparisons of the original and processed images. While the exact encryption algorithm used is not explicitly stated, the code demonstrates the application of compression, encryption, and analysis techniques for image data.
