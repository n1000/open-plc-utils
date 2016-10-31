add_executable(int6kbaud int6kbaud.c)
target_link_libraries(int6kbaud serial_lib tools_lib)

add_executable(int6kdetect int6kdetect.c)
target_link_libraries(int6kdetect serial_lib tools_lib)

add_executable(int6kuart int6kuart.c)
target_link_libraries(int6kuart serial_lib tools_lib)

add_executable(ptsctl ptsctl.c)
target_link_libraries(ptsctl tools_lib)

add_executable(ttycat ttycat.c)
target_link_libraries(ttycat serial_lib tools_lib)

add_executable(ttyrecv ttyrecv.c)
target_link_libraries(ttyrecv serial_lib tools_lib)

add_executable(ttysend ttysend.c)
target_link_libraries(ttysend serial_lib tools_lib)

add_executable(ttysig ttysig.c)
target_link_libraries(ttysig tools_lib)

add_executable(weeder weeder.c)
target_link_libraries(weeder tools_lib)

add_library(serial_lib STATIC
	../serial/baudrate.c
	../serial/closeport.c
	../serial/openport.c
	../serial/serial.c
	)
