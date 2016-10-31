add_executable(hpavkey hpavkey.c)
target_link_libraries(hpavkey key_lib tools_lib)

add_executable(hpavkeys hpavkeys.c)
target_link_libraries(hpavkeys key_lib tools_lib)

add_executable(mac2pw mac2pw.c)
target_link_libraries(mac2pw key_lib tools_lib)

add_executable(mac2pwd mac2pwd.c)
target_link_libraries(mac2pwd key_lib tools_lib)

add_executable(rkey rkey.c)
target_link_libraries(rkey key_lib tools_lib)

add_library(key_lib STATIC
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
