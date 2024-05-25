cmake_minimum_required(VERSION 3.4)
project(solver)
add_subdirectory(formatter_ex)
add_subdirectory(solver_lib)
set(SOURCES
    solver.cpp
)
add_executable(solver )
target_link_libraries(solver PRIVATE formatter_ex solver_lib)
