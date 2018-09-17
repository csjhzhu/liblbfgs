ADD_EXECUTABLE(sample sample.c)
ADD_EXECUTABLE(sample2 sample.cpp)

INCLUDE_DIRECTORIES(../include)

TARGET_LINK_LIBRARIES(sample lbfgs)
TARGET_LINK_LIBRARIES(sample2 lbfgs)