add_executable(hpav hpav.c
	../mme/MMEMode.c
	../mme/MMEName.c
	../mme/MMEPeek.c
	$<TARGET_OBJECTS:ether>
	$<TARGET_OBJECTS:tools>
	)
add_executable(mme mme.c
	../mme/MMEMode.c
	../mme/MMEName.c
	$<TARGET_OBJECTS:tools>
	)
