C++ Project Template

This project template provides a simple starting point for a new C++ project. 
It includes a basic main.cpp file, a resource file (info.rc), and a batch script (build.bat) to compile the project.
This template is purposed for quickly putting together lightweight applications with a refined look and slim size.

Project Structure

- appicon.ico: The icon file for the application.
- bin/: Directory where the compiled resources and executable will be placed.
- build.bat: Batch script to compile the project.
- info.rc: Resource file containing version information and icon path.
- main.cpp: Main source file for the application.
- README.txt: This file.
- upx.exe: UPX executable for compressing the final binary.

Instructions

1. Adjust the Icon Path:
   The info.rc file contains an absolute path to the icon file. You need to update this path to match the location of appicon.ico on your system. Open info.rc and modify the following line:
   id ICON "C:/Your/Absolute/Path/To/The/Icon/appicon.ico"
   Replace C:/Your/Absolute/Path/To/The/Icon/appicon.ico with the correct path to appicon.ico.

2. Compile the Project:
   Run the build.bat script to compile the project. This script will:
   - Compile the resource file (info.rc) using windres.
   - Compile the main source file (main.cpp) and link it with the compiled resource file using g++.
   - Compress the resulting executable using UPX.

   To run the script, open a command prompt and execute:
   build.bat

3. Run the Executable:
   After the build process completes, the final executable (main.exe) will be located in the bin directory. You can run it from there.

Notes

- Ensure that windres, g++, and upx are installed and available in your system's PATH.
- The provided upx.exe is for convenience. If you prefer, you can download the latest version of UPX from the official website.

License

This project template is provided freely for anyone to use and modify. Feel free to customize it to suit your needs.
For license information on UPX, read https://upx.github.io/upx-license.html or https://upx.github.io/
For license information on g++, read https://gcc.gnu.org/onlinedocs/libstdc++/manual/license.html