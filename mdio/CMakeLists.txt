add_executable(mdioblock mdioblock.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(mdioblock2 mdioblock2.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(mdiodump mdiodump.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(mdiogen mdiogen.c
	$<TARGET_OBJECTS:tools>
	)
