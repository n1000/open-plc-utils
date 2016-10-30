add_executable(hpavkey hpavkey.c
	../key/HPAVKeyDAK.c
	../key/HPAVKeyNID.c
	../key/HPAVKeyNMK.c
	../key/HPAVKeyOut.c
	../key/HPAVKeySHA.c
	../key/SHA256Block.c
	../key/SHA256Fetch.c
	../key/SHA256Reset.c
	../key/SHA256Write.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(hpavkeys hpavkeys.c
	../key/HPAVKeyDAK.c
	../key/HPAVKeyNID.c
	../key/HPAVKeyNMK.c
	../key/HPAVKeyOut.c
	../key/HPAVKeySHA.c
	../key/SHA256Block.c
	../key/SHA256Fetch.c
	../key/SHA256Reset.c
	../key/SHA256Write.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(mac2pw mac2pw.c
	../key/MACPasswords.c
	../key/RNDPasswords.c
	../key/putpwd.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(mac2pwd mac2pwd.c
	../key/MACPasswords.c
	../key/RNDPasswords.c
	../key/putpwd.c
	$<TARGET_OBJECTS:tools>
	)
add_executable(rkey rkey.c
	../key/HPAVKeyDAK.c
	../key/HPAVKeyNID.c
	../key/HPAVKeyNMK.c
	../key/HPAVKeyOut.c
	../key/HPAVKeySHA.c
	../key/SHA256Block.c
	../key/SHA256Fetch.c
	../key/SHA256Reset.c
	../key/SHA256Write.c
	$<TARGET_OBJECTS:tools>
	)
