file(GLOB_RECURSE TARGET_SOURCES "sources/*.cpp")
add_executable(Consumer ${TARGET_SOURCES})
target_include_directories(Consumer PUBLIC "${CMAKE_CURRENT_LIST_DIR}/includes")
target_link_libraries(Consumer ${CONAN_LIBS})