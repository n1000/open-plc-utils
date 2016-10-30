add_executable(chknvm chknvm.c
	../ram/sdrampeek.c
	$<TARGET_OBJECTS:nvm>
	$<TARGET_OBJECTS:tools>
	)
add_executable(chknvm2 chknvm2.c
	$<TARGET_OBJECTS:nvm>
	$<TARGET_OBJECTS:tools>
	)
add_executable(nvmmerge nvmmerge.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(nvmsplit nvmsplit.c
	$<TARGET_OBJECTS:tools>
	)

add_library(nvm OBJECT
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
