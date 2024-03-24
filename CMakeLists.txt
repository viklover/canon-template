cmake_minimum_required(VERSION 3.15)
project(conan-test CXX)

find_package(libpqxx REQUIRED)

add_executable(${PROJECT_NAME} src/main.cpp)
target_link_libraries(${PROJECT_NAME} libpqxx::pqxx)
