cmake_minimum_required(VERSION 3.6)

project(octopus-ice)
add_executable(main main.cpp)

find_package(OpenGL REQUIRED)
find_package(GLUT REQUIRED)

include_directories(SYSTEM ${GLUT_INCLUDE_PATH} ${OPENGL_INCLUDE_PATH})
target_link_libraries(main ${GLUT_LIBRARIES} ${OPENGL_LIBRARIES})

