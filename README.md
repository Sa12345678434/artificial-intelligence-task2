 # artificial-intelligence-task2


## Color recognition using openCV
This task involves a project that recognizes colors when you click on any point in image.
The project recognizes the color based on RGB values using data from colors.csv file, and the color and its RGB values are displayed at the top of image.


## Software used
1. Anaconda
2. Visual Studio


## Language used
 Python


## How this project works?
1. Uploads an image and enlarges it to specific size
2. When you click on any point in the image, its RGB values are calculated
3. After calculating the RGB values for selected point, they are compared to values in colors.csv file to determine which color are closest to selected point
4. The color name and its RGB values are showing at the top of the image


## Steps to implement this project

1. I download Anaconda and Visual Studio 
2. I clicked on __environments > base > open Terminal__ and then typed the following command:

   __pip install opencv-python__
4. On home page I clicked Launch for VS code
5. In Visual Studio code I clicked on __File > open folder > colors__

   The colors folder contains 6 images to test the project
7. After opening the folder containing the images, I created new file named __colors.csv__, in which I stored the color values in form of a table in RGB and HEX formats,which will be read to recognize the color

   image from file:
   
   ![image_alt](https://github.com/Sa12345678434/artificial-intelligence-task2/blob/main/colors11.jpg?raw=true)

8. I created new file named colors.ipynb, which is where I wrote the code in Python

   ### Some important commands:
 
 ```colors = pd.read_csv('colors.csv')``` -----> This command reads the __colors.csv__ file to find out what closest color is as selected point in image based on RGB values 

 ```img = cv2.imread('c6.jpg')``` -----> This command reads the image that I previously brought from folder , there are 6 images so every time I change the image path here 
 
 ```if cv2.waitKey(20) & 0xFF == 27: break```  ------> The window will continue to appear until you press the Esc key  
                             
9. I run the code on base(Python 3.13.5)

## Output

![image_alt](https://github.com/Sa12345678434/artificial-intelligence-task2/blob/main/outp1.png?raw=true)




  
 

