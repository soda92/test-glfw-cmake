cmake_minimum_required(VERSION "3.16")
project(glfw)

add_executable(main main.c)

include_directories(include)

# find_library(LIB_TO_INCLUDE glfw ${PROJECT_SOURCE_DIR}/lib-mingw-w64/)
# add_library(glfw SHARED ${PROJECT_SOURCE_DIR}/lib-mingw-w64/)
# set_target_properties(glfw PROPERTIES LINKER_LANGUAGE CXX)
target_link_libraries(main ${PROJECT_SOURCE_DIR}/lib-mingw-w64/libglfw3.a)
