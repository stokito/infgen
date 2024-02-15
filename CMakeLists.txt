cmake_minimum_required(VERSION 2.4.4)
project(zlib-infgen C)

add_executable(infgen infgen.c)
target_link_libraries(infgen z)

INSTALL(TARGETS infgen
    RUNTIME DESTINATION bin
)