add_executable(chkpib chkpib.c)
target_link_libraries(chkpib nvm_lib pib_lib key_lib tools_lib)

add_executable(chkpib2 chkpib2.c)
target_link_libraries(chkpib2 nvm_lib pib_lib key_lib tools_lib)

add_executable(getpib getpib.c)
target_link_libraries(getpib nvm_lib tools_lib)

add_executable(modpib modpib.c)
target_link_libraries(modpib pib_lib key_lib tools_lib)

add_executable(pib2xml pib2xml.c)
target_link_libraries(pib2xml nvm_lib nodes_lib tools_lib)

add_executable(pibcomp pibcomp.c)
target_link_libraries(pibcomp nvm_lib tools_lib)

add_executable(pibdump pibdump.c)
target_link_libraries(pibdump nvm_lib tools_lib)

add_executable(pibruin pibruin.c)
target_link_libraries(pibruin plc_lib nvm_lib tools_lib) 

add_executable(pibrump pibrump.c)
target_link_libraries(pibrump plc_lib pib_lib tools_lib) 

add_executable(psgraph psgraph.c)
target_link_libraries(psgraph pib_lib tools_lib)

add_executable(psin psin.c)
target_link_libraries(psin pib_lib tools_lib)

add_executable(pskey pskey.c)
target_link_libraries(pskey pib_lib key_lib tools_lib)

add_executable(psnotch psnotch.c)
target_link_libraries(psnotch tools_lib)

add_executable(psout psout.c)
target_link_libraries(psout pib_lib tools_lib)

add_executable(setpib setpib.c)
target_link_libraries(setpib nvm_lib tools_lib)

add_executable(xml2pib xml2pib.c)
target_link_libraries(xml2pib nodes_lib tools_lib)

add_library(pib_lib STATIC
	../pib/pibscalers.c
	../pib/pibfile.c
	../pib/pibfile1.c
	../pib/pibfile2.c
	../pib/piblock.c
	../pib/pibpeek1.c
	../pib/pibpeek2.c
	../pib/ruledump.c
	)
