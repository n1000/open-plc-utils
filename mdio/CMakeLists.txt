add_executable(mdioblock mdioblock.c)
target_link_libraries(mdioblock tools_lib)

add_executable(mdioblock2 mdioblock2.c)
target_link_libraries(mdioblock2 tools_lib)

add_executable(mdiodump mdiodump.c)
target_link_libraries(mdiodump tools_lib)

add_executable(mdiogen mdiogen.c)
target_link_libraries(mdiogen tools_lib)
