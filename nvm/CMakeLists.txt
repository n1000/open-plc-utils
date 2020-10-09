add_executable(chknvm chknvm.c)
target_link_libraries(chknvm lib_nvm lib_ram lib_tools)

add_executable(chknvm2 chknvm2.c)
target_link_libraries(chknvm2 lib_nvm lib_tools)

add_executable(nvmmerge nvmmerge.c)
target_link_libraries(nvmmerge lib_tools)

add_executable(nvmsplit nvmsplit.c)
target_link_libraries(nvmsplit lib_tools)

add_library(lib_nvm STATIC
	../nvm/fdmanifest.c
	../nvm/manifest.c
	../nvm/nvm.c
	../nvm/nvmfile.c
	../nvm/nvmfile1.c
	../nvm/nvmfile2.c
	../nvm/nvmpeek1.c
	../nvm/nvmpeek2.c
	../nvm/nvmseek2.c
	)

install(TARGETS chknvm chknvm2 nvmmerge nvmsplit
	RUNTIME PERMISSIONS OWNER_READ OWNER_EXECUTE GROUP_READ GROUP_EXECUTE WORLD_READ WORLD_EXECUTE)

install(FILES chknvm.1 chknvm2.1 nvmmerge.1 nvmsplit.1
	DESTINATION ${CMAKE_INSTALL_MANDIR}/man1 COMPONENT doc)
