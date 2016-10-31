add_executable(config2cfg config2cfg.c)
target_link_libraries(config2cfg lib_tools)

add_executable(sdram sdram.c)
target_link_libraries(sdram lib_tools)

add_library(lib_ram STATIC
	../ram/nvram.c
	../ram/sdramfile.c
	../ram/sdrampeek.c
	)
