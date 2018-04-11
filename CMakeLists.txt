cmake_minimum_required(VERSION 2.8.9)

get_filename_component(ZLIB_ROOT_DIR "../fips-zlib" ABSOLUTE)

option(LWS_WITH_SSL "" OFF)
option(LWS_WITHOUT_TESTAPPS "" ON)
option(LWS_WITH_SHARED "" OFF)
option(LWS_WITH_BUNDLED_ZLIB "" OFF)
set(LWS_ZLIB_INCLUDE_DIRS "${ZLIB_ROOT_DIR}/zlib" CACHE PATH "Path to the zlib include directory")
set(LWS_ZLIB_LIBRARIES "${ZLIB_ROOT_DIR}/zlib" CACHE PATH "Path to the zlib include directory")

add_subdirectory(libwebsockets)