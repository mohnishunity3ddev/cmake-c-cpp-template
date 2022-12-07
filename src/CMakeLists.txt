cmake_minimum_required(VERSION 3.22.0)

project(breakout-src)

include(../cmake_macros/prac.cmake)

SETUP_APP(breakout-src "breakout-src")

if(TARGET SharedUtils)
    target_link_libraries(breakout-src SharedUtils)
endif()
