cmake_minimum_required(VERSION 3.5)
project(my_project)

set(CMAKE_CXX_STANDARD 17)

# 配置头文件搜索路径
# include_directories(${PROJECT_SOURCE_DIR}/include)
# include_directories(${PROJECT_SOURCE_DIR}/include/log)

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)

# 设置生成clangd所需的comlile_commands.json
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_executable(main main.cpp)