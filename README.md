# Qupath Initiation

![Qupath](https://user-images.githubusercontent.com/127110867/230375253-a976740b-cfd1-4065-9acd-0246424c009a.png)


For more informations about QuPath consult the website "https://qupath.readthedocs.io/en/stable/index.html" or watch the videos in Youtube "https://www.youtube.com/c/QuPath"

## Use of QuPath (version 0.4.1)
### Create a project 
  - Press "Create project"   
  ![image](https://user-images.githubusercontent.com/127110867/230054393-01c82036-e607-47db-9ea3-22c7c3a20cd8.png)

  - Create an empty directory
  - Select the image format compatible with Bioformat : use only 2D image in fluorescence or coloration. Z stack images are readeable but can be processed only slice by slice with specific script
  - Select the images with "Add images" or drag and drop directly the images in the software. 
   - By double-clicking on the selected image, a "set image type" window opens. Select the appropriate image type ("fluo","HE",..).
   - To reopen the project, click on "open project" and select "project.qpproj" or drag and drop the project files directly into the sofware. You can also affiliate the file to QuPath with the option "open with". If you lose all the data in your file it is possible to recover them with "project.qpproj.backup". 
  - You can move the directory of your project, if the images are in the directory of your project, you will have to update the URL of the image which is displayed in red in the "Image" tab, just double click it to update it. 
By right-clicking on the image, you can open, delete or rename it. You can also add notes using the "Edit Description" function. Or create a folder with the name of the starting image using the "Sort By" -> "URI" option.  
  ![image](https://user-images.githubusercontent.com/127110867/230065394-cdaca62a-abb2-4c83-87f2-aa5f87f8f94c.png)


### Properties of the image 
The "image" tab allows you to see the properties of the image. Like the name, the file, the pixel size, the dimensions...  
![image](https://user-images.githubusercontent.com/127110867/226386290-bebeb45d-d614-4bba-ad70-cad681297709.png)

    Image specific keys 
![image](https://user-images.githubusercontent.com/127110867/226399645-1c918eef-aac2-47e7-b616-dce61f7b54d7.png) : Allows you to make the left interface appear or disappear  

![image](https://user-images.githubusercontent.com/127110867/226399716-1dd33d56-df0f-4f32-be40-af8d9adabc6c.png) : Allows you to move image in all directions. You can also use the mouse scroll wheel for zooming. 
    
![image](https://user-images.githubusercontent.com/127110867/225261236-ef56c90d-59b7-4d97-9fd8-54679f882eee.png) : Select the channels and their brightness/contrast. You can change the channel name by double-clicking on the top or by using a script.   
![image](https://user-images.githubusercontent.com/127110867/230066475-06620c57-5bef-4429-99b4-543724616673.png)
- Write the channel name as a "notepad or word" on the separate line. 
- Copy the lines and select all channels at once and press "Clrl+V"  
 ![image](https://user-images.githubusercontent.com/127110867/230362762-dd2ebdd9-ca40-412d-be3f-8e95b3429b41.png)

- In the "Annotation" tab, there are classes, you can press the three small dots at the bottom right of the column and select "Populate from image channels" to create classes names from your channel.  
-  The initial names of the channels are not lost, if you press the "Image" tab, and double-click on "Metadata changed" you can reset the names back.   

-  To get the optimal intensity, you can play with "Min display" or "Max display". The "Gamma" allows you to amplify low intensity signal.   

![image](https://user-images.githubusercontent.com/127110867/225269648-0ed7deef-2f6e-4a9c-9019-e91c26d1869e.png) : 
By pressing this key, you can see the whole image and freeze it. If you want to move again or to zoom, you have to press the button again.

![image](https://user-images.githubusercontent.com/127110867/225281398-47464a56-647b-42b4-910f-fc3ad5663623.png) : Display the overview image in the top right corner.

![image](https://user-images.githubusercontent.com/127110867/225281522-1ce29af9-3e88-4e91-8889-80f8c341fe09.png) : Displays the position and intensity of the mouse position in the lower right corner.

![image](https://user-images.githubusercontent.com/127110867/225281613-2a539c11-ecd3-4e1a-b202-817096315fe0.png) : Displays the measurement scale in the lower left corner. 

![image](https://user-images.githubusercontent.com/127110867/225281688-6033bcc0-51d6-4e9e-b351-9ce8a1a5c003.png) : Positioning a grid over the entire image.

![image](https://user-images.githubusercontent.com/127110867/225286726-b4f89fe2-3d68-4132-bffa-ffa1b4f1312d.png) : Set software preferences (live width detection...).
 
### Create annotations 

By default, Qupath work only on current/selected annotation. If you want to create a full image annotation, you can use enter ctrl maj A.

There are 3 different objects created in this software: **annotation** (region of tissue); **detections** which are a mask (nucleus or whole cell depending which channel you process) ; and **cells** which is a mask of the whole cell containing three compartments : nucleus, cytoplasm (or membrane) and the whole cell.

The "Annotation" tab allows you to see the annotations you have created. To change the name and colour of the annotation, simply right-click on the annotation and click on "Set Properties". On the right side of the toolbar you see different classes defined by default. The class "None/Unclassified" shows the unclassified cells (by default) and "Ignore" is the class corresponding to the unclassified objects (below the threshold) after the classification process. You can add classes corresponding to cell classes (LT, LB,..) or annotation classes (tumour, follicles). You can also "lock" the annotation so that it cannot be modified.   
When you select an annotation and a class and then click on "Set class", your annotation will belong to this the class.   
With the three dots you can Add or remove an annotation, remove all the annotation except those used, export the channel name, or show/hide the classe selected (space bar can do it).  
![image](https://user-images.githubusercontent.com/127110867/230066173-f749036a-c0a7-4db6-b3b8-3c681ae2470e.png)
 
    Annotation function keys
![image](https://user-images.githubusercontent.com/127110867/226398948-cc645e65-dfe3-44aa-80e4-35070b59821d.png) : Draws a rectangle annotation. (This annotation is saved in the "Annotation" tab). When this annotation is yellow, you can move it, but when it is red, you cannot move it unless you double-click inside. 

![image](https://user-images.githubusercontent.com/127110867/225034022-d21ac8d4-e381-4457-9b5b-6296d10e304b.png) : Ellipse annotation.

![image](https://user-images.githubusercontent.com/127110867/225034273-7302a61f-910a-4fbd-83e4-b416bfe131eb.png) : Create a line 

![image](https://user-images.githubusercontent.com/127110867/225035326-06cddf99-5d66-417c-8833-545ebf57a0bf.png) :
Create a polygon. Double-click when finished. 

![image](https://user-images.githubusercontent.com/127110867/225035459-4458d2f8-65a4-4634-8690-ed1b44f5b3ba.png) : Creat a polyline annotation, either by clicking individual points (with double-click to end) or clicking and dragging

![image](https://user-images.githubusercontent.com/127110867/225037603-e83a92da-da25-458b-9166-1e46f2a8f5b5.png) : Create an area with rounded corners. When you draw a large circle, you can fill inside the circle.

![image](https://user-images.githubusercontent.com/127110867/225038422-82a158ee-5c79-4edc-abf8-20034fe97cd1.png) : Click and drag to draw with a wand tool. Adjust brightness/contrast or wand preferences to customize the sensitivity and behavior, (wand sensitivity or smoothing).

![image](https://user-images.githubusercontent.com/127110867/225042065-a328453b-71b6-4c0b-a0ec-a6faa4406495.png) : Count mannuly cells of the same class. If you want to count cells of another class, you can press "Add". You can save the list of points.

![image](https://user-images.githubusercontent.com/127110867/225261165-fa603c30-9744-474b-a909-863e4b67cec7.png) : When this option is selected, it allows the protection of pre-excited annotations and prevents the creation of other annotations.

The three dots or right click on annotation have different functions: 
  - Unlock: allows the annotation to remain unchanged 
  - Insert in hierarchy: the annotation is integrated into another annotation (if inside).  
  - Edit single: "Make inverse" allows to create a complementary annotation of a child annotation from the parent annotation 

![image](https://user-images.githubusercontent.com/127110867/230067724-d06f6db4-7964-4eea-99a9-40a059130c58.png)

When several annotations are selected, a new function is available: "Edit multiple" :
  - Merge selected : merge the annotations 
  - Substract selected : allows you to substract two annotations (take care in which order you select annotations)

![image](https://user-images.githubusercontent.com/127110867/226577083-9dc93d6d-025a-4ec8-9391-449f8c945b53.png)  ![image](https://user-images.githubusercontent.com/127110867/226581247-986ce506-f962-4653-b2d1-180e8294db99.png)

  - Intersect selected : only the region in common will remain

![image](https://user-images.githubusercontent.com/127110867/226576846-9a36c657-31c3-4a82-8283-19842872583d.png)  ![image](https://user-images.githubusercontent.com/127110867/226576945-36b79b87-f3ed-4700-94d6-bf981fd263d0.png)

*Note :*  Ctrl Z will reset the last operation

### Visualisation of the object hierarchy 
The "Hierarchy" tab displays the different object hierarchies, the number of objects present in the different annotations and the object class:  
A region included in another region is considered a child annotation. Resolving the hierarchy creates the hierarchy between the annotations   
  ![image](https://user-images.githubusercontent.com/127110867/230376007-f88a35d4-43c8-45e5-bd41-7ba7c5211368.png)


### Workflow 
The "Workflow" tab allows you to see the different functions used during your session. You can create a script with the different options.

   

## Command menu

#### File

  - Recent project : Open the recent project 
  - Save : It is important to save your project every time, when you change the image you get a message to save
  - Export snapshot (main window content)
  - Import objects and export objects (annotation, detections) in format Geojson

#### Edit  
  - Undo (Ctrl Z) 
  
#### Tools 
  - As in toolbar
  
#### View 
  - Multiview : Insert columns or rows to view images at the same time, you can also do this with a right-click
  - "Show channel viewer" allows you to see the different channels at the same time but separately 
  - "Rotate image" allows you to rotate the image  
  - Select what you want to see when there is a cells detection "Cell display - Nuclei only - Nuclei and cell boundaries - Centroids only", you can also do this with a right-click
  
   
#### Object
  - Delete all the selected object or just annotation and detection
  - Select object by class
  - In the option "Annotation" you can do more  :  
      -"Specify annotation" : Create annotation (rectangle or eclipse) with your own mesure  
      -Insert into hierarchy just the selected annotation, or resolve hierarchy of all annotations  
      -Duplicate or expand/erode an annotation  
      -Merge annotation together or split   
      -Modify the shape with "Simplify shape" by creating a polygon

#### Measure 
  - "Show measurements map " : Assign a colour to cells or detections for measurements (area, distance,...)  
  ![image](https://user-images.githubusercontent.com/127110867/230372071-3c8c5287-1b31-4fe2-b416-66852dd0db01.png)

  - "Show measurement manager" : Choose the parameters to measure
  - Show annotation measurements or detection measurements 
  - "Grid views" -> "Annotation grid summary wiew" : See the differents annotations, and the number of detection inside 

  - **"Export measurement"** :  export the annotations or detections measurements in csv
![export measurement](https://user-images.githubusercontent.com/127110867/230373940-fb8e953c-fb67-4b2d-b8d7-172feb9675e9.png)


#### Automate
  - "Show script editor" :  create a script or drag and drop an already created script   ![image](https://user-images.githubusercontent.com/127110867/230374946-8d89b8a8-cce4-48b1-9c93-52e3af293616.png)
  - You can also import a script directly into the software or drag and drop. Some script need extansion programme in Java. Jar file can also be dragged and drop and will be installed in the extension folder.
  - The "Run in project" function allows to run the script on all your images. 

#### Analyse 
  - "Cell detection" : you can create detections or cells (cell expansion > 0)

![cell detection](https://user-images.githubusercontent.com/41480459/230610270-1e9e0e9c-6b82-4a66-9228-8cfa19133599.png)

    - "Positive cell detection" : create cells that belong to the "Positive" class
    - "Subcellular detection" : detection of subcellular objects in cells
  -  Spatial analysis (distance cells to annotation,..)

![Clipboard](https://user-images.githubusercontent.com/41480459/230606533-4152a14c-891a-4a1b-aa85-fc2feccfd6e2.jpg)
  - Create a "Density maps" from detections and finally an annotations by thresholding the maps  
 
![Clipboard](https://user-images.githubusercontent.com/41480459/230608511-e37bc41c-fbe2-4b09-8e1e-0c17b37efe13.jpg)


#### Classify 
  - "Object classification" : Allows to classify detections/cells  
  ![Clipboard](https://user-images.githubusercontent.com/41480459/225030223-4162f204-68ed-47c1-835b-16a492d86a57.jpg) 
  - "Pixel classification" : train pixel classifier or pixel thresholder to create automaticaly annotations
![image001](https://user-images.githubusercontent.com/41480459/225047518-e8cf9565-b953-401a-845e-93a6722d4571.png)

![Clipboard](https://user-images.githubusercontent.com/41480459/230612705-55136436-9bcf-4737-91a0-dba5908423b9.png)


#### Extensions 
  - Combined extensions with QuPath like Cellpose 

#### Help 
  - Documentations









    Fonctionnel keys  

![image](https://user-images.githubusercontent.com/127110867/225270911-3d6aaa16-1e73-40fe-89f9-007b77ae10d8.png) : Shows only the selected annotation(s).

![image](https://user-images.githubusercontent.com/127110867/225271644-87dd7076-f335-4b6c-b190-e256515e4c8c.png) : 
Displays the name of the annotations. To name an annotation, you need to go to the "Annotation" tab and double-click on the annotation, then select "Set properties" and change the name. 

![image](https://user-images.githubusercontent.com/127110867/225273685-638fe595-c9f0-46ef-8269-c63bd4051b67.png) : Shows the TMA grid in the viewer.

![image](https://user-images.githubusercontent.com/127110867/225278991-be528b5c-0e8e-405f-80f3-bb9e4ff9e7e2.png) : Shows the contours detections or cells.

![image](https://user-images.githubusercontent.com/127110867/225279318-a434b7cb-1fea-47ce-ac3d-0156965aa7d9.png) : Fills in detections or cells.

![image](https://user-images.githubusercontent.com/127110867/225280507-b4a1c82c-52ef-4192-b15b-cc1074f8a6d9.png). Shows pixels classification in the overlay.

![image](https://user-images.githubusercontent.com/127110867/225280131-33b778e0-7887-49eb-b304-72ff20fa8e01.png) : overlay opacity (detections,..).

![image](https://user-images.githubusercontent.com/127110867/225280759-1ab602c2-45b3-4875-9acd-73678fd019d8.png) : To view measurements of TMAs, annotations or detections and also histogram, save in "txt".  
![image](https://user-images.githubusercontent.com/127110867/230372909-96b3e056-8a76-4b5e-b06d-64e7230fdf1a.png)
















      Shortcut keys  
- When you click into (1,2,3...) you can choose the channel
- When you click into top or down arrow you can choose the Z-stack 
- When you click into a letter you can choose the type of annotation : 

![image](https://user-images.githubusercontent.com/127110867/225045509-a3103c7b-ea3b-49a4-8c49-fb5c7f2fa941.png)   

ALT Key : 
- When the Move tool is selected, use the Alt key to click on multiple objects to select them.
- When the Brush or Wand tools are selected, use the Alt key to switch to 'eraser' mode when drawing

Shift Key :
- When the Brush or Wand tools are selected, use the Shift key to continue adding to an existing selected annotation (rather than creating a new one).

![image](https://user-images.githubusercontent.com/127110867/225048760-5512b02f-1afe-4678-add6-98f66dc8db72.png) ![image](https://user-images.githubusercontent.com/127110867/225048877-c990f570-dd8b-4d81-b650-54ddb3eb9624.png)


