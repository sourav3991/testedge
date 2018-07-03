cmake_minimum_required(VERSION 2.8)

set(CMAKE_BUILD_TYPE debug)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++14")

project(sample)

add_executable(
	sample
        main.cpp
)

target_link_libraries(
	sample
	mosquitto
)
