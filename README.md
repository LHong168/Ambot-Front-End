# Ambot-Front-End
AUPP Marketing Robot - FYP Project

## Prerequisites
- Visual Studio 2019 or later

## Run Ambot Project
- Download or Clone Ambot-Json Project Folder
- Open Visual Studio
- Click on `Open a project or solution`
- find `Ambot-Json.sin` or `Ambot-Json.csproj`
- Optional: After the project load in Visual Studio, Right click on Main Project solution and build it
- Click Start Run Project

## How to Modify the Content of the Project
+ Open Ambot.json in `path: bin/debugg`
+ JSON file sections explanation:
- Pagenav: determine which Usercontrol layout will be use
- Button: buttonText (for the name and position of the button), buttonNav (for page navigation of button correspond to the number of the button)
- Content: 
set your image path starting from resources folder till the name of the file
Change text content accordingly

## How to add new key object to the JSon 
+ To add more unique object key in JSON file, for exmaple, image1, title or description1 etc. Do not forget to create a Class Object in JsonObject.cs
- Step 1: go to `JsonObject.cs`
- Step 2: look for parent class that you want to add, for example, Pages, Avatar, Contents or ControlButton etc
- Step 3: add a class object with the same key object in JSON.

## How to change layout of the Page
+ Choose Usercontrol that you want according to the name `PageLayout1` etc
+ Right click on that Usercontrol and select "View Design" 
+ Move or add any control that you want

## How to change the object key in the code
+ Choose Usercontrol that you want according to the name `PageLayout1` etc
+ Right click on that Usercontrol and select "View Code"
+ Set any field text or image you want to set, follow the Object tree in JsonObject.cs

#(OPTIONAL) How to display Image from resources folder
- Get the path from JSON object `resources/logo.png`
- Initialize the Image class and call this special class `ImageLoader.LoadImage()` and include the path above to the parameter
- Set any field .Image = to the initial variable

## How to create a new layout 
- Right click on the project solution, in this case, it's `Ambot-Json`
- Move your cursor to "Add" and then "User Control (Window Forms)"
- Set the name approprately "PageLayout...(Number)"
- Set the "PageNav" in JSON file according to the name of Usercontrol that you have created

