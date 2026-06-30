
cmake_minimum_required(VERSION  3.28.3)
project(linux_lesson)

add_subdirectory(add)

#  强制把编译好的程序扔进你的 build 文件夹
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/build)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/build)


add_executable(lesson1_1 main.cpp)

#  告诉编译器，main.cpp 里用的 #include "add.h" 去哪找

target_include_directories(lesson1_1 PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/add)



target_link_libraries(lesson1_1 PUBLIC add_lib)