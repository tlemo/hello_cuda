
cmake_minimum_required(VERSION 3.25 FATAL_ERROR)

project(hello_cuda LANGUAGES C CXX CUDA)

add_executable(hello_cuda main.cu)

set_property(TARGET hello_cuda PROPERTY CUDA_ARCHITECTURES 60)
