include_directories(android)

add_library(
        libmad

        STATIC

        version.c
        fixed.c
        bit.c
        timer.c
        stream.c
        frame.c
        synth.c
        decoder.c
        layer12.c
        layer3.c
        huffman.c
)

target_compile_options(libmad PUBLIC -DHAVE_CONFIG_H -DFPM_DEFAULT)
