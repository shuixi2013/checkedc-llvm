include_directories( ${CMAKE_CURRENT_BINARY_DIR}/.. ${CMAKE_CURRENT_SOURCE_DIR}/.. )

add_llvm_library(LLVMAMDGPUDisassembler
  AMDGPUDisassembler.cpp
  )

add_dependencies(LLVMAMDGPUDisassembler AMDGPUCommonTableGen)
