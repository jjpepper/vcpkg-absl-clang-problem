cmake_minimum_required(VERSION 3.17)
project(vcpkg-absl-clang-problem VERSION 0.1 LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 17) 
find_package(absl CONFIG REQUIRED)

add_executable(main main.cpp)
target_link_libraries(main PUBLIC absl::flat_hash_map)
