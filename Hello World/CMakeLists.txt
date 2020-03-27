cmake_minimum_required(VERSION "3.11.4")

project("HelloWorld")

add_executable("${PROJECT_NAME}" "Main.cpp") # the first parameter is the name of the executable, second is the source code that is required to build the executable  

install(TARGETS "${PROJECT_NAME}" DESTINATION bin) #${CMAKE_INSTALL_PREFIX}/bin
install(FILES "Main.cpp" DESTINATION src) #${CMAKE_INSTALL_PREFIX}/src
