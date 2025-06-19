cmake_minimum_required(VERSION 3.10)
project(stb_img LANGUAGES C)

add_library(stb_img STATIC
    src/stb_image.cpp
)

target_include_directories(stb_img PUBLIC
    $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
    $<INSTALL_INTERFACE:include>
)
