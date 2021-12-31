project(sqlite_modern_cpp)

add_library(sqlite_modern_cpp INTERFACE)
add_library(sqlite_modern_cpp::sqlite_modern_cpp  ALIAS sqlite_modern_cpp)
target_include_directories(sqlite_modern_cpp INTERFACE
    $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/hdr>
    $<INSTALL_INTERFACE:include>
)

# TBD install
