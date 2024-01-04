This is a template which uses CMake and VCPKG...

Change the "vcpkg.json" file to change the dependencies for your project

What to change:

      --  Replace/Change the vcpkg.json file dependencies to the depencies you want for your project
      --  In the CMakePresets.json file look for "CMAKE_TOOLCHAIN_FILE" under "cacheVariables" and replace the value for it with the location of the vcpkg.cmake location
      --  Change the CMakeLists.txt with whatever your project needs

Then you are set to go....
      
    
