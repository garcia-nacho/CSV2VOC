# CSV2VOC
Script to convert a CSV file into an XML (VOC based) file to perform YOLOv3 training.

This script is an adaptation of the script [Yolo_to_voc.py](https://gist.github.com/goodhamgupta/7ca514458d24af980669b8b1c8bcdafd) by [goodhamgupta](https://gist.github.com/goodhamgupta).

I have added the following features:

1. It runs in google colab 
2. It accepts csv files
3. It takes the width and height from the csv file instead of from the pictures

The format of the csv files is the following:
<pre><code>object-class-id , center-x , center-y , width , height</code></pre>

The folder containing the files must be in Google Colab and it is declared in the variable <code>ANNOTATIONS_DIR_PREFIX</code> and the folder containing the .xml files it is declared in <code>DESTINATION_DIR</code>. The key for classID-object type is declared in <code>CLASS_MAPPING</code>
