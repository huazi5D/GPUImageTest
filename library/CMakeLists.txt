cmake_minimum_required(VERSION 3.4.1)

add_library( gpuimage-library SHARED src/main/cpp/yuv-decoder.cpp )

find_library( log-lib log )

target_link_libraries( gpuimage-library ${log-lib} )