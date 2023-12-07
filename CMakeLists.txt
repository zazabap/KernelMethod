cmake_minimum_required(VERSION 3.0)
project(kernel-methods-cpp)

set(CMAKE_CXX_STANDARD 17)

# Include directories for svm_light
include_directories(${CMAKE_SOURCE_DIR}/lib/svm_light)

# Link directories for svm_light
link_directories(${CMAKE_SOURCE_DIR}/lib/svm_light)

# Source files
file(GLOB SOURCES "src/*.cpp")

# Executable
add_executable(main ${SOURCES})

# Link svm_light library
# target_link_libraries(main svm_light)
