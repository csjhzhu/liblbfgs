SET(LIBLBFGS_SRC lbfgs.c)

INCLUDE_DIRECTORIES(../include)

# build dynamic lib:  so(linux) dylib(mac osx)
ADD_LIBRARY(lbfgs SHARED ${LIBLBFGS_SRC})

INSTALL(TARGETS lbfgs
        LIBRARY DESTINATION /usr/local/lib)
