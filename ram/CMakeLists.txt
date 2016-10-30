add_executable(config2cfg config2cfg.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(sdram sdram.c
	$<TARGET_OBJECTS:tools>
	)
