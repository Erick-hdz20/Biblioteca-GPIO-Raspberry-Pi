cmake_minimum_required(VERSION 3.16)

project(Proyecto5 C)

add_executable(Proyecto5
    src/main.c
    src/gpio.c
)

target_include_directories(Proyecto5
    PRIVATE
    include
)

target_link_libraries(Proyecto5
    gpiod
)