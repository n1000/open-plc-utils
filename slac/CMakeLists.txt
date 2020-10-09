add_executable(evse evse.c)
target_link_libraries(evse lib_plc lib_slac lib_mme lib_ether lib_tools)

add_executable(pev pev.c)
target_link_libraries(pev lib_plc lib_slac lib_mme lib_ether lib_tools)

add_library(lib_slac STATIC
	../slac/evse_cm_atten_char.c
	../slac/evse_cm_mnbc_sound.c
	../slac/evse_cm_set_key.c
	../slac/evse_cm_slac_match.c
	../slac/evse_cm_slac_param.c
	../slac/evse_cm_start_atten_char.c
	../slac/pev_cm_atten_char.c
	../slac/pev_cm_mnbc_sound.c
	../slac/pev_cm_set_key.c
	../slac/pev_cm_slac_match.c
	../slac/pev_cm_slac_param.c
	../slac/pev_cm_start_atten_char.c
	../slac/slac_connect.c
	../slac/slac_debug.c
	../slac/slac_session.c
	)

install(TARGETS evse pev
	RUNTIME PERMISSIONS OWNER_READ OWNER_EXECUTE GROUP_READ GROUP_EXECUTE WORLD_READ WORLD_EXECUTE SETUID)

install(FILES evse.1 pev.1
	DESTINATION ${CMAKE_INSTALL_MANDIR}/man1 COMPONENT doc)
