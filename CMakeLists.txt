cmake_minimum_required(VERSION 3.0.0)
project(Testing_local_git_rep VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()

set(SOURCES
    main.cpp
    class_from_dev2.h
)

set(HEAD 
    class_from_dev2.h
)

add_executable(Testing_local_git_rep  ${SOURCES} ${HEAD})



set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
