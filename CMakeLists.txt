cmake_minimum_required(VERSION 2.8)

PROJECT(LBFGS)

set(CMAKE_MACOSX_RPATH 1)

#add source dir
ADD_SUBDIRECTORY(lib)
ADD_SUBDIRECTORY(sample)

# install include 
INSTALL(FILES include/lbfgs.h DESTINATION /usr/local/include)