cmake_minimum_required(VERSION 3.22.0)
project(HomeWork_2_11_5)
set(LIB Figure.cpp
		Triangle.cpp
		Equilateral_triangle.cpp
		Isosceles_triangle.cpp
		Rectangle.cpp
		Right_triangle.cpp
		Square.cpp
		Parallelogram.cpp
		Quadrangle.cpp
		Rhombus.cpp)
set ( CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON )
add_library(Figure SHARED ${LIB})
add_executable(triangle_and_square main.cpp)
target_link_libraries(triangle_and_square Figure)
