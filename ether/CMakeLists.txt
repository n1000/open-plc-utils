add_executable(edru edru.c)
target_link_libraries(edru lib_ether lib_tools)

add_executable(edsu edsu.c)
target_link_libraries(edsu lib_ether lib_tools)

add_executable(efbu efbu.c)
target_link_libraries(efbu lib_ether lib_tools)

add_executable(efeu efeu.c)
target_link_libraries(efeu lib_ether lib_tools)

add_executable(efru efru.c)
target_link_libraries(efru lib_ether lib_tools)

add_executable(efsu efsu.c)
target_link_libraries(efsu lib_ether lib_tools)

add_executable(nics nics.c)
target_link_libraries(nics lib_ether lib_tools)

add_library(lib_ether STATIC
	../ether/channel.c
	../ether/closechannel.c
	../ether/hostnics.c
	../ether/initchannel.c
	../ether/openchannel.c
	../ether/readpacket.c
	../ether/sendpacket.c
	)

install(TARGETS edru edsu efbu efeu efru efsu nics
	RUNTIME PERMISSIONS OWNER_READ OWNER_EXECUTE GROUP_READ GROUP_EXECUTE WORLD_READ WORLD_EXECUTE SETUID)

install(FILES edru.1 edsu.1 efbu.1 efeu.1 efru.1 efsu.1 nics.1
	DESTINATION ${CMAKE_INSTALL_MANDIR}/man1 COMPONENT doc)
