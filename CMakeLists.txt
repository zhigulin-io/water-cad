cmake_minimum_required(VERSION 3.6)

project(WaterCAD VERSION 1.0.0)

set(CXX_STANDARD 17)
set(CXX_STANDARD_REQUIRED true)

configure_file(config/ProjectConfig.h.in ProjectConfig.h)

add_executable(WaterCAD src/main.cpp)

target_include_directories(WaterCAD PUBLIC "${PROJECT_BINARY_DIR}")