# File modified to compile for ESP-IDF

cmake_minimum_required(VERSION 3.5)

file(GLOB_RECURSE app_sources RELATIVE ${CMAKE_CURRENT_LIST_DIR} "src/*.c")

idf_component_register(SRCS ${app_sources} INCLUDE_DIRS "src" PRIV_INCLUDE_DIRS ".")

project(WebP)
