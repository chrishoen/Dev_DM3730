cmake_minimum_required(VERSION 3.10)
set (project "MyProgram3")
project(${project} CXX)
my_find_src_files (src_files ${project})
add_executable (${project} ${src_files})
my_add_compile_options (${project})

my_inc_import_MyStaticLib(${project})
my_lib_import_MyStaticLib(${project})
