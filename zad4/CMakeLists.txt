cmake_minimum_required(VERSION 3.10)
project(zad4)
include_directories(include)
add_library(Student STATIC src/Student.cpp)
install(TARGETS Student DESTINATION /lib)
link_directories(/lib)
add_executable(zad4 src/libtest.cpp)
target_link_libraries(zad4 Student.a)
install(TARGETS zad4 DESTINATION /bin)
