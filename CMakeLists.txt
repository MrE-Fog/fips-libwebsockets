cmake_minimum_required(VERSION 2.8.9)

option(LWS_WITH_SSL "" OFF)
option(LWS_WITHOUT_TESTAPPS "" ON)
option(LWS_WITH_SHARED "" OFF)
add_subdirectory(libwebsockets)
target_include_directories(libwebsockets PUBLIC libwebsockets/include)

#fips_begin_lib(libwebsockets)
#    fips_dir(libwebsockets/lib)
#    fips_files(
#	misc/base64-decode.c
#	handshake.c
#	libwebsockets.c
#	service.c
#	pollfd.c
#	output.c
#	server/parsers.c
#	context.c
#	alloc.c
#	header.c
#	misc/lws-ring.c
#   client/client.c
#	client/client-handshake.c
#	client/client-parser.c)
#fips_end_lib()
