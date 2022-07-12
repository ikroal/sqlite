cmake_minimum_required(VERSION 3.22)
project(sqlite C)

set(CMAKE_C_STANDARD 99)
set(CMAKE_C_FLAGS "-DSQLITE_CORE=1")
INCLUDE_DIRECTORIES(${CMAKE_INCLUDE_CURRENT_DIR})
aux_source_directory(src SQLITE_SRC)

add_executable(sqlite ${SQLITE_SRC})
