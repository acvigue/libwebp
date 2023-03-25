# File modified to compile for ESP-IDF

cmake_minimum_required(VERSION 3.5)

FILE(GLOB_RECURSE app_sources ${CMAKE_CURRENT_LIST_DIR}/src/*.c)

idf_component_register(SRCS app_sources
                       INCLUDE_DIRS "./src" 
                       )

project(WebP)
