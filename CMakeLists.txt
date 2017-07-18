cmake_minimum_required(VERSION 2.6)
project(mouSSH)

set(mouSSHd_VERSION_MAJOR 1)
set(mouSSHd_VERSION_MINOR 0)

find_package(libssh REQUIRED)

add_executable(mouSSH main.c)
target_link_libraries(mouSSH ${LIBSSH_LIBRARIES})
