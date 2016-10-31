add_executable(evse evse.c)
target_link_libraries(evse plc_lib slac_lib mme_lib ether_lib tools_lib)

add_executable(pev pev.c)
target_link_libraries(pev plc_lib slac_lib mme_lib ether_lib tools_lib)

add_library(slac_lib STATIC
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
	../slac/slac_structs.c
	)
