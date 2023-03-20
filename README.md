# Qupath_Initiation
cluster/phenotyping/interaction

For more informations about QuPath consult the website "https://qupath.readthedocs.io/en/stable/index.html" or watch the videos in the plateform Github.com "..."

## Use of QuPath (version 0.4.1)
### Create a project 
  - Press "Create project" 
  - Create an empty directory
  - Image format (compatible with Bioformat)
  - Selection the images with "Add images" or drag and drop directly the images in the software. 
   - By double-clicking on the selected image, a "set image type" window opens. Select the appropriate image type ("fluo","HE",..).
   - To reopen the project, click on "open project" and select "project".qpproj or drag and drop the project files directly into the sofware 

### Properties of the image 
The "image" tab allows you to see the properties of the image. Like the name, the file, the size, the dimensions...  
![image](https://user-images.githubusercontent.com/127110867/226386290-bebeb45d-d614-4bba-ad70-cad681297709.png)

    Image specific icon 
![image](https://user-images.githubusercontent.com/127110867/225029024-b802c332-f8c5-473e-a7c0-59e0ba6d2013.png) : Allows you to make the left tools bar appear or disappear  

![image](https://user-images.githubusercontent.com/127110867/225029694-10ee0824-4ace-4c61-9b05-d8ab78472636.png) : Allows you to move image in all directions. You can also use the mouse scroll wheel for zooming. 
    
![image](https://user-images.githubusercontent.com/127110867/225261236-ef56c90d-59b7-4d97-9fd8-54679f882eee.png) : Select the channels and their brightness/contrast. You can change the channel name by double-clicking on the top or by using a script.   
- Write the channel name as a "notepad or word" on the separate line. 
- Copy the lines and select all channels at once and press "Clrl+V"  
![image](https://user-images.githubusercontent.com/127110867/225262038-e164f93b-8b36-4ad5-87c5-087996baed33.png) ![image](https://user-images.githubusercontent.com/127110867/225263469-21f7d51a-f7fb-40c2-a2be-10d4bf263a9f.png)

- In the "Annotation" tab, on the right hand side, the channels name are in the column. If this is not the case, you can press the three small dots at the bottom right of the column and select "Populate from image channels".  
-  The names of the start channels are not lost, if you press the "Image" tab, and double-click on "Metadata changed" you get the start names back.   

Select the channel. To get the optimal intensity, you can play with the mi and max bar of the graph.You can also use "Min display" or "Max display". The "Gamma" allows you to amplify the background signal.   
![image](https://user-images.githubusercontent.com/127110867/225268944-dd1a1a41-9899-412c-a72d-3207c6bf7415.png) ![image](https://user-images.githubusercontent.com/127110867/225268978-dad7ba74-91f8-4e5a-b69f-1e37d028b03c.png)

![image](https://user-images.githubusercontent.com/127110867/225269648-0ed7deef-2f6e-4a9c-9019-e91c26d1869e.png) : 
By pressing this key, you can see the whole image and freeze it. If you want to move again or to zoom, you have to press the button again.

![image](https://user-images.githubusercontent.com/127110867/225281398-47464a56-647b-42b4-910f-fc3ad5663623.png) : Display the overview image in the top right corner.

![image](https://user-images.githubusercontent.com/127110867/225281522-1ce29af9-3e88-4e91-8889-80f8c341fe09.png) : Displays the position and intensity of the mouse position in the lower right corner.

![image](https://user-images.githubusercontent.com/127110867/225281613-2a539c11-ecd3-4e1a-b202-817096315fe0.png) : Displays the measurement scale in the lower left corner. 

![image](https://user-images.githubusercontent.com/127110867/225281688-6033bcc0-51d6-4e9e-b351-9ce8a1a5c003.png) : Positioning a grid over the entire image.

![image](https://user-images.githubusercontent.com/127110867/225286726-b4f89fe2-3d68-4132-bffa-ffa1b4f1312d.png) : Set software preferences.

## Create a annotation 
The "Annotation" tab allows you to see the created annotations in order. To change the name and colour of the annotation, simply right-click on the annotation and press "Set Properties". On the right hand side of the toolbar you see different classes defined by default. The classes can be changed, or deleted, some may be interesting to keep, like "None", which shows the unclassified cells. You can add a classe, beacause when you want define a classe of the cells you need to create a classe before. 
When you select annotation and you click on "Set class", your annotation have the name of the class. 
With the three dot you can Add or remove a annotation, remove all the annotation except those used, export the channel name, or show/hide the classe selected (space bar can do it).  
![image](https://user-images.githubusercontent.com/127110867/226393521-72e82183-e2fc-4cd7-8aae-db278aa4cb96.png)

There are many icon functions to make an annotation: 
    Annotation function icon


![image](https://user-images.githubusercontent.com/127110867/225032103-7ba78885-f2b4-4408-b767-3d04b08d4be7.png) : Draws a rectangle annotation. (This annotation is saved in the "Annotation" tab). When this annotation is yellow, you can move it, but when it is red, you cannot move it unless you double-click inside. 

![image](https://user-images.githubusercontent.com/127110867/225034022-d21ac8d4-e381-4457-9b5b-6296d10e304b.png) : Ellipse annotation.

![image](https://user-images.githubusercontent.com/127110867/225034273-7302a61f-910a-4fbd-83e4-b416bfe131eb.png) : Create a line 

![image](https://user-images.githubusercontent.com/127110867/225035326-06cddf99-5d66-417c-8833-545ebf57a0bf.png) :
Create a polygon. Double-click when finished. 

![image](https://user-images.githubusercontent.com/127110867/225035459-4458d2f8-65a4-4634-8690-ed1b44f5b3ba.png) : Create a segmented or freehand line

![image](https://user-images.githubusercontent.com/127110867/225037603-e83a92da-da25-458b-9166-1e46f2a8f5b5.png) : Create an area with rounded corners. When you draw a large circle, you can fill in the inside of the circle.

![image](https://user-images.githubusercontent.com/127110867/225038422-82a158ee-5c79-4edc-abf8-20034fe97cd1.png) : wand tool, set the sensitivty in preferences.

![image](https://user-images.githubusercontent.com/127110867/225042065-a328453b-71b6-4c0b-a0ec-a6faa4406495.png) : Allows you to count the cells of the same class. If you want to count cells of another class, you can press "Add" in the window that opened when you started selecting cells. You can save the list of points to a file for future reference.

![image](https://user-images.githubusercontent.com/127110867/225261165-fa603c30-9744-474b-a909-863e4b67cec7.png) : When selected it prevents the creation of annotations but not modify the existing ones.

The annotations can be prioritised, when you press on "insert in hierarchy", the annotation 




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
![image](https://user-images.githubusercontent.com/127110867/225045509-a3103c7b-ea3b-49a4-8c49-fb5c7f2fa941.png)   

ALT Key : 
- When the Move tool is selected, use the Alt key to click on multiple objects to select them.
- When the Brush or Wand tools are selected, use the Alt key to switch to 'eraser' mode when drawing

Shift Key :
- When the Brush or Wand tools are selected, use the Shift key to continue adding to an existing selected annotation (rather than creating a new one).

![image](https://user-images.githubusercontent.com/127110867/225048760-5512b02f-1afe-4678-add6-98f66dc8db72.png) ![image](https://user-images.githubusercontent.com/127110867/225048877-c990f570-dd8b-4d81-b650-54ddb3eb9624.png)


![Clipboard](https://user-images.githubusercontent.com/41480459/225923649-6c638346-f737-4d2f-8bd4-8c853beab471.jpg)

![Clipboard-1](https://user-images.githubusercontent.com/41480459/225924006-8c9935d8-25a6-470b-bb13-f070b961297c.jpg)
