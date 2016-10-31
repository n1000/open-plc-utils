add_executable(chkpib chkpib.c)
target_link_libraries(chkpib lib_nvm lib_pib lib_key lib_tools)

add_executable(chkpib2 chkpib2.c)
target_link_libraries(chkpib2 lib_nvm lib_pib lib_key lib_tools)

add_executable(getpib getpib.c)
target_link_libraries(getpib lib_nvm lib_tools)

add_executable(modpib modpib.c)
target_link_libraries(modpib lib_pib lib_key lib_tools)

add_executable(pib2xml pib2xml.c)
target_link_libraries(pib2xml lib_nvm lib_nodes lib_tools)

add_executable(pibcomp pibcomp.c)
target_link_libraries(pibcomp lib_nvm lib_tools)

add_executable(pibdump pibdump.c)
target_link_libraries(pibdump lib_nvm lib_tools)

add_executable(pibruin pibruin.c)
target_link_libraries(pibruin lib_plc lib_nvm lib_tools) 

add_executable(pibrump pibrump.c)
target_link_libraries(pibrump lib_plc lib_pib lib_tools) 

add_executable(psgraph psgraph.c)
target_link_libraries(psgraph lib_pib lib_tools)

add_executable(psin psin.c)
target_link_libraries(psin lib_pib lib_tools)

add_executable(pskey pskey.c)
target_link_libraries(pskey lib_pib lib_key lib_tools)

add_executable(psnotch psnotch.c)
target_link_libraries(psnotch lib_tools)

add_executable(psout psout.c)
target_link_libraries(psout lib_pib lib_tools)

add_executable(setpib setpib.c)
target_link_libraries(setpib lib_nvm lib_tools)

add_executable(xml2pib xml2pib.c)
target_link_libraries(xml2pib lib_nodes lib_tools)

add_library(lib_pib STATIC
	../pib/pibscalers.c
	../pib/pibfile.c
	../pib/pibfile1.c
	../pib/pibfile2.c
	../pib/piblock.c
	../pib/pibpeek1.c
	../pib/pibpeek2.c
	../pib/ruledump.c
	)
