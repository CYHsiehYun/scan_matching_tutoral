cmake_minimum_required(VERSION 3.1)

#set the project name and version
project(scan_matching VERSION 1.0)

find_package(Eigen3 REQUIRED NO_MODULE)

#specify the cpp standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

include_directories(
    include
    ${EIGEN3_INCLUDE_DIRS})

#add_library(scan_matching_libs src/csv_reader.cpp)

#add the execotable
add_executable(01_eigen_tester apps/01_eigen_tester.cpp)