# ultinject_krnl
A secure driver-interface for moder BE/EAC versions. The kernelmode code gets executed by the UM-process that calls gHalDispatchTable[1] (hooked by the driver on load)

  -dll-injection capabilities
  
  -km-um communication using a small "shared" memory buffer within the usermode process
  
  -clearing traces of the unloaded vulnerable driver

this whole shit is coded by me and was ALOT OF WORK. so pls treat it with respect xD

credits to @fisherprice from UC for cleaning MmUnloadedDrivers & PiDDBCacheTable structures (signatures should at least work for 1803-1903)
