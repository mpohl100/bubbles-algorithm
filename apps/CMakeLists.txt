include_directories(${CMAKE_SOURCE_DIR}/src)
link_directories(${CMAKE_SOURCE_DIR}/src)

find_package(clara REQUIRED)

add_executable(bubble bubbles.cpp)
target_link_libraries(bubble bubbles math2d clara::clara)
target_include_directories(bubble PUBLIC ${CMAKE_SOURCE_DIR}/src)