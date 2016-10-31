add_executable(mdioblock mdioblock.c)
target_link_libraries(mdioblock lib_tools)

add_executable(mdioblock2 mdioblock2.c)
target_link_libraries(mdioblock2 lib_tools)

add_executable(mdiodump mdiodump.c)
target_link_libraries(mdiodump lib_tools)

add_executable(mdiogen mdiogen.c)
target_link_libraries(mdiogen lib_tools)
