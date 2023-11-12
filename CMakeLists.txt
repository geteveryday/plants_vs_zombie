# 下面写的是CMake最低版本要求 格式：cmke_minimum_required(VERSION 版本号)
cmake_minimum_required(VERSION 3.26)
# 下面写的是项目名称 格式：project(项目名称)
project(plants_vs_Zombie)
#下面写的是项目c语言标准，即17标准 格式：set(CMAKE_CXX_STANDARD 标准号)
set(CMAKE_CXX_STANDARD 17)
# 下面是设置源文件路径
set(SOURCES main.cpp)
include_directories(include)
#设置外部库
link_directories(lib)
link_libraries(libeasyx.a)
#设置静态库
# 添加可执行文件，并指定源文件 格式： add_executable(可执行文件名称 源文件名称)
add_executable(plants_vs_Zombie ${SOURCES})
