cmake_minimum_required(VERSION 3.0)

project(LP_PROJETO_FINAL VERSION 0.1.0)

set(CMAKE_VERBOSE_MAKEFILE OFF)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/../bin)

set(CMAKE_C_STANDARD 11)
set(CMAKE_C_EXTENSIONS OFF)
set(CMAKE_CXX_FLAGS_DEBUG "${CMAKE_CXX_FLAGS_DEBUG} -Wall -Wextra -fsanitize=undefined")
set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE} -Wall -Wextra")

add_executable(main.x86
               ../src/main.c
               ../src/menu.c
               ../src/morada.c
               ../src/artigo.c
               ../src/encomenda.c
               ../src/utilities.c
               ../src/utilizador.c)