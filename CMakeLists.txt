cmake_minimum_required(VERSION  3.16.3)
project(directory_test)
set(CMAKE_CXX_STANDARD 17)
#set(CMAKE_BUILD_TYPE Release)

include_directories(include)

file(GLOB SOURCES "src/examples/*.cpp")

add_library(numeths SHARED ${SOURCES})

install(TARGETS numeths DESTINATION /usr/lib/)

