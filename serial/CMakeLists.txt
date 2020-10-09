add_executable(int6kbaud int6kbaud.c)
target_link_libraries(int6kbaud lib_serial lib_tools)

add_executable(int6kdetect int6kdetect.c)
target_link_libraries(int6kdetect lib_serial lib_tools)

add_executable(int6kuart int6kuart.c)
target_link_libraries(int6kuart lib_serial lib_tools)

add_executable(ptsctl ptsctl.c)
target_link_libraries(ptsctl lib_tools)

add_executable(ttycat ttycat.c)
target_link_libraries(ttycat lib_serial lib_tools)

add_executable(ttyrecv ttyrecv.c)
target_link_libraries(ttyrecv lib_serial lib_tools)

add_executable(ttysend ttysend.c)
target_link_libraries(ttysend lib_serial lib_tools)

add_executable(ttysig ttysig.c)
target_link_libraries(ttysig lib_tools)

add_executable(weeder weeder.c)
target_link_libraries(weeder lib_tools)

add_library(lib_serial STATIC
	../serial/baudrate.c
	../serial/closeport.c
	../serial/openport.c
	../serial/serial.c
	)

install(TARGETS int6kbaud int6kdetect int6kuart ptsctl ttycat ttyrecv ttysend ttysig weeder
	RUNTIME PERMISSIONS OWNER_READ OWNER_EXECUTE GROUP_READ GROUP_EXECUTE WORLD_READ WORLD_EXECUTE)

install(FILES int6kbaud.1 int6kdetect.1 int6kuart.1 ptsctl.1 ttycat.1 ttyrecv.1 ttysend.1 ttysig.1 weeder.1
	DESTINATION ${CMAKE_INSTALL_MANDIR}/man1 COMPONENT doc)
