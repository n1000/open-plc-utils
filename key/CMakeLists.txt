add_executable(hpavkey hpavkey.c)
target_link_libraries(hpavkey lib_key lib_tools)

add_executable(hpavkeys hpavkeys.c)
target_link_libraries(hpavkeys lib_key lib_tools)

add_executable(mac2pw mac2pw.c)
target_link_libraries(mac2pw lib_key lib_tools)

add_executable(mac2pwd mac2pwd.c)
target_link_libraries(mac2pwd lib_key lib_tools)

add_executable(rkey rkey.c)
target_link_libraries(rkey lib_key lib_tools)

add_library(lib_key STATIC
	../key/HPAVKeyDAK.c
	../key/HPAVKeyNID.c
	../key/HPAVKeyNMK.c
	../key/HPAVKeyOut.c
	../key/HPAVKeySHA.c
	../key/MACPasswords.c
	../key/RNDPasswords.c
	../key/SHA256Block.c
	../key/SHA256Fetch.c
	../key/SHA256Reset.c
	../key/SHA256Write.c
	../key/keys.c
	../key/putpwd.c
	)
