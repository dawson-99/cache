# 指定CMake的最低版本要求，确保兼容性
cmake_minimum_required(VERSION 3.10)

# 定义项目名称，后续可以使用${PROJECT_NAME}引用
project(MyCppProject)

# 设置C++标准为C++17
set(CMAKE_CXX_STANDARD 17)

# 强制要求使用指定的C++标准，如果编译器不支持则报错
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 添加头文件目录，使编译器能够找到include目录下的头文件
include_directories(${PROJECT_SOURCE_DIR}/include)

# 定义可执行文件，${PROJECT_NAME}为项目名称，src/main.cpp为源文件
add_executable(${PROJECT_NAME} src/main.cpp) 