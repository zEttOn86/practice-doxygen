# first we can indicate the documentation build as an option and set it to ON by default
option(BUILD_DOC "Build documentation" ON)

# check if Doxygen is installed
find_package(Doxygen REQUIRED)

#--------
# Build doxygen docs
#--------
if(DOXYGEN_FOUND)
add_custom_target(documents ALL
                  COMMAND doxygen ${CMAKE_CURRENT_SOURCE_DIR}/Doxyfile
                  WORKING_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}
                  COMMENT "Generating API documentation with Doxygen"
                )
endif()