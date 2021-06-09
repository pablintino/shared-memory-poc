file(GLOB_RECURSE TARGET_SOURCES "sources/*.cpp")
add_executable(Producer ${TARGET_SOURCES})
target_include_directories(Producer PUBLIC "${CMAKE_CURRENT_LIST_DIR}/includes")
target_link_libraries(Producer ${CONAN_LIBS})