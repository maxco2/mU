include(${CMAKE_SOURCE_DIR}/UnifyPackageNameFormat.cmake)
include_directories(${mU_HEADER_DIR})
AUX_SOURCE_DIRECTORY(. MATRIX_SRCS)

add_library(Matrix ${PACKAGE_LIB_TYPE} ${MATRIX_SRCS})

target_link_libraries(Matrix Kernel Function gmp)

