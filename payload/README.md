# Compiling the Payload

1. Install the Microsoft Visual C++ (MSVC) C and C++ compilers and linkers by following the instructions [here](https://learn.microsoft.com/en-us/cpp/build/building-on-the-command-line?view=msvc-170#download-and-install-the-tools).
1. Set the build environment as per the instructions [here](https://learn.microsoft.com/en-us/cpp/build/building-on-the-command-line?view=msvc-170#developer_command_file_locations):
   ```
   "C:\Program Files (x86)\Microsoft Visual Studio\2022\BuildTools\VC\Auxiliary\Build\vcvars64.bat"
   ```
1. Compile the Dynamic-Link Library (DLL) file that contains the payload.
   ```
   cl /LD providers.cpp
   ```
