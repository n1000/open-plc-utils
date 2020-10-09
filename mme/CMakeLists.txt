add_executable(hpav hpav.c)
target_link_libraries(hpav lib_mme lib_ether lib_tools)

add_executable(mme mme.c)
target_link_libraries(mme lib_mme lib_tools)

add_library(lib_mme STATIC
	../mme/ARPCPrint.c
	../mme/Devices.c
	../mme/EthernetHeader.c
	../mme/FirmwareMessage.c
	../mme/HomePlugHeader.c
	../mme/HomePlugHeader1.c
	../mme/MMECode.c
	../mme/MMEMode.c
	../mme/MMEName.c
	../mme/MMEPeek.c
	../mme/QualcommHeader.c
	../mme/QualcommHeader1.c
	../mme/UnwantedMessage.c
	../mme/readmessage.c
	../mme/sendmessage.c
	)

install(TARGETS hpav
	RUNTIME PERMISSIONS OWNER_READ OWNER_EXECUTE GROUP_READ GROUP_EXECUTE WORLD_READ WORLD_EXECUTE SETUID)

install(TARGETS mme
	RUNTIME PERMISSIONS OWNER_READ OWNER_EXECUTE GROUP_READ GROUP_EXECUTE WORLD_READ WORLD_EXECUTE)

install(FILES hpav.1 mme.1
	DESTINATION ${CMAKE_INSTALL_MANDIR}/man1 COMPONENT doc)
