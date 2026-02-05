# GmE 205: Laboratory 1
## Computational Thinking Foundations: Python, VS Code, and GitHUb 

### *Description*
This project teaches how to set up the Python virtual environment in VS Code, to create a GitHub repository to practice *commit*, *push*, and *pull*, and to inspect *points.csv* using a Python script.

### *Dependencies*
* Python 3.14
* Visual Studio Code
* GitHub
* pandas
* matplotlib

### *How to set up the virtual environment?*
Here are the steps to set up a virtual environment:
1. Open the Visual Studio Code.
2. Under the VS Code Terminal tab, select "New Terminal."
3. Run this code:
        `py -m venv .venv`
        `.\.venv\Scripts\activate`

### *How to run Python scripts?*
Here are the steps to run Python scripts:
1. Create a new file named *hello.py* by right-clicking the specific folder under the Explorer tab.
2. Enter this code: 
        `import sys`<br>
        `print("Hello GmE 205")`
        `print("Python version:", sys.version)`
3. In the Terminal Tab, run this code:
        `python hello.py`

### *Help*
While performing this project, I encountered two errors.

1. I could not activate a virtual environment, which showed an error message like this: "*You cannot run this script on the current system. For more information about running scripts and setting execution policy, see about_Execution_Policies.*" I fixed this by following these steps:
* Press *Ctrl + Shift + P*
* Search for "*Terminal: Select Default Profile*"
* Select "*Command Prompt*"
* Make sure that your terminal is running using *cmd prompt* instead of "*Powershell*."

2. I could not find "*Python: Select Interpreter*," even though I have already installed Python. To resolve this case, I followed the following steps:
* Press Ctrl + Shift + X to open the Extension Marketplace.
* Search for the Python extension.
* Install the extension.
* Once the Python extension is installed, you will be able to search for "*Python: Select Interpreter*."

### *Reflection*
  Based on the script, I inspected the *points.csv* file, which contains longitude and latitude values. In the first part of the script, it checks the number of rows and columns, the column names, and any misisng or invalid values. The last part of the script plots the values, which produced a png file and a summary in a JSON file. I noticed that the Python scripts run in an activated virtual environment (*venv*), which provides this project with its own workspace without affecting other Python projects (CodeRivers, 2025). From the given CSV file and coordinates, the script assumes that the coordinates are within the range of -90 to 90 for latitude and -180 to 180 for longitude, wherein each are represented as a point. As shown in Lines 38 to 61 of *inspect_data.py*, it automatically checks the data quality by identifying missing and invalid values of longitude and latitude within the specified ranges. On the other hand, a human should check whether the output of the script plots the points accurately on the given coordinates and not interchanged, which results in a helpful output. If the dataset becomes very large, the application may consume higher memory and may load the script slowly, and sometimes, it may crash, similar to processing high-resolution satellite images in GIS, and the output image may become cluttered, which may show overlapping points or objects that are harder to analyze. 

## Author
Maria Graciella L. Roque  
Discord:[@grachiebob]

## Acknowledgements
* GmE 205 Laboratory Exercise 1 Manual
* [CodeRivers] (https://coderivers.org/blog/create-a-venv-python/)
* [MarkDown] (https://www.markdownguide.org/cheat-sheet/)

Edited on GitHub web interface and VS Code
