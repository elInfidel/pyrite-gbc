set(SRC_DIR ${CMAKE_CURRENT_SOURCE_DIR}/src)

set(
    HEADER_FILES
    ${SRC_DIR}/z80.h 
    ${SRC_DIR}/memory.h
	${SRC_DIR}/cartridge.h
	${SRC_DIR}/ppu.h
)

set(
    SOURCE_FILES 
    ${SRC_DIR}/z80.cpp
    ${SRC_DIR}/memory.cpp
	${SRC_DIR}/cartridge.cpp
	${SRC_DIR}/ppu.cpp
)

add_library(pyrite-core STATIC ${HEADER_FILES} ${SOURCE_FILES})