add_executable(config2cfg config2cfg.c
	../tools/checksum32.c
	../tools/error.c
	../tools/getoptv.c
	../tools/hexencode.c
	../tools/putoptv.c
	../tools/todigit.c
	../tools/version.c
	)
add_executable(sdram sdram.c
	../tools/checksum32.c
	)
