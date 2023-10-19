
*Problem*: make host -> fatal error: experimental/xrt_aie.h: No such file or directory

*Solution*: source /opt/petalinux/2022.2/environment-setup-cortexa72-cortexa53-xilinx-linux

# 

*Problem*: AIE license not found!

 *Solution*: 
 Set fixed MAC addr for WSL so that Vivado AIE license will work using standalone license. Set MAC addr to match license:
 Use ``ip link`` to create a dummy address which matches the AIE license file.
 
    sudo ip link add vmnic0 type dummy ; sudo ip link set vmnic0 addr 00:15:5d:d9:3b:65

#
