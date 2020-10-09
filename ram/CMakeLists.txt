add_executable(config2cfg config2cfg.c)
target_link_libraries(config2cfg lib_tools)

add_executable(sdram sdram.c)
target_link_libraries(sdram lib_tools)

add_library(lib_ram STATIC
	../ram/nvram.c
	../ram/sdramfile.c
	../ram/sdrampeek.c
	)

install(TARGETS config2cfg sdram
	RUNTIME PERMISSIONS OWNER_READ OWNER_EXECUTE GROUP_READ GROUP_EXECUTE WORLD_READ WORLD_EXECUTE)

install(FILES config2cfg.1 sdram.1
	DESTINATION ${CMAKE_INSTALL_MANDIR}/man1 COMPONENT doc)
