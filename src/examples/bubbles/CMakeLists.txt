include_directories( ${CMAKE_SOURCE_DIR}/src )

set( BUBBLES_SOURCES Canvas2D.cpp bubbles_swarm.cpp Tiles.cpp)

add_library( bubbles SHARED ${BUBBLES_SOURCES} )
target_include_directories(bubbles PUBLIC {CMAKE_SOURCE_DIR}/src)

add_library( math2d SHARED math2d.cpp )
target_include_directories(math2d PUBLIC {CMAKE_SOURCE_DIR}/src)