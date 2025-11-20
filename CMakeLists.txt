cmake_minimum_required( VERSION 3.17 )

#
project( simpleptgpu CUDA )

include_directories( C:/Users/sukai/source/repos/cuda-samples/Common/ )
add_executable( simpleptgpu main.cu ray.hpp scene.hpp sphere.hpp intersection.hpp )

set_target_properties(
        simpleptgpu
        PROPERTIES
        CUDA_SEPARABLE_COMPILATION ON)

#
project( simplertaa CUDA )
include_directories( C:/Users/sukai/source/repos/cuda-samples/Common/ )
add_executable( simplertaa rtaa.cu ray.hpp scene.hpp sphere.hpp intersection.hpp )

set_target_properties(
        simplertaa
        PROPERTIES
        CUDA_SEPARABLE_COMPILATION ON)
