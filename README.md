<h1>BlodectCV</h1>

<h3>A tool for the detection and classification of blood cells</h3>

**Problem Statement**

A complete blood cell count is an important test in medical diagnosis to evaluate overall health condition. Traditionally blood cells are counted manually using haemocytometer along with other laboratory equipment's and chemical compounds, which is a time-consuming and tedious task. 

**Solution**

A computer aided sytem that detects and classifies the bloods cells from the microscopic images fed into it.

**MVP**

An online website that enables medical professionals upload microscopic images of blood containing different types of blood cells. Once the image is uploaded, the image is be fed into a model that detects and classify the blood cells present in the image.
xeguV.jpeg
After successful processing of the image, the following output is  displayed on the website along with the image maked with bounding boxes representing different types of cells:

🔴 Number of red blood cells 

⚪ Number of white blood cells

🟡 Number of platelets

**Working**

In this project, a technique for automatic identification and counting of three types of blood cells using ‘you only look once’ (YOLO) object detection and classification algorithm is used. 
YOLO framework has been trained with a BCCD Dataset of blood smear images to automatically identify and count red blood cells, white blood cells, and platelets. 
Moreover, this project employed state of the art CNN architectures considering architecture complexity, reported accuracy, and running time with this framework and compare the accuracy of the models for blood cells detection. 
Overall the computer-aided system of detection and counting enables us to count blood cells from smear images in less than a second, which is useful for practical applications.

**Dataset**

Roboflow BCCD dataset: Dataset of blood smear images 
There are 364 images across three classes: WBC (white blood cells), RBC (red blood cells), and Platelets

**Shortcomings**

* This project primarily focuses only on three types of blood cells.
* The BCCD dataset used in the project is not uniform.
    * WBC’s and platelets are under represented
    * RBC’s are over represented

**Future scope**

The project yields a great potential. It can be improved to be used to detect other types of cells found in the blood. It can be extended further to detect the abnomalities in the different types of cells. A good improvement would be to detect cancer cells in the blood.
