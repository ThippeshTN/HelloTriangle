cmake_minimum_required (VERSION 3.6)
project (Hello_Triangle)

add_subdirectory(src_ext)

add_executable(${PROJECT_NAME} ./src/main.cpp)

target_link_libraries(${PROJECT_NAME} glad glfw)

target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/src_ext/glad/include)