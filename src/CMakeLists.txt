cmake_minimum_required(VERSION 3.22.0)

project(template-project)

include(../cmake_macros/prac.cmake)

SETUP_APP(template-project "template-project")

if(TARGET SharedUtils)
    target_link_libraries(template-project SharedUtils)
endif()
