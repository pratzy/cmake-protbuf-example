set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

add_executable(main main.cpp)
target_link_libraries(main message ${PROTOBUF_LIBRARY})
target_link_options(main PRIVATE "-pthread")