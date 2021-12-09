cmake_minimum_required(VERSION 3.0.0)
project(NetfilterEG VERSION 0.1.0)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

aux_source_directory(src DIR_SRCS)
add_executable(NetfilterEG ${DIR_SRCS})
target_link_libraries(NetfilterEG mnl netfilter_queue)