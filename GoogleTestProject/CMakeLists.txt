cmake_minimum_required(VERSION 3.13)
set(CMAKE_CXX_STANDARD 11)

find_package(GTest REQUIRED)
message("GTest_INCLUDE_DIRS = ${GTest_INCLUDE_DIRS}")

# Adding the library code ( Or you can linking the LibraryCode.cpp) 
add_library(commonLibrary LibraryCode.cpp)

# Adding the first executable
add_executable(mainApp main.cpp)
target_link_libraries(mainApp commonLibrary)

# Adding the second executable 
add_executable(unitTestRunner testRunner.cpp)

# Linking the google test for the second executable
target_link_libraries(unitTestRunner commonLibrary ${GTEST_LIBRARIES} pthread)

