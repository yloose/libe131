set( e131_sources src/e131.c src/e131.h )

add_library( e131 ${e131_sources} )

target_include_directories( e131 PUBLIC src )

target_compile_options( e131 PRIVATE -Wall -O3 -std=gnu11 -pedantic )
# target_link_options( libe131 PRIVATE -export-symbols-regex '^[eE]131_[^_]')
