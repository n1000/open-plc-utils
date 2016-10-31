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
