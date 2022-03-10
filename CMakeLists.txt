cmake_minimum_required(VERSION 3.5)
project(UdpSocketLearn)

set(CMAKE_C_STANDARD 11)

aux_source_directory(client clientSource)
aux_source_directory(server serverSource)

add_executable(udp_client ${clientSource})
add_executable(udp_server ${serverSource})