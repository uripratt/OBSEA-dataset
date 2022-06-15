# OBSEA dataset
Full dataset OBSEA with images and annotations

En este respositorio se encuentran las imágenes y sus correspondientes archivos .xml utilizados para entrenar i validar los modelos [Model Mask - RCNN](https://github.com/EnocMartinez/obsea-camera-ml-model1) y [Model YOLO2](https://github.com/EnocMartinez/obsea-camera-ml-model2). Para ver una comparación entre el ajuste de los dos modelos se recomienda mirar el resositorio de [Comparation Model Mask-RCNN vs Model Yolo2](https://github.com/EnocMartinez/obsea-camera-ml-comparison/blob/master/README.md). 

Una vez descargadas ambas carpetas se podran visualizar un total de 4.209 elementos en cada una de ellas (.jpg + .xml). Para ejectuar el modelo es necesario adecuar el directorio de trabajo correspondiente.


###Data organization
Cada imagen tiene un archivo .xml asociado, en el caul cada detección esta reflejada en el archivo con los cuatro vértices (pixel coordenadas). Se encuentra principalmente la siguiente información:
1. Path indormation
2. Image size
3. Object name
4. Detection box



Ejemplo un archivo .xml: 

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

Ejemplo de su imagen correspondiente:


![](C:\Users\uripr\OneDrive\Documentos\UNI_CiTM\SARTI\RCNN_Kangaroo\kangaroo\IMG-TAG\una\DETECT_UNA.png)
![img](https://user-images.githubusercontent.com/106528363/173813419-096a8206-3a37-4b7d-980b-3e2265447c9d.png)
