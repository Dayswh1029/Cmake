cmake_minimum_required(VERSION 4.3.0)
# cmake 需要的最小版本


# 写一个项目的名字

project(camke--study)

# 为了编译lesson1_1里面的文件，需要添加这个子目录
# 注意是这个根目录所在的文件夹里面有这个文件夹！ 
add_subdirectory(lesson1_1) 


# 如果当前文件夹 用./ ../ 为上一级文件夹
# add_subdirectory(./lesson1_1)

add_subdirectory(lesson1_2)

add_subdirectory(lesson2_1)
