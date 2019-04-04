# Semantic Structure Identification using Image Detection Algorithms <br>
~~~
#Python #TensorFlow #DeepLearning #UnsupervisedLearning #Tesseract #OpenCV
~~~
Project Paper - https://www.dropbox.com/s/q4ssacdievrmu52/Semantic%20Structure%20Identification%20using%20Image%20Detection%20Algorithms.docx?dl=0 <br>

Project Poster - https://www.dropbox.com/s/az6d160ao9zcv09/Informs%20BA%20Table%20Cell%20Detection%20Poster.pptx?dl=0 <br>

## Abstract <br>

In this project, we aim to develop a tool capable of identifying useful semantic structures from various file formats such as PDFs, images, etc. The tool attempts to identify cells of semantic continuity(e.g., table cells)within files using Image recognitionand table identification from images. The tool will first convert each page of the document to an image in order to detect these cells. The second stage will detect semantic structures and linkages within the data (such asdata presentin tables).To perform the task described in the previous paragraph, we collected over 400 PDF files that contain textual as well as tabular data. These files are used in our model as part of the training data. Thesefiles are converted to JPEG format using OpenCV.Toolssuch as PyTesseract are used to identify cells and create bounding boxes around them, andMachine Learning/Artificial Intelligence frameworks such as TensorFlow and Luminoth are utilized to extract tables from the images by training deep learning algorithms. Finally, arrays of these bounding boxes are analyzed to detect semantic structures.

Below are the procedures to follow to achieve individual goals in this stepwise approach:

Table Detection 1.)	You will need to install cv2 and luminoth for this 2.)	To add new images for classification, add them in the images folder 3.)	To get these images trained, you will need to record the table coordinates and add them to the Train.csv file 4.)	If there are multiple tables in an image, you need to add separate rows for the table cells with the same image_id 5.)	The Table Detection code was run on Google Colab for GPU utility and so the folders are named according to that. When it’s run locally, you can replace the “content/” path with the path of the folder in which you’ve placed the data 6.)	A variable has been created to store the predicted table details of the algorithm and write it into a file

Table Cell Detection 1.)	You will need to Install Pytesseract,OpenCv 2.)	For this, the images are placed in the TCD folder and their table coordinates are obtained from the train.csv file 3.)	To change the file you’re using, you will need to replace train.csv with a similar structure file which has the table coordinates. As generated from the Table Detection code 4.) Once the coordinates are obtained and the word boxes are generated, we use K-means clustering to obtain the columns and then the cells are obtained by comparing the Y coordinates
