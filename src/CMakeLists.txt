#Deprecate to use this style
#include_directories("${PROJECT_SOURCE_DIR}")

set(SHAPE_SRC
    circle.cpp
    point.cpp
    rectangle.cpp
    shape.cpp
    shapefactory.cpp
    triangle.cpp 
    )

add_library(shape_base STATIC ${SHAPE_SRC})
target_include_directories(shape_base
    PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

add_executable(shape_demo main.cpp)
target_link_libraries(shape_demo PUBLIC shape_base)