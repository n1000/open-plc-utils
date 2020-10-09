string(APPEND CMAKE_C_FLAGS " -DAR7x00")

add_executable(CMEncrypt CMEncrypt.c)
target_link_libraries(CMEncrypt lib_plc lib_key lib_ether lib_mme lib_tools)

add_executable(ampID ampID.c)
target_link_libraries(ampID lib_plc lib_ether lib_mme lib_tools)

add_executable(ampboot ampboot.c)
target_link_libraries(ampboot lib_plc lib_nvm lib_pib lib_ether lib_mme lib_tools)

add_executable(amphost amphost.c)
target_link_libraries(amphost lib_plc lib_nvm lib_pib lib_ether lib_mme lib_tools)

add_executable(amplist amplist.c)
target_link_libraries(amplist lib_plc lib_ether lib_mme lib_tools)

add_executable(amprate amprate.c)
target_link_libraries(amprate lib_plc lib_ether lib_mme lib_tools)

add_executable(amprule amprule.c)
target_link_libraries(amprule lib_plc lib_ether lib_mme lib_tools)

add_executable(ampstat ampstat.c)
target_link_libraries(ampstat lib_plc lib_ether lib_mme lib_tools)

add_executable(amptest amptest.c)
target_link_libraries(amptest lib_plc lib_nvm lib_ether lib_mme lib_tools)

add_executable(amptone amptone.c)
target_link_libraries(amptone lib_plc lib_ether lib_mme lib_tools)

add_executable(amptool amptool.c)
target_link_libraries(amptool lib_plc lib_key lib_pib lib_ram lib_nvm lib_ether lib_mme lib_tools)

add_executable(ampwait ampwait.c)
target_link_libraries(ampwait lib_plc lib_ether lib_mme lib_tools)

add_executable(coqos_add coqos_add.c)
target_link_libraries(coqos_add lib_plc lib_ether lib_mme lib_tools)

add_executable(coqos_info coqos_info.c)
target_link_libraries(coqos_info lib_plc lib_ether lib_mme lib_tools)

add_executable(coqos_man coqos_man.c)
target_link_libraries(coqos_man lib_plc lib_ether lib_mme lib_tools)

add_executable(coqos_mod coqos_mod.c)
target_link_libraries(coqos_mod lib_plc lib_ether lib_mme lib_tools)

add_executable(coqos_rel coqos_rel.c)
target_link_libraries(coqos_rel lib_plc lib_ether lib_mme lib_tools)

add_executable(int64host int64host.c)
target_link_libraries(int64host lib_plc lib_nvm lib_pib lib_ether lib_mme lib_tools)

add_executable(int6k int6k.c)
target_link_libraries(int6k lib_plc lib_nvm lib_pib lib_key lib_ram lib_ether lib_mme lib_tools)

add_executable(int6kboot int6kboot.c)
target_link_libraries(int6kboot lib_plc lib_nvm lib_pib lib_ether lib_mme lib_tools)

add_executable(int6keth int6keth.c)
target_link_libraries(int6keth lib_plc lib_ether lib_mme lib_tools)

add_executable(int6kf int6kf.c)
target_link_libraries(int6kf lib_plc lib_nvm lib_pib lib_ram lib_ether lib_mme lib_tools)

add_executable(int6khost int6khost.c)
target_link_libraries(int6khost lib_plc lib_nvm lib_pib lib_ram lib_ether lib_mme lib_tools)

add_executable(int6kid int6kid.c)
target_link_libraries(int6kid lib_plc lib_ether lib_mme lib_tools)

add_executable(int6klist int6klist.c)
target_link_libraries(int6klist lib_plc lib_ether lib_mme lib_tools)

add_executable(int6klog int6klog.c)
target_link_libraries(int6klog lib_plc lib_ether lib_mme lib_tools)

add_executable(int6kmdio int6kmdio.c)
target_link_libraries(int6kmdio lib_plc lib_ether lib_mme lib_tools)

add_executable(int6kmdio2 int6kmdio2.c)
target_link_libraries(int6kmdio2 lib_plc lib_ether lib_mme lib_tools)

add_executable(int6kmod int6kmod.c)
target_link_libraries(int6kmod lib_plc lib_ether lib_mme lib_tools)

add_executable(int6krate int6krate.c)
target_link_libraries(int6krate lib_plc lib_ether lib_mme lib_tools)

add_executable(int6krule int6krule.c)
target_link_libraries(int6krule lib_plc lib_ether lib_mme lib_tools)

add_executable(int6kstat int6kstat.c)
target_link_libraries(int6kstat lib_plc lib_ether lib_mme lib_tools)

add_executable(int6ktest int6ktest.c)
target_link_libraries(int6ktest lib_plc lib_nvm lib_ether lib_mme lib_tools)

add_executable(int6ktone int6ktone.c)
target_link_libraries(int6ktone lib_plc lib_ether lib_mme lib_tools)

add_executable(int6kwait int6kwait.c)
target_link_libraries(int6kwait lib_plc lib_ether lib_mme lib_tools)

add_executable(mdustats mdustats.c)
target_link_libraries(mdustats lib_plc lib_ether lib_mme lib_tools)

add_executable(plcID plcID.c)
target_link_libraries(plcID lib_plc lib_ether lib_mme lib_tools)

add_executable(plcboot plcboot.c)
target_link_libraries(plcboot lib_plc lib_nvm lib_pib lib_ether lib_mme lib_tools)

add_executable(plcdevs plcdevs.c)
target_link_libraries(plcdevs lib_plc lib_ether lib_mme lib_tools)

add_executable(plcfwd plcfwd.c)
target_link_libraries(plcfwd lib_plc lib_ether lib_mme lib_tools)

add_executable(plcget plcget.c)
target_link_libraries(plcget lib_plc lib_ether lib_mme lib_tools)

add_executable(plchost plchost.c)
target_link_libraries(plchost lib_plc lib_nvm lib_pib lib_ether lib_mme lib_tools)

add_executable(plchostd plchostd.c)
target_link_libraries(plchostd lib_plc lib_nvm lib_pib lib_ether lib_mme lib_tools)

add_executable(plchostd2 plchostd2.c)
target_link_libraries(plchostd2 lib_plc lib_nvm lib_pib lib_ether lib_mme lib_tools)

add_executable(plclist plclist.c)
target_link_libraries(plclist lib_plc lib_ether lib_mme lib_tools)

add_executable(plclog plclog.c)
target_link_libraries(plclog lib_plc lib_ether lib_mme lib_tools)

add_executable(plcmdio16 plcmdio16.c)
target_link_libraries(plcmdio16 lib_plc lib_ether lib_mme lib_tools)

add_executable(plcmdio32 plcmdio32.c)
target_link_libraries(plcmdio32 lib_plc lib_ether lib_mme lib_tools)

add_executable(plcotst plcotst.c)
target_link_libraries(plcotst lib_plc lib_ether lib_mme lib_tools)

add_executable(plcrate plcrate.c)
target_link_libraries(plcrate lib_plc lib_ether lib_mme lib_tools)

add_executable(plcrule plcrule.c)
target_link_libraries(plcrule lib_plc lib_ether lib_mme lib_tools)

add_executable(plcset plcset.c)
target_link_libraries(plcset lib_plc lib_ether lib_mme lib_tools)

add_executable(plcstat plcstat.c)
target_link_libraries(plcstat lib_plc lib_ether lib_mme lib_tools)

add_executable(plctest plctest.c)
target_link_libraries(plctest lib_plc lib_nvm lib_ether lib_mme lib_tools)

add_executable(plctone plctone.c)
target_link_libraries(plctone lib_plc lib_ether lib_mme lib_tools)

add_executable(plctool plctool.c)
target_link_libraries(plctool lib_plc lib_nvm lib_pib lib_key lib_ram lib_ether lib_mme lib_tools)

add_executable(plcwait plcwait.c)
target_link_libraries(plcwait lib_plc lib_ether lib_mme lib_tools)

add_executable(sada sada.c)
target_link_libraries(sada lib_plc lib_ether lib_mme lib_tools)

add_library(lib_plc STATIC
	../plc/Antiphon.c
	../plc/Attributes1.c
	../plc/Attributes2.c
	../plc/BootDevice1.c
	../plc/BootDevice2.c
	../plc/BootFirmware1.c
	../plc/BootFirmware2.c
	../plc/BootParameters1.c
	../plc/BootParameters2.c
	../plc/Confirm.c
	../plc/Display.c
	../plc/EmulateHost.c
	../plc/EmulateHost64.c
	../plc/ExecuteApplets.c
	../plc/ExecuteApplets1.c
	../plc/ExecuteApplets2.c
	../plc/FactoryDefaults.c
	../plc/Failure.c
	../plc/FlashDevice1.c
	../plc/FlashDevice2.c
	../plc/FlashFirmware.c
	../plc/FlashNVM.c
	../plc/FlashParameters.c
	../plc/FlashSoftloader.c
	../plc/GetProperty.c
	../plc/HostActionResponse.c
	../plc/Identity1.c
	../plc/Identity2.c
	../plc/InitDevice.c
	../plc/InitDevice1.c
	../plc/InitDevice2.c
	../plc/LinkStatistics.c
	../plc/LinkStatus.c
	../plc/ListLocalDevices.c
	../plc/ListRemoteDevices.c
	../plc/ListRemoteDevices1.c
	../plc/ListRemoteDevices2.c
	../plc/LocalDevices.c
	../plc/MDUTrafficStats.c
	../plc/MakeRule.c
	../plc/ModuleCommit.c
	../plc/ModuleDump.c
	../plc/ModuleRead.c
	../plc/ModuleSession.c
	../plc/ModuleSpec.c
	../plc/ModuleWrite.c
	../plc/NVMSelect.c
	../plc/NVRAMInfo.c
	../plc/NetInfo1.c
	../plc/NetInfo2.c
	../plc/NetworkInformation1.c
	../plc/NetworkInformation2.c
	../plc/NetworkTraffic1.c
	../plc/NetworkTraffic2.c
	../plc/PLCSelect.c
	../plc/PLCTopology.c
	../plc/PLCTopologyPrint.c
	../plc/ParseRule.c
	../plc/PhyRates1.c
	../plc/PhyRates2.c
	../plc/Platform.c
	../plc/PrintRule.c
	../plc/PushButton.c
	../plc/ReadFirmware1.c
	../plc/ReadFirmware2.c
	../plc/ReadMFG.c
	../plc/ReadMME.c
	../plc/ReadParameters.c
	../plc/ReadParameters1.c
	../plc/ReadParameters2.c
	../plc/ReadRules.c
	../plc/RemoteHosts.c
	../plc/Request.c
	../plc/ResetDevice.c
	../plc/RxRates2.c
	../plc/SDRAMInfo.c
	../plc/SendMME.c
	../plc/SetNMK.c
	../plc/SetProperty.c
	../plc/SignalToNoise1.c
	../plc/SignalToNoise2.c
	../plc/SlaveMembership.c
	../plc/StartDevice1.c
	../plc/StartFirmware1.c
	../plc/StationRole.c
	../plc/ToneMaps1.c
	../plc/ToneMaps2.c
	../plc/Topology1.c
	../plc/Topology2.c
	../plc/Traffic1.c
	../plc/Traffic2.c
	../plc/Transmit.c
	../plc/UpgradeDevice1.c
	../plc/VersionInfo1.c
	../plc/VersionInfo2.c
	../plc/WaitForReset.c
	../plc/WaitForRestart.c
	../plc/WaitForStart.c
	../plc/WatchdogReport.c
	../plc/WriteCFG.c
	../plc/WriteExecuteApplet2.c
	../plc/WriteExecuteFirmware1.c
	../plc/WriteExecuteFirmware2.c
	../plc/WriteExecutePIB.c
	../plc/WriteExecuteParameters2.c
	../plc/WriteFirmware1.c
	../plc/WriteMEM.c
	../plc/WriteNVM.c
	../plc/WritePIB.c
	../plc/chipset.c
	../plc/rules.c
	)
