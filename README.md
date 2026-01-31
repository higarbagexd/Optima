# Optima
release > exe has main program
instructions for exe building:
set to release mode

switch the build configuration from Debug to Release. 
Build. this will generate an .exe file in a new release folder within your build directory. 
Step 2: Deploy using windeployqt which can be retrieved from tools in your qt directory 
the generated .exe file depends on specific qt libs and dlls so to run on other computers (or even outside of the Qt Creator environment on your own machine), the windeployqt tool automates copying these required files. 
Open the appropriate Qt command-line window from start menu(e.g., "Qt 6.x.x (MinGW x.x.x 64-bit)" or the Visual Studio equivalent, depending on your compiler).
use cd and navigate to directory
run
windeployqt your_project_name.exe
OR
go to exe folder, click on the folder path bar, type 'cmd' and press enter. The windows command line will open and you can run the above command there
This may not work (because it requires qt's libs) but sometimes it can.
