cmake_minimum_required(VERSION 2.8)

project(main)


find_package(Flann REQUIRED)
#find_package(HDF5 REQUIRED)


include_directories(${FLANN_INCLUDE_DIRS})
#include_directories(${HDF5_INCLUDE_DIRS})

link_directories(${HDF5_LIBRARY_DIRS})

add_executable(${PROJECT_NAME} ../src/main.cpp)

target_link_libraries(${PROJECT_NAME} ${FLANN_LIBRARIES} lz4 )

# ${HDF5_LIBRARIES}
