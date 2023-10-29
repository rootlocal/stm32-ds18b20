set(LIB_NAME ds18b20_lib)

message(STATUS "Build: ${LIB_NAME}")

include_directories("src/inc")
file(GLOB_RECURSE LIB_SOURCES "src/*.c")

ADD_LIBRARY(${LIB_NAME} STATIC ${LIB_SOURCES})