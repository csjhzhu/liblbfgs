SET(LIBLBFGS_SRC lbfgs.c)

INCLUDE_DIRECTORIES(../include)

# build dynamic lib:  so(linux) dylib(mac osx)
ADD_LIBRARY(lbfgs SHARED ${LIBLBFGS_SRC})

TARGET_LINK_LIBRARIES(lbfgs m)

INSTALL(TARGETS lbfgs
        LIBRARY DESTINATION /usr/local/lib)
