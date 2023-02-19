cmake_minimum_required (VERSION 3.8)

set(CMAKE_EXPORT_COMPILE_COMMANDS true)
set(MY_MACRO_DIR "${CMAKE_CURRENT_SOURCE_DIR}/zzzMacros")
include("${MY_MACRO_DIR}/MyCodeMacros.cmake")
include("${MY_MACRO_DIR}/MyLocalImports.cmake")
include("${MY_MACRO_DIR}/MySpecial.cmake")

project ("Dev_DM3730")
my_print_cmake_vars()


add_subdirectory ("MyStaticLib")
add_subdirectory ("MyProgram1")
add_subdirectory ("MyProgram2")
add_subdirectory ("MyProgram3")
return()

add_subdirectory ("MyProgram1")
return()
