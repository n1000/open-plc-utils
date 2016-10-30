add_executable(edru edru.c
	$<TARGET_OBJECTS:ether>
	$<TARGET_OBJECTS:tools>
	)
add_executable(edsu edsu.c
	$<TARGET_OBJECTS:ether>
	$<TARGET_OBJECTS:tools>
	)
add_executable(efbu efbu.c
	$<TARGET_OBJECTS:ether>
	$<TARGET_OBJECTS:tools>
	)
add_executable(efeu efeu.c
	$<TARGET_OBJECTS:ether>
	$<TARGET_OBJECTS:tools>
	)
add_executable(efru efru.c
	$<TARGET_OBJECTS:ether>
	$<TARGET_OBJECTS:tools>
	)
add_executable(efsu efsu.c
	$<TARGET_OBJECTS:ether>
	$<TARGET_OBJECTS:tools>
	)
add_executable(nics nics.c
	$<TARGET_OBJECTS:ether>
	$<TARGET_OBJECTS:tools>
	)

add_library(ether OBJECT
	../ether/channel.c
	../ether/closechannel.c
	../ether/hostnics.c
	../ether/openchannel.c
	../ether/readpacket.c
	../ether/sendpacket.c
	)
