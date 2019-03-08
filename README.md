# Semantic Structure Identification using Image Detection Algorithms
~~~
#Python #TensorFlow #DeepLearning #UnsupervisedLearning #Tesseract #OpenCV
~~~
Project Paper - https://www.dropbox.com/home/Unicreate/MWDSI?preview=Semantic+Structure+Identification+using+Image+Detection+Algorithms.docx
Project Poster - https://www.dropbox.com/s/az6d160ao9zcv09/Informs%20BA%20Table%20Cell%20Detection%20Poster.pptx?dl=0

### Abstract
In this project, we aim to develop a tool capable of identifying useful semantic structures from various file formats such as PDFs, images, etc. The tool attempts to identify cells of semantic continuity(e.g., table cells)within files using Image recognitionand table identification from images. The tool will first convert each page of the document to an image in order to detect these cells. The second stage will detect semantic structures and linkages within the data (such asdata presentin tables).To perform the task described in the previous paragraph, we collected over 400 PDF files that contain textual as well as tabular data. These files are used in our model as part of the training data. Thesefiles are converted to JPEG format using OpenCV.Toolssuch as PyTesseract are used to identify cells and create bounding boxes around them, andMachine Learning/Artificial Intelligence frameworks such as TensorFlow and Luminoth are utilized to extract tables from the images by training deep learning algorithms. Finally, arrays of these bounding boxes are analyzed to detect semantic structures.
