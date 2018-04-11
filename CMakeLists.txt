cmake_minimum_required(VERSION 2.8.9)

option(LWS_WITH_SSL "" OFF)
option(LWS_WITHOUT_TESTAPPS "" ON)
option(LWS_WITH_SHARED "" OFF)
option(LWS_WITH_ZLIB "" OFF)

add_subdirectory(libwebsockets)