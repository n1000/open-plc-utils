add_executable(chkpib chkpib.c
	../key/HPAVKeyNID.c
	../key/SHA256Block.c
	../key/SHA256Fetch.c
	../key/SHA256Reset.c
	../key/SHA256Write.c
	../key/keys.c
	../pib/pibpeek1.c
	../pib/pibpeek2.c
	$<TARGET_OBJECTS:nvm>
	$<TARGET_OBJECTS:tools>
	)
add_executable(chkpib2 chkpib2.c
	../key/HPAVKeyNID.c
	../key/SHA256Block.c
	../key/SHA256Fetch.c
	../key/SHA256Reset.c
	../key/SHA256Write.c
	../key/keys.c
	../pib/pibpeek1.c
	../pib/pibpeek2.c
	$<TARGET_OBJECTS:nvm>
	$<TARGET_OBJECTS:tools>
	)
add_executable(getpib getpib.c
	$<TARGET_OBJECTS:nvm>
	$<TARGET_OBJECTS:tools>
	)
add_executable(modpib modpib.c
	../key/HPAVKeyNID.c
	../key/SHA256Block.c
	../key/SHA256Fetch.c
	../key/SHA256Reset.c
	../key/SHA256Write.c
	../key/keys.c
	../key/keys.c
	../pib/pibpeek1.c
	../pib/pibpeek2.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(pib2xml pib2xml.c
	../nodes/xmlschema.c
	$<TARGET_OBJECTS:nvm>
	$<TARGET_OBJECTS:tools>
	)
add_executable(pibcomp pibcomp.c
	$<TARGET_OBJECTS:nvm>
	$<TARGET_OBJECTS:tools>
	)
add_executable(pibdump pibdump.c
	$<TARGET_OBJECTS:nvm>
	$<TARGET_OBJECTS:tools>
	)
add_executable(pibruin pibruin.c
	$<TARGET_OBJECTS:plc>
	$<TARGET_OBJECTS:nvm>
	$<TARGET_OBJECTS:tools>
	)
add_executable(pibrump pibrump.c
	../pib/pibfile1.c
	$<TARGET_OBJECTS:plc>
	$<TARGET_OBJECTS:tools>
	)
add_executable(psgraph psgraph.c
	../pib/pibscalers.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(psin psin.c
	../pib/pibfile1.c
	../pib/piblock.c
	../pib/pibscalers.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(pskey pskey.c
	../key/SHA256Block.c
	../key/SHA256Fetch.c
	../key/SHA256Reset.c
	../key/SHA256Write.c
	../pib/pibfile1.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(psnotch psnotch.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(psout psout.c
	../pib/pibfile.c
	../pib/pibfile1.c
	../pib/pibfile2.c
	../pib/pibscalers.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(setpib setpib.c
	$<TARGET_OBJECTS:nvm>
	$<TARGET_OBJECTS:tools>
	)
add_executable(xml2pib xml2pib.c
	../nodes/xmledit.c
	../nodes/xmlfree.c
	../nodes/xmlnode.c
	../nodes/xmlopen.c
	../nodes/xmlscan.c
	../nodes/xmltree.c
	$<TARGET_OBJECTS:tools>
	)
