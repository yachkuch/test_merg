cmake_minimum_required(VERSION 3.0.0)
project(Testing_local_git_rep VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()

add_executable(Testing_local_git_rep main.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
