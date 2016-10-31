add_executable(hpav hpav.c)
target_link_libraries(hpav mme_lib ether_lib tools_lib)

add_executable(mme mme.c)
target_link_libraries(mme mme_lib tools_lib)

add_library(mme_lib STATIC
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
