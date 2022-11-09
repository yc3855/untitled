cmake_minimum_required(VERSION 3.14)

project("HelloWorld" CXX)

add_executable(${PROJECT_NAME} main.cpp)

find_package(NumCpp 0.0.0 REQUIRED)
target_link_libraries(${PROJECT_NAME}
        NumCpp::NumCpp
        )