string(APPEND CMAKE_C_FLAGS " -DINT6x00")

add_executable(mdioblock mdioblock.c)
target_link_libraries(mdioblock lib_tools)

add_executable(mdioblock2 mdioblock2.c)
target_link_libraries(mdioblock2 lib_tools)

add_executable(mdiodump mdiodump.c)
target_link_libraries(mdiodump lib_tools)

add_executable(mdiogen mdiogen.c)
target_link_libraries(mdiogen lib_tools)

install(TARGETS mdioblock mdioblock2 mdiodump mdiogen
	RUNTIME PERMISSIONS OWNER_READ OWNER_EXECUTE GROUP_READ GROUP_EXECUTE WORLD_READ WORLD_EXECUTE)

install(FILES mdioblock.1 mdioblock2.1 mdiodump.1 mdiogen.1
	DESTINATION ${CMAKE_INSTALL_MANDIR}/man1 COMPONENT doc)
