cmake_minimum_required(VERSION "3.16")

project(test-glfw)
find_package(glad CONFIG REQUIRED)
find_package(glfw3 CONFIG REQUIRED)
 
add_executable(main main3.cc)
target_link_libraries(main PRIVATE glad::glad glfw)
