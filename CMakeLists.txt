# CMake for GLAD/GLFW project
cmake_minimum_required(VERSION 3.24)

# Change this to your project name
project("CMAKE_VCPKG_TEMPLATE")

# Finding the packages
find_package(glm)
find_package(glad)
find_package(glfw3)

# Prepping the glm package 
add_library(glm INTERFACE)
target_include_directories(glm INTERFACE ${GLM_INCLUDE_DIRS})

add_executable(${PROJECT_NAME} src/main.cpp)

target_link_libraries(${PROJECT_NAME} PRIVATE glad::glad glfw glm)