
cmake_minimum_required(VERSION 3.25)

project(network_message_pipeline
    VERSION 0.1.0
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

option(BUILD_PRODUCER "Build market data producer" ON)
option(BUILD_RECEIVER "Build message receiver" OFF)
option(BUILD_BENCHMARKS "Build benchmarks" OFF)

# find_package(Threads REQUIRED)

# add_subdirectory(common)

if(BUILD_PRODUCER)
    add_subdirectory(producer)
endif()

# if(BUILD_RECEIVER)
#     add_subdirectory(transport)
#     add_subdirectory(pipeline)
#     add_subdirectory(order_book)
# endif()

# if(BUILD_BENCHMARKS)
#     add_subdirectory(benchmarks)
# endif()
