cmake_minimum_required(VERSION 3.10.2)
project("shurikenmod")

add_library(
    shurikenmod
    SHARED
    main.cpp
)

find_library(
    log-lib
    log
)

target_link_libraries(
    shurikenmod
    ${log-lib}
)
