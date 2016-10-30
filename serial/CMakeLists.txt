add_executable(int6kbaud int6kbaud.c
	../serial/closeport.c
	../serial/openport.c
	../serial/serial.c
	../tools/error.c
	../tools/getoptv.c
	../tools/putoptv.c
	../tools/synonym.c
	../tools/todigit.c
	../tools/uintspec.c
	../tools/version.c
	)
add_executable(int6kdetect int6kdetect.c
	../serial/baudrate.c
	../tools/error.c
	../tools/getoptv.c
	../tools/putoptv.c
	../tools/version.c
	)
add_executable(int6kuart int6kuart.c
	../serial/closeport.c
	../serial/openport.c
	../serial/serial.c
	../tools/basespec.c
	../tools/checksum32.c
	../tools/error.c
	../tools/getoptv.c
	../tools/hexdecode.c
	../tools/hexencode.c
	../tools/hexstring.c
	../tools/putoptv.c
	../tools/todigit.c
	../tools/uintspec.c
	../tools/version.c
	)
add_executable(ptsctl ptsctl.c
	../tools/error.c
	../tools/getoptv.c
	../tools/putoptv.c
	../tools/synonym.c
	../tools/todigit.c
	../tools/uintspec.c
	../tools/version.c
	)
add_executable(ttycat ttycat.c
	../serial/baudrate.c
	../tools/efreopen.c
	../tools/error.c
	../tools/getoptv.c
	../tools/putoptv.c
	../tools/todigit.c
	../tools/uintspec.c
	../tools/version.c
	)
add_executable(ttyrecv ttyrecv.c
	../serial/baudrate.c
	../tools/error.c
	../tools/getoptv.c
	../tools/putoptv.c
	../tools/todigit.c
	../tools/uintspec.c
	../tools/version.c
	)
add_executable(ttysend ttysend.c
	../serial/baudrate.c
	../tools/error.c
	../tools/getoptv.c
	../tools/putoptv.c
	../tools/todigit.c
	../tools/uintspec.c
	../tools/version.c
	)
add_executable(ttysig ttysig.c
	../tools/error.c
	../tools/getoptv.c
	../tools/putoptv.c
	../tools/todigit.c
	../tools/uintspec.c
	../tools/version.c
	)
add_executable(weeder weeder.c
	../tools/error.c
	../tools/getoptv.c
	../tools/putoptv.c
	../tools/synonym.c
	../tools/todigit.c
	../tools/uintspec.c
	../tools/version.c
	)
