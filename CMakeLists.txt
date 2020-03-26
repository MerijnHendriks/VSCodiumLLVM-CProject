cmake_minimum_required(VERSION 3.5)

# project name
project(proc)

# clangd
set(CMAKE_EXPORT_COMPILE_COMMANDS true)

# executable
add_executable(proc
    src/proc.c
)

# compiler flags
target_compile_options(proc
    PRIVATE
        "-O0"
        "-v"
)
