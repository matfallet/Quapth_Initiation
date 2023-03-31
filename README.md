# Qupath_Initiation

For more informations about QuPath consult the website "https://qupath.readthedocs.io/en/stable/index.html" or watch the videos in Youtube "https://www.youtube.com/c/QuPath"

## Use of QuPath (version 0.4.1)
### Create a project 
  - Press "Create project" 
  - Create an empty directory
  - Image format (compatible with Bioformat) : use only 2D image in fluorescence or coloration. Z stack images are readed but can be processed only slice by slice with specific script
  - Selection the images with "Add images" or drag and drop directly the images in the software. 
   - By double-clicking on the selected image, a "set image type" window opens. Select the appropriate image type ("fluo","HE",..).
   - To reopen the project, click on "open project" and select "project".qpproj or drag and drop the project files directly into the sofware. You can also affiliate the file to QuPath with the option "open with". 

When you right-click on the image, you can open, delete or rename it. You can also add notes using the "Edit description" function. Have the name of the mask image, or create files with the name of the starting image.   
![image](https://user-images.githubusercontent.com/127110867/226588395-bba3dacf-1038-4308-80c6-0b98c8c6a647.png)


### Properties of the image 
The "image" tab allows you to see the properties of the image. Like the name, the file, the size, the dimensions...  
![image](https://user-images.githubusercontent.com/127110867/226386290-bebeb45d-d614-4bba-ad70-cad681297709.png)

    Image specific keys 
![image](https://user-images.githubusercontent.com/127110867/226399645-1c918eef-aac2-47e7-b616-dce61f7b54d7.png) : Allows you to make the left tools bar appear or disappear  

![image](https://user-images.githubusercontent.com/127110867/226399716-1dd33d56-df0f-4f32-be40-af8d9adabc6c.png) : Allows you to move image in all directions. You can also use the mouse scroll wheel for zooming. 
    
![image](https://user-images.githubusercontent.com/127110867/225261236-ef56c90d-59b7-4d97-9fd8-54679f882eee.png) : Select the channels and their brightness/contrast. You can change the channel name by double-clicking on the top or by using a script.   
- Write the channel name as a "notepad or word" on the separate line. 
- Copy the lines and select all channels at once and press "Clrl+V"  
![image](https://user-images.githubusercontent.com/127110867/225262038-e164f93b-8b36-4ad5-87c5-087996baed33.png) ![image](https://user-images.githubusercontent.com/127110867/225263469-21f7d51a-f7fb-40c2-a2be-10d4bf263a9f.png)

- In the "Annotation" tab, on the right hand side, the channels name are in the column. If this is not the case, you can press the three small dots at the bottom right of the column and select "Populate from image channels".  
-  The initial names of the channels are not lost, if you press the "Image" tab, and double-click on "Metadata changed" you can reset the names back.   

-   To get the optimal intensity, you can play with the min and max bar of the graph.You can also use "Min display" or "Max display". The "Gamma" allows you to amplify low intensity signal.   
![image](https://user-images.githubusercontent.com/127110867/225268944-dd1a1a41-9899-412c-a72d-3207c6bf7415.png) ![image](https://user-images.githubusercontent.com/127110867/225268978-dad7ba74-91f8-4e5a-b69f-1e37d028b03c.png)

![image](https://user-images.githubusercontent.com/127110867/225269648-0ed7deef-2f6e-4a9c-9019-e91c26d1869e.png) : 
By pressing this key, you can see the whole image and freeze it. If you want to move again or to zoom, you have to press the button again.

![image](https://user-images.githubusercontent.com/127110867/225281398-47464a56-647b-42b4-910f-fc3ad5663623.png) : Display the overview image in the top right corner.

![image](https://user-images.githubusercontent.com/127110867/225281522-1ce29af9-3e88-4e91-8889-80f8c341fe09.png) : Displays the position and intensity of the mouse position in the lower right corner.

![image](https://user-images.githubusercontent.com/127110867/225281613-2a539c11-ecd3-4e1a-b202-817096315fe0.png) : Displays the measurement scale in the lower left corner. 

![image](https://user-images.githubusercontent.com/127110867/225281688-6033bcc0-51d6-4e9e-b351-9ce8a1a5c003.png) : Positioning a grid over the entire image.

![image](https://user-images.githubusercontent.com/127110867/225286726-b4f89fe2-3d68-4132-bffa-ffa1b4f1312d.png) : Set software preferences.
 
### Create a annotation 

*Note :* 
By default, Qupath work only on current/selected annotation. If you want to create a full image annotation, you can use enter ctrl maj A.

There are 3 different objects created in this software: **annotation** (region of tissue or others); **detections** which is a mask (nucleus or whole cell depending which channel you process) ; and **cells** which is a mask of the whole cell containing three compartments : nucleus, cytoplasm (or membrane) and the whole cell.

The "Annotation" tab allows you to see the created annotations. To change the name and colour of the annotation, simply right-click on the annotation and press "Set Properties". On the right hand side of the toolbar you see different classes defined by default. Class "None", shows  unclassified cells (by default) and "Ignore", is the class corresponding to unclassified objects (below threshold) after classification process. You can add class corresponing to cell classes (LT, LB,..) or annotations classes (tumor, folicles). 
When you select an annotation and a class and then click on "Set class", your annotation will belong to this the class. 
With the three dot you can Add or remove an annotation, remove all the annotation except those used, export the channel name, or show/hide the classe selected (space bar can do it).  
![image](https://user-images.githubusercontent.com/127110867/226393521-72e82183-e2fc-4cd7-8aae-db278aa4cb96.png)
 
    Annotation function keys
![image](https://user-images.githubusercontent.com/127110867/226398948-cc645e65-dfe3-44aa-80e4-35070b59821d.png) : Draws a rectangle annotation. (This annotation is saved in the "Annotation" tab). When this annotation is yellow, you can move it, but when it is red, you cannot move it unless you double-click inside. 

![image](https://user-images.githubusercontent.com/127110867/225034022-d21ac8d4-e381-4457-9b5b-6296d10e304b.png) : Ellipse annotation.

![image](https://user-images.githubusercontent.com/127110867/225034273-7302a61f-910a-4fbd-83e4-b416bfe131eb.png) : Create a line 

![image](https://user-images.githubusercontent.com/127110867/225035326-06cddf99-5d66-417c-8833-545ebf57a0bf.png) :
Create a polygon. Double-click when finished. 

![image](https://user-images.githubusercontent.com/127110867/225035459-4458d2f8-65a4-4634-8690-ed1b44f5b3ba.png) : Creat a polyline annotattion, either by clicking individualpoints (with double-click to end) or clicking and dragging

![image](https://user-images.githubusercontent.com/127110867/225037603-e83a92da-da25-458b-9166-1e46f2a8f5b5.png) : Create an area with rounded corners. When you draw a large circle, you can fill in the inside of the circle.

![image](https://user-images.githubusercontent.com/127110867/225038422-82a158ee-5c79-4edc-abf8-20034fe97cd1.png) : Click and drag to draw with a wand tool. Adjust brightness/contrast or wand preferences to customize in the sensitivity and behavior. 

![image](https://user-images.githubusercontent.com/127110867/225042065-a328453b-71b6-4c0b-a0ec-a6faa4406495.png) : Allows you to count the cells of the same class. If you want to count cells of another class, you can press "Add" in the window that opened when you started selecting cells. You can save the list of points to a file for future reference.

![image](https://user-images.githubusercontent.com/127110867/225261165-fa603c30-9744-474b-a909-863e4b67cec7.png) : When this option is selected, it allows the protection of pre-excited annotations and prevents the creation of other annotations.

The three dots have different functions: 
  - Unlock: allows the annotation to remain unchanged 
  - Insert in hierarchy: the annotation is integrated into another annotation (if inside).  
  - Edit single: "Make inverse" allows to create a complementary annotation of a child annotation from the parent annotation 

![image](https://user-images.githubusercontent.com/127110867/226573034-495a7b90-7447-472f-a157-6736a02cf855.png)

When several annotations are selected, a new function is available: "Edit multiple" :
  - Merge selected : merge the annotations 
  - Substract selected : allows you to substract two annotations (take care in which order you select annotations)

![image](https://user-images.githubusercontent.com/127110867/226577083-9dc93d6d-025a-4ec8-9391-449f8c945b53.png)  ![image](https://user-images.githubusercontent.com/127110867/226581247-986ce506-f962-4653-b2d1-180e8294db99.png)

  - Intersect selected : only the region in common will remain

![image](https://user-images.githubusercontent.com/127110867/226576846-9a36c657-31c3-4a82-8283-19842872583d.png)  ![image](https://user-images.githubusercontent.com/127110867/226576945-36b79b87-f3ed-4700-94d6-bf981fd263d0.png)

*Note :*  Ctrl Z will reset the last operation

### Visualisation of the object hierarchy 
The "Hierarchy" tab allows you to display the different object hierarchies, the number of the object present in the different annotations, the classifier affiliated to the object...

### Workflow 
The "Workflow" tab allows you to see the different functions used during your session. You can create a script with the different options.

   

## Command menu

#### File
  - Project : Same function as the operational tabs 
  - Recent project : Open the recent project 
  - Save : It is important to save your project every time, when you change the image you get a message to save. 
  - Import and export some files......

#### Edit  
  - Copy to clipboard : Do some screenshots of just the software (main window screeshot) or the entire computer screen (full screenshot) 
  
#### Tools 
  - Functionnal keys 
  
#### View 
  - You can see the recent commands 
  - "Show channel viewer" allows you to see the different channels at the same time but separately 
  - "Rotate image" allows you to rotate the image  
  - Select what you want to see when there is a cells detection "Cell display - Nuclei only - Nuclei and cell boundaries - Centroids only", you can also do this with a right-click
  - After there is a fonctionnel keys 
  
   
#### Object
  - Delete all the selected object or just annotation and detection
  - Select object 
  - Lock or unlock the object 
  - In the obtion "Annotation" you can do more thing :
      - "Specify annotation" : Create annotation (rectangle or eclipse) with your own mesure
      - Insert into hierarchy just the selected annotation, or resolve hierarchy of all annotation
      - Rotate your annotation with "transform annotations". 
      - Duplicate or expand a annotation. 
      - Merge annotation togother 
      - Modify the shape by adding points with "Simplify shap"

#### Measure 
  - "Show measurement manager" : Choose what do you want to see during the measurement
  
    ![image](https://user-images.githubusercontent.com/127110867/228238971-70d11fbb-4b74-4021-8ca5-ce2bb0d409c6.png)
  - Show annotation measurements or detection measurements 
  - "Grid views" -> "Annotation grid summary wiew" : allows  you to see the differents annotations, and the number of detection inside  ![image](https://user-images.githubusercontent.com/127110867/228241476-b678031d-cc49-4e58-870d-098378ce232d.png)

  - "Export measurement" : allows you to export the information of the image 
  - "Show measurement maps": ... 

#### Automate
  - "Show scrip editor" : allows you to create a script or drag and drop an already created script   ![image](https://user-images.githubusercontent.com/127110867/228241890-b8873e8a-e40d-4775-b733-69c4734ec771.png)
  - "Script interperter" : ...
  - "Show workflow command history" : allows you to create a script from your workflow by selecting or keeping all functions already used during your session
  - You can also import scrip directly in to the software 

#### Analyse 
  - "Cell detection" : you can create cells or a detection of the channel you want
      - "Positive cell detection" : create a cell affiliated to the "Positive" class
      - "Subcellular detection" : detection of another channel in the cytoplasm of the cell 
  - 
  - Create a "Density maps" : like a Heatmap 

#### Classify 
  - "Object classification" : Allows to classify or name a object
  - "Pixel classification" : Allows to classify some pixels 
  - 

#### Extensions 
  - Combined extensions with QuPath like Cellpose 

#### Help 
  - All the website for helping you 


    Fonctionnel keys   

![image](https://user-images.githubusercontent.com/127110867/225270911-3d6aaa16-1e73-40fe-89f9-007b77ae10d8.png) : Shows only the selected annotation(s).

![image](https://user-images.githubusercontent.com/127110867/225271644-87dd7076-f335-4b6c-b190-e256515e4c8c.png) : 
Displays the name of the annotations. To name an annotation, you need to go to the "Annotation" tab and double-click on the annotation, then select "Set properties" and change the name. 

![image](https://user-images.githubusercontent.com/127110867/225273685-638fe595-c9f0-46ef-8269-c63bd4051b67.png) : Shows the TMA grid in the viewer.

![image](https://user-images.githubusercontent.com/127110867/225278991-be528b5c-0e8e-405f-80f3-bb9e4ff9e7e2.png) : Shows the contours detections or cells.

![image](https://user-images.githubusercontent.com/127110867/225279318-a434b7cb-1fea-47ce-ac3d-0156965aa7d9.png) : Fills in detections or cells.

![image](https://user-images.githubusercontent.com/127110867/225280507-b4a1c82c-52ef-4192-b15b-cc1074f8a6d9.png). Shows pixels classification in the overlay.

![image](https://user-images.githubusercontent.com/127110867/225280131-33b778e0-7887-49eb-b304-72ff20fa8e01.png) : overlay opacity (detections,..).

![image](https://user-images.githubusercontent.com/127110867/225280759-1ab602c2-45b3-4875-9acd-73678fd019d8.png) : Allows you to view measurements of TMAs, annotations or detections. 
















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


