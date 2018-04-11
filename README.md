# Fipsified libwebsockets

This is [libwebsockets](https://github.com/warmcat/libwebsockets) for [fips](https://github.com/floooh/fips). It is compiled without SSL by default, but the option can be set in the CMakeLists.txt.  When adding deps for this, use `fips_deps(zlib websockets <other deps>)`.