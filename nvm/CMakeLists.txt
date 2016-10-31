add_executable(chknvm chknvm.c)
target_link_libraries(chknvm nvm_lib ram_lib tools_lib)

add_executable(chknvm2 chknvm2.c)
target_link_libraries(chknvm2 nvm_lib tools_lib)

add_executable(nvmmerge nvmmerge.c)
target_link_libraries(nvmmerge tools_lib)

add_executable(nvmsplit nvmsplit.c)
target_link_libraries(nvmsplit tools_lib)

add_library(nvm_lib STATIC
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
