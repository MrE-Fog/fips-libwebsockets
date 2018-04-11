cmake_minimum_required(VERSION 2.8.9)

fips_begin_lib(libwebsockets)
    fips_dir(libwebsockets/lib)
    fips_files(
	misc/base64-decode.c
	handshake.c
	libwebsockets.c
	service.c
	pollfd.c
	output.c
	server/parsers.c
	context.c
	alloc.c
	header.c
	misc/lws-ring.c
    client/client.c
	client/client-handshake.c
	client/client-parser.c
    server/server.c
	server/lws-spa.c
	server/server-handshake.c)
fips_end_lib()
