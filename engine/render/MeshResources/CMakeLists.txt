#--------------------------------------------------------------------------
# MeshResources project
#--------------------------------------------------------------------------

PROJECT(MeshResources)
FILE(GLOB example_headers code/*.h)
FILE(GLOB example_sources code/*.cc)
FILE(GLOB example_sources code/*.cpp)

SET(files_MeshResources ${example_headers} ${example_sources})
SOURCE_GROUP("MeshResources" FILES ${files_example})

ADD_EXECUTABLE(MeshResources ${files_example})
TARGET_LINK_LIBRARIES(MeshResources core render)
ADD_DEPENDENCIES(MeshResources core render)