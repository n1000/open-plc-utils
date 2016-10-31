add_executable(edru edru.c
	)
target_link_libraries(edru ether_lib tools_lib)
add_executable(edsu edsu.c
	)
target_link_libraries(edsu ether_lib tools_lib)
add_executable(efbu efbu.c
	)
target_link_libraries(efbu ether_lib tools_lib)
add_executable(efeu efeu.c
	)
target_link_libraries(efeu ether_lib tools_lib)
add_executable(efru efru.c
	)
target_link_libraries(efru ether_lib tools_lib)
add_executable(efsu efsu.c
	)
target_link_libraries(efsu ether_lib tools_lib)
add_executable(nics nics.c
	)
target_link_libraries(nics ether_lib tools_lib)

add_library(ether_lib STATIC
	../ether/channel.c
	../ether/closechannel.c
	../ether/hostnics.c
	../ether/openchannel.c
	../ether/readpacket.c
	../ether/sendpacket.c
	)
