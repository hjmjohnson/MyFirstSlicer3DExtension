cmake_minimum_required(VERSION 2.8.9)

project(MyFirstSlicer3DExtension)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/hjmjohnson/MyFirstSlicer3DExtension")
set(EXTENSION_CATEGORY "Examples")
set(EXTENSION_CONTRIBUTORS "Hans Johnson (The University of Iowa), Anonymous")
set(EXTENSION_DESCRIPTION "Learning the extension development")
set(EXTENSION_ICONURL "https://raw.github.com/hjmjohnson/MyFirstSlicer3DExtension/master/MyFirstSlicer3DExtension.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/MyFirstSlicer3DExtension/Screenshots/1.png")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(LineIntensityProfile)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
