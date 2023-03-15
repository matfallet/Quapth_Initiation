# Qupath_Initiation
cluster/phenotyping/interaction

For more informations about QuPath consult the website "https://qupath.readthedocs.io/en/stable/index.html" or watch the videos in the plateform Github.com "..."

## Use of QuPath
### Create a project 
  - Press "Create project" 
  - Create a file with nothing in it 
  - Selection the image that interess you with "Add images", choose in your files or drag and drop directly in the software. 
   - FORMAT D'IMAGE --> demander 
   - By double-clicking on the selected image, a "set image type" window opens. Select the appropriate image type.
   - To reopen the project, clic on "open project" and select "project".qpproj or drag and drop the project files directly into the sofware 

## Icon function 
![image](https://user-images.githubusercontent.com/127110867/225029024-b802c332-f8c5-473e-a7c0-59e0ba6d2013.png) : Allows you to make the left column appear or disappear  

![image](https://user-images.githubusercontent.com/127110867/225029694-10ee0824-4ace-4c61-9b05-d8ab78472636.png) : Allows you to move image in all directions, but you can do this with the right-click. You can also use the mouse scroll wheel for zooming. 

![image](https://user-images.githubusercontent.com/127110867/225032103-7ba78885-f2b4-4408-b767-3d04b08d4be7.png) : Draws a rectangle around the area of interest. This function is used to acquire an annotation. This annotation is saved in the "Annotation" tab. When this annotation is yellow, you can move it, but when it is red, you cannot move it unless you double-click inside. 

![image](https://user-images.githubusercontent.com/127110867/225034022-d21ac8d4-e381-4457-9b5b-6296d10e304b.png) : Same function as the rectangle 

![image](https://user-images.githubusercontent.com/127110867/225034273-7302a61f-910a-4fbd-83e4-b416bfe131eb.png) : Create a line 

![image](https://user-images.githubusercontent.com/127110867/225035326-06cddf99-5d66-417c-8833-545ebf57a0bf.png) :
Create a polygon. Double-click when finished. 

![image](https://user-images.githubusercontent.com/127110867/225035459-4458d2f8-65a4-4634-8690-ed1b44f5b3ba.png) : Create a freehand area, without releasing the mouse 

![image](https://user-images.githubusercontent.com/127110867/225037603-e83a92da-da25-458b-9166-1e46f2a8f5b5.png) : Create an area with rounded corners. When you draw a large circle, you can fill in the inside of the circle.

![image](https://user-images.githubusercontent.com/127110867/225038422-82a158ee-5c79-4edc-abf8-20034fe97cd1.png) : Create an area close to your image, avoiding cells and nuclei 

![image](https://user-images.githubusercontent.com/127110867/225042065-a328453b-71b6-4c0b-a0ec-a6faa4406495.png) : Allows you to count the cells of the same class. If you want to count cells of another class, you can press "Add" in the window that opened when you started selecting cells. You can save the list of points to a file for future reference.

![image](https://user-images.githubusercontent.com/127110867/225261165-fa603c30-9744-474b-a909-863e4b67cec7.png) : When selected it prevents the creation of annotations 

![image](https://user-images.githubusercontent.com/127110867/225261236-ef56c90d-59b7-4d97-9fd8-54679f882eee.png) : Select the channels and their intensity. You can change the channel name by double-clicking on the top. Or by using a script.   
- Write the channel name as a "notepad or word" on the separate line. 
- Copy the lines and select all channels at once and press "Clrl+V"  
![image](https://user-images.githubusercontent.com/127110867/225262038-e164f93b-8b36-4ad5-87c5-087996baed33.png) ![image](https://user-images.githubusercontent.com/127110867/225263469-21f7d51a-f7fb-40c2-a2be-10d4bf263a9f.png)

- In the "Annotation" tab, on the right hand side, the channels name are in the column. If this is not the case, you can press the three small dots at the bottom right of the column and select "Populate from image channels".  
-  The names of the start channels are not lost, if you press the "Image" tab, and double-click on "Metadata changed" you get the start names back.   

To get the optimal intensity of the channel, you can play with the bar of the graph. You have to select the channel beforehand. You can also use "Min display" or "Max display". The "Gamma" allows you to amplify the background noise.   
![image](https://user-images.githubusercontent.com/127110867/225268944-dd1a1a41-9899-412c-a72d-3207c6bf7415.png) ![image](https://user-images.githubusercontent.com/127110867/225268978-dad7ba74-91f8-4e5a-b69f-1e37d028b03c.png)

![image](https://user-images.githubusercontent.com/127110867/225269648-0ed7deef-2f6e-4a9c-9019-e91c26d1869e.png) : 
By pressing this key, you can freeze the image. If you are in zoom mode, you can press the button to return to the original position and freeze the image, if you want to move again, you have to press the button again.

![image](https://user-images.githubusercontent.com/127110867/225270911-3d6aaa16-1e73-40fe-89f9-007b77ae10d8.png) : Shows only the selected annotation.

![image](https://user-images.githubusercontent.com/127110867/225271644-87dd7076-f335-4b6c-b190-e256515e4c8c.png) : 
Displays the name of the annotations. To name an annotation, you need to go to the "Annotation" tab and double-click on the annotation, then select "Set properties" and change the name. 

![image](https://user-images.githubusercontent.com/127110867/225273685-638fe595-c9f0-46ef-8269-c63bd4051b67.png) : Shows the TMA grid in the viewer






































      Shortcut keys  
![image](https://user-images.githubusercontent.com/127110867/225045509-a3103c7b-ea3b-49a4-8c49-fb5c7f2fa941.png)   

ALT Key : 
- When the Move tool is selected, use the Alt key to click on multiple objects to select them.
- When the Brush or Wand tools are selected, use the Alt key to switch to 'eraser' mode when drawing

Shift Key :
- When the Brush or Wand tools are selected, use the Shift key to continue adding to an existing selected annotation (rather than creating a new one).

![image](https://user-images.githubusercontent.com/127110867/225048760-5512b02f-1afe-4678-add6-98f66dc8db72.png) ![image](https://user-images.githubusercontent.com/127110867/225048877-c990f570-dd8b-4d81-b650-54ddb3eb9624.png)



