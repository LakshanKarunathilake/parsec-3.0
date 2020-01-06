cmake_minimum_required(VERSION 3.15)
project(src C)

set(CMAKE_C_STANDARD 11)

include_directories(.)
include_directories(openssl)

add_executable(src
        openssl/md32_common.h
        openssl/sha.h
        openssl/sha_locl.h
        binheap.c
        binheap.h
        config.h
        debug.h
        decoder.c
        decoder.h
        dedup.c
        dedupdef.h
        encoder.c
        encoder.h
        hashtable.c
        hashtable.h
        hashtable_private.h
        mbuffer.c
        mbuffer.h
        queue.c
        queue.h
        rabin.c
        rabin.h
        sha.c
        sha.h
        tree.c
        tree.h
        util.c
        util.h)
