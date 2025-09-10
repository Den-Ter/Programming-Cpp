cmake_minimum_required(VERSION 4.1.1)
project(MyProject)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Явно указываем имя исполняемого файла
add_executable(my_app main.cpp)

# Для macOS/Linux добавляем возможность запуска
set_target_properties(my_app PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})