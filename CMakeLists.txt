cmake_minimum_required(VERSION 3.17)
project(maco)

set(CMAKE_CXX_STANDARD 17)

include_directories(
    "${CMAKE_CURRENT_SOURCE_DIR}/include"
    "${CMAKE_CURRENT_SOURCE_DIR}/tests"
)

#set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -E ")

add_executable(maco
        tests/catch.cpp
        include/maco/basic.h
        include/maco/detail/pp_size.h
        include/maco/detail/repeat_call.h
        tests/test_maco.cpp include/maco/aggregate.h include/maco/map.h include/maco/map_2.h include/maco/iterator_0.h include/maco/iterator_1.h include/maco/arguments.h include/maco/condition.h include/maco/loop.h include/maco/detail/loop.h include/maco/config.h include/maco/natural.h include/maco/compare.h include/maco/index_seq.h include/maco/detail/iterator_0.h include/maco/detail/map_2.h include/maco/detail/map.h include/maco/meta/meta_data_common.h include/maco/meta/lock_meta_data.h include/maco/meta/ro_meta_data.h)