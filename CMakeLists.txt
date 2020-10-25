cmake_minimum_required(VERSION 3.10.2)

project(SearchServer)

set(SOURCES main.cpp search_server.cpp parse.cpp)
set(HEADERS search_server.h parse.h Synchronized.h iterator_range.h profile.h test_runner.h)
set(CMAKE_CXX_STANDARD 17)

add_executable(SearchServer ${SOURCES} ${HEADERS})

set_target_properties(
	SearchServer PROPERTIES
	CXX_STANDART 17
	CXX_STANDART_REQUIRED ON
)
