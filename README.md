# OBSEA dataset
Full dataset OBSEA with images and annotations

In this repository you can find the full dataset OBSEA with images and their corresponding annotations (.xml files) used to train and validate the [Model Mask - RCNN](https://github.com/EnocMartinez/obsea-camera-ml-model1) and [Model YOLO2](https://github.com/EnocMartinez/obsea-camera-ml-model2) models. To see a comparison between the fit of the two models it is recommended to look at the [Comparison Model Mask-RCNN vs Model Yolo2](https://github.com/EnocMartinez/obsea-camera-ml-comparison/blob/master/README.md) repository. 

Once both folders have been downloaded, a total of 4,209 elements can be viewed in each folder (.jpg + .xml). To run the model it is necessary to adapt the corresponding working directory.


### Data organization
Each image has an associated .xml file, in which each detection is reflected in the file with the four vertices (pixel coordinates). Mainly the following information is found:
1. Path indormation
2. Image size
3. Object name
4. Detection box



Example of an .xml file: 


```xml
<annotation>
    <folder>2014/cam1</folder>
    <filename>OBSEA140103211704_1186_00.jpg</filename>
    <path>2014/cam1/OBSEA140103211704_1186_00.jpg</path>
    <source>
        <database>Unknown</database>
    </source>
    <size>
        <width>640</width>
        <height>480</height>
        <depth>3</depth>
    </size>
    <segmented>0</segmented>
    <object>
        <name>fish</name>
        <pose>Unspecified</pose>
        <truncated>0</truncated>
        <difficult>0</difficult>
        <bndbox>
            <xmin>-9</xmin>
            <ymin>84</ymin>
            <xmax>280</xmax>
            <ymax>296</ymax>
        </bndbox>
    </object>
```


Example of the corresponding image:


![](C:\Users\uripr\OneDrive\Documentos\UNI_CiTM\SARTI\RCNN_Kangaroo\kangaroo\IMG-TAG\una\DETECT_UNA.png)
![img](https://user-images.githubusercontent.com/106528363/173813419-096a8206-3a37-4b7d-980b-3e2265447c9d.png)


potser posar en el git de comparació els dos models amb un xml i la seva img...
