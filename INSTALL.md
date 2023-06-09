3D ScANNING SOFTWARE BUILD INSTRUCTIONS

The software requires Qt and OpencV libraries. It should run on any system
satisfying those requirements. The current version was tested with Qt 5.5.1
and OpenCV 2.4.11, but could run with other versions. The software was developed
and extensively used with Visual Studio 2010 on Windows 7 x64. It can be compiled
for 32 bits and 64 bits targets. I have tested the software briefly on OS X 10.7.5
where it compiles and runs. At this time it is completely untested for GNU/Linux
although experienced programmers should be able to build it there too.

Prior to building, modify the paths on project/scan3d-capture.pro to match the location
and version of OpenCv in your system. The project file may be opened and build using 
Qt Creator or built from command line.

To build using make files from command line do this:
```
cd scan3d-capture && mkdir build &&cd build
qmake ../project
make (or nmake to build with Microsoft Visual Studio)
```

