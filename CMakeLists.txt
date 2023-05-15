cmake_minimum_required(VERSION 3.14 FATAL_ERROR)

set(CMAKE_CXX_STANDARD 20)

set(CMAKE_CXX_EXTENSIONS OFF)

project(NanoSignalSlot VERSION 2.0.1 LANGUAGES CXX)

add_library(nano-signal-slot ALIAS NanoSignalSlot INTERFACE)

target_compile_features(nano-signal-slot INTERFACE cxx_std_${CMAKE_CXX_STANDARD})

target_include_directories(nano-signal-slot INTERFACE include)

