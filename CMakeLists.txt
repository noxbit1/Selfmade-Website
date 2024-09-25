cmake_minimum_required(VERSION 3.10)
project(SimpleServer)

set(CMAKE_CXX_STANDARD 17)

add_executable(SimpleServer server.cpp)
find_package(Threads REQUIRED)
target_link_libraries(SimpleServer ${CMAKE_THREAD_LIBS_INIT})