add_definitions(-D_SPIRV_LLVM_API)
include_directories(..)
add_llvm_library(LLVMSPIRVlibSPIRV
  SPIRVBasicBlock.cpp
  SPIRVDebug.cpp
  SPIRVDecorate.cpp
  SPIRVEntry.cpp
  SPIRVFunction.cpp
  SPIRVInstruction.cpp
  SPIRVModule.cpp
  SPIRVStream.cpp
  SPIRVType.cpp
  SPIRVUtil.cpp
  SPIRVValue.cpp
  LINK_LIBS LLVMSPIRVMangler
 )
