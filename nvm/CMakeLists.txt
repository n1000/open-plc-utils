add_executable(chknvm chknvm.c
	../nvm/fdmanifest.c
	../nvm/manifest.c
	../nvm/nvm.c
	../nvm/nvm.c
	../nvm/nvmpeek1.c
	../nvm/nvmpeek2.c
	../ram/sdrampeek.c
	../tools/checksum32.c
	../tools/error.c
	../tools/fdchecksum32.c
	../tools/getoptv.c
	../tools/putoptv.c
	../tools/strfbits.c
	../tools/version.c
	)
add_executable(chknvm2 chknvm2.c
	../nvm/manifest.c
	../nvm/nvm.c
	../nvm/nvm.c
	../nvm/nvmpeek1.c
	../nvm/nvmpeek2.c
	../tools/checksum32.c
	../tools/error.c
	../tools/getoptv.c
	../tools/putoptv.c
	../tools/strfbits.c
	../tools/version.c
	)
add_executable(nvmmerge nvmmerge.c
	../tools/checksum32.c
	../tools/error.c
	../tools/getoptv.c
	../tools/putoptv.c
	../tools/version.c
	)
add_executable(nvmsplit nvmsplit.c
	../tools/checksum32.c
	../tools/error.c
	../tools/getoptv.c
	../tools/putoptv.c
	../tools/version.c
	)
