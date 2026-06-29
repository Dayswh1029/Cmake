add_subdirectory(add)

include_directories(./lib)

# 生成可执行文件
# 链接库 
# method 1 不推荐！ 需要绝度路径
# link_libraries(E:/CPP_Project/Cmake/lesson2_1/lib/add_static.lib)


# 方法2 
link_directories(E:/CPP_Project/Cmake/lesson2_1/lib/add_static.lib)

# 把cpp文件生成可执行文件！！ 

add_executable(lesson2_1 main.cpp)

# target 就是less2_1 希望 链接到lib 为add_static.lib
target_link_libraries(lesson2_1 add_static.lib)