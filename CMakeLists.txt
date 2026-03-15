cmake_minimum_required(VERSION 3.5)

project(GHMTexTool)

set (CMAKE_CXX_STANDARD 20)
set (CMAKE_DEBUG_POSTFIX -debug)

SET_PROPERTY(GLOBAL PROPERTY USE_FOLDERS ON)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/$<CONFIG>)

add_executable(GHMTexTool
    inc_wrapper.h
    hasher.h
    NMH.h
    extractorimpl.h
    main.cpp
)