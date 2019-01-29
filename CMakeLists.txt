# Modified by madmaxoft for static linkage
cmake_minimum_required(VERSION 2.8)
project(lsqlite3 C)

add_library(lsqlite3 STATIC
	lsqlite3.c
	sqlite3.c
)

target_link_libraries(lsqlite3 lua)
