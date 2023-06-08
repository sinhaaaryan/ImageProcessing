The sample image for the program is in the folder “images” in the submission folder.


Program Design changes and justifications

Considering the MVC design pattern, all three components, the model, the view, and the controller, are all completed and are functional.

In terms of the model, following the open-closed design principal, we created a new interface called IMultiplexImageModel and a new class called MultiplexImageModelImpl that implements the new interface. Using composition, this class has a field that takes in our previous version of the model, or ComplexImageModel. In the MultiplexImageModel class, we added a method that creates the histogram for the corresponding loaded image.

For the GUI View, we created a new interface called IGUIView and a class called GUI View that extends JFrame and also implements this interface. Within this class, we created the GUI View using the Java Swing library. 

We also created a new controller in a class called GUIController that implements ActionListener and also a new interface called IGUIController. This class serves as the action listener that is being added to the components of the GUI View in the GUIView class. We can start the program by calling upon the start method in this GUIController class.

List of Complete and Working Features
Open Image (Load)
Horizontal Flip
Vertical Flip
Brighten
Greyscale by Red Component
Greyscale by Blue Component
Greyscale by Green Component
Greyscale by Value Component
Greyscale by Luma Component
Greyscale by Intensity Component
Greyscale
Sepia
Blur
Sharpen
Save

Citation for Image
The image of Boston’s North End is displayed on the screenshot is taken from Viator.com. The image is from the following link. 
https://www.viator.com/tours/Boston/PhotoWalks-Boston-North-End-Little-Italy-Tour/d678-3643P12


How to use the program

The program can be used in three ways, either by using it with its GUI, with a script you can pass into the program, or by using the interactive text mode to use program.

In order to use the GUI, further instructions are given in the USEME file.

In order to use the program with a script to pass in, essentially you will need to pass in the command line argument “-file path-of-script-file” when running the jar file. This script file will need to have commands according to how the program is used in interactive text mode. 

In order to use the interactive text mode, here are the following commands:

Supported Script Commands

1. “file”
ex: “file script/script.txt”

2. “load”
ex: “load images/koala.png koala”

3. “red-component”
ex: “red-component koala koala-redGrey”

4. “blue-component”
ex: “blue-component koala koala-blueGrey”

5. “green-component”
ex: “red-component koala koala-greenGrey”

6. “value-component”
ex: “red-component koala koala-valueGrey”

7. “luma-component”
ex: “luma-component koala koala-lumaGrey”

8. “intensity-component”
ex: “intensity-component koala koala-intensityGrey”

9. “vertical-flip”
ex: “vertical-flip koala koala-vertical”

10. “horizontal-flip”
ex: “horizontal-flip koala koala-horizontal”

11. “brighten:
ex: “brighten 100 koala koala-brighter”
ex: “brighten -100 koala koala-darker”

12. “blur”
ex: “blur koala koala-blur”

13. “sharpen”
ex: “sharpen koala koala-sharp”

14. “greyscale”
ex: “greyscale koala koala-grey”

15. “sepia”
ex: “sepia koala koala-sepia”

16. “save”
ex: “save images/koala.bmp koala-sepia

17. “quit”/“Quit”/“q”/“Q”


