add_executable(config2cfg config2cfg.c)
target_link_libraries(config2cfg tools_lib)

add_executable(sdram sdram.c)
target_link_libraries(sdram tools_lib)

add_library(ram_lib STATIC
	../ram/nvram.c
	../ram/nvrampeek.c
	../ram/sdramfile.c
	../ram/sdramfileA.c
	../ram/sdrampeek.c
	../ram/sdramtext.c
	)
