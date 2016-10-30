add_executable(int6kbaud int6kbaud.c
	../serial/closeport.c
	../serial/openport.c
	../serial/serial.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(int6kdetect int6kdetect.c
	../serial/baudrate.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(int6kuart int6kuart.c
	../serial/closeport.c
	../serial/openport.c
	../serial/serial.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(ptsctl ptsctl.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(ttycat ttycat.c
	../serial/baudrate.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(ttyrecv ttyrecv.c
	../serial/baudrate.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(ttysend ttysend.c
	../serial/baudrate.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(ttysig ttysig.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(weeder weeder.c
	$<TARGET_OBJECTS:tools>
	)
