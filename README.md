#!/bin/bash

# nvOC v0018 by fullzero
#
# + contributors:
#
# IAmNotAJeep: IAmNotAJeep_and_Maxximus007_WATCHDOG
# IAmNotAJeep BTC address:  13PnEKpfVzNseWkrm6LoueKcCMPj74zPv7
#
# Maxximus007: Maxximus007_AUTO_TEMPERATURE_CONTROL / expectless oneBash / WATCHDOG
# Maxximus007 BTC address:  1JAFefdPVAs3WQiTqnYWbsjifJAEjQcjQ8
#
# _Parallax_:  _Parallax_ Mode ( wget + pastebin oneBash updating )
# _Parallax_ BTC address:  329k8rDgxHHcHAEXfwznqv25Go5LERGWLp
#
# salfter: SALFTER_NICEHASH_PROFIT_SWITCHING
# salfter BTC address:  1TipsGocnz2N5qgAm9f7JLrsMqkb3oXe2
#
# xleejohnx: SRR support
# xleejohnx BTC address:  1EY5WbiW3YkWanSKEGcjCETpQfCR81wc56
#
#
# Open a terminal to launch miner; will auto launch on boot
#
# firefox has an OP bookmark; look at the OP for more information
#
# click the Desktop Sharing icon on the left for RDP 
#
# your rig IP displays at beginning of mining process
#
# worker names will default to nvXYZ your rig host address (last 3 digits of rig IP)
#
# if your rig host address is less than 100 it will default to nv0XX or nv0X
#
# USE ALL CAPS
#
# CHOOSE COIN FROM:
# DMD  GRS  ZPOOL_LYRA2V2  ZPOOL_BLAKE2S
# ZEC   ZCOIN  HUSH   ZEN  ZCL  
# NICE_ETHASH  ETH    MUSIC  ETC  EXP  DCR  PASC
# MONA  VTC    DGB    SIA  FTC  LBC  
# DUAL_ETC_DCR    DUAL_ETC_PASC    DUAL_ETC_LBC    DUAL_ETC_SC
# DUAL_EXP_DCR    DUAL_EXP_PASC    DUAL_EXP_LBC    DUAL_EXP_SC
# DUAL_ETH_DCR    DUAL_ETH_PASC    DUAL_ETH_LBC    DUAL_ETH_SC
# DUAL_MUSIC_DCR  DUAL_MUSIC_PASC  DUAL_MUSIC_LBC  DUAL_MUSIC_SC

COIN="ETH"

SALFTER_NICEHASH_PROFIT_SWITCHING="NO"

Maxximus007_AUTO_TEMPERATURE_CONTROL="NO"

IAmNotAJeep_and_Maxximus007_WATCHDOG="YES"

# LOCAL will attach the mining process to the gnome or guake terminal
# REMOTE will leave it unattached / ready for SSH 
LOCALorREMOTE="LOCAL"       # LOCAL  or  REMOTE

SRR="NO"                       # YES NO

SRR_SERIAL="000055"
__SRR_SLOT="1"

TEAMVIEWER="YES"                 # YES NO

SSH="YES"                       # YES NO

AUTO_REBOOT="NO"

REBOOT_TIMEOUT_IN_MINUTES=1440   # every 24 hours

POWERLIMIT="YES"              	# YES NO

POWERLIMIT_WATTS=125

__CORE_OVERCLOCK=-200
MEMORY_OVERCLOCK=875

MANUAL_FAN="YES"             	# YES NO

# Set fan speed if MANUAL_FAN="YES"
FAN_SPEED=75

# If you are using a slow USB Key
SLOW_USB_KEY_MODE="YES"        	# YES NO

# Mine XMR with CPU
plusCPU="NO"		        # YES NO

# Number of threads for plusCPU
threadCOUNT="1"                 # varies per CPU

GPUPowerMizerMode_Adjust="YES"

# Set PowerMizerMode
GPUPowerMizerMode=1


INDIVIDUAL_CLOCKS="NO"      	# YES NO

# Set individual clocks here if INDIVIDUAL_CLOCKS="YES"
__CORE_OVERCLOCK_0=100
MEMORY_OVERCLOCK_0=100

__CORE_OVERCLOCK_1=100
MEMORY_OVERCLOCK_1=100

__CORE_OVERCLOCK_2=100
MEMORY_OVERCLOCK_2=100

__CORE_OVERCLOCK_3=100
MEMORY_OVERCLOCK_3=100

__CORE_OVERCLOCK_4=100
MEMORY_OVERCLOCK_4=100

__CORE_OVERCLOCK_5=100
MEMORY_OVERCLOCK_5=100

__CORE_OVERCLOCK_6=100
MEMORY_OVERCLOCK_6=100

__CORE_OVERCLOCK_7=100
MEMORY_OVERCLOCK_7=100

__CORE_OVERCLOCK_8=100
MEMORY_OVERCLOCK_8=100

__CORE_OVERCLOCK_9=100
MEMORY_OVERCLOCK_9=100

__CORE_OVERCLOCK_10=100
MEMORY_OVERCLOCK_10=100

__CORE_OVERCLOCK_11=100
MEMORY_OVERCLOCK_11=100

__CORE_OVERCLOCK_12=100
MEMORY_OVERCLOCK_12=100

__CORE_OVERCLOCK_13=100
MEMORY_OVERCLOCK_13=100


INDIVIDUAL_POWERLIMIT="NO"   	# YES NO

# Set individual powerlimits here if INDIVIDUAL_POWERLIMIT="YES"

# or if using Maxximus007_AUTO_TEMPERATURE_CONTROL

#######################################################################################


# Maxximus007_AUTO_TEMPERATURE_CONTROL


INDIVIDUAL_POWERLIMIT_0=125

INDIVIDUAL_POWERLIMIT_1=125

INDIVIDUAL_POWERLIMIT_2=125

INDIVIDUAL_POWERLIMIT_3=125

INDIVIDUAL_POWERLIMIT_4=125

INDIVIDUAL_POWERLIMIT_5=125

INDIVIDUAL_POWERLIMIT_6=125

INDIVIDUAL_POWERLIMIT_7=125

INDIVIDUAL_POWERLIMIT_8=125

INDIVIDUAL_POWERLIMIT_9=125

INDIVIDUAL_POWERLIMIT_10=125

INDIVIDUAL_POWERLIMIT_11=125

INDIVIDUAL_POWERLIMIT_12=125

INDIVIDUAL_POWERLIMIT_13=125

# Set the target temperature per card.

# Don't set it too low, if the temperature can't be reached with fan adjustments it will decrease power.

# Recommended ranges: 55 - 70 degrees Celsius

# If actual temp is above the target temp this script will up the fan speed

TARGET_TEMP_0=70

TARGET_TEMP_1=70

TARGET_TEMP_2=70

TARGET_TEMP_3=70

TARGET_TEMP_4=70

TARGET_TEMP_5=70

TARGET_TEMP_6=70

TARGET_TEMP_7=70

TARGET_TEMP_8=70

TARGET_TEMP_9=70

TARGET_TEMP_10=70

TARGET_TEMP_11=70

TARGET_TEMP_12=70

TARGET_TEMP_13=70


# If actual temp is above value set above and fan speed is 100,
# the script will lower the power limit

# SET INDIVIDUAL POWERLIMITS ABOVE


# Adjustment size (FAN in percent, POWER in Watts)
__FAN_ADJUST=5
POWER_ADJUST=5

# Difference in actual temperature allowed before action.
#Works only if current is BELOW target temp
ALLOWED_TEMP_DIFF=3

# Restore original power limit if fan speed is lower than this percentage
RESTORE_POWER_LIMIT=80


# IP as worker implementation
########################################################################################
IPW=$(ifconfig | sed -En 's/127.0.0.1//;s/.*inet (addr:)?(([0-9]*\.){3}[0-9]*).*/\2/p')
echo ""
echo ""
# using only host address
IP_AS_WORKER=$(echo -n $IPW | tail -c -3 | sed 'y/./0/')
# for_full_IP with - instead of .
#IP_AS_WORKER=$(echo $IPW | sed 'y/./-/')
echo workername: nv$IP_AS_WORKER
########################################################################################

# useful cmds when using SALFTER_NICEHASH_PROFIT_SWITCHING:
# ps aux | grep miner
# screen -r miner
# pkill -e miner

# SALFTER_NICEHASH_PROFIT_SWITCHING

CURRENCY=USD

POWER_COST=0.10

MINIMUM_PROFIT=0.0

# this is salfters BTC address:  1TipsGocnz2N5qgAm9f7JLrsMqkb3oXe2

PAYMENT_ADDRESS=1TipsGocnz2N5qgAm9f7JLrsMqkb3oXe2

WORKER_NAME=nv$IP_AS_WORKER

PROFIT_CHECK_TIMEOUT=600


# USE Maxximus007_AUTO_TEMPERATURE_CONTROL for fanspeed


daggerhashimoto_POWERLIMIT_WATTS=125
__daggerhashimoto_CORE_OVERCLOCK=-200
daggerhashimoto_MEMORY_OVERCLOCK=900

equihash_POWERLIMIT_WATTS=125
__equihash_CORE_OVERCLOCK=100
equihash_MEMORY_OVERCLOCK=100

neoscrypt_POWERLIMIT_WATTS=125
__neoscrypt_CORE_OVERCLOCK=100
neoscrypt_MEMORY_OVERCLOCK=100

lyra2rev2_POWERLIMIT_WATTS=125
__lyra2rev2_CORE_OVERCLOCK=100
lyra2rev2_MEMORY_OVERCLOCK=100

lbry_POWERLIMIT_WATTS=125
__lbry_CORE_OVERCLOCK=100
lbry_MEMORY_OVERCLOCK=100

########################################################################################


# set YOUR ADDRESSES, WORKERS, POOL and PORT:
ZEC_WORKER="nv$IP_AS_WORKER"
ZEC_ADDRESS="t1XfkZUZWME8FnRiFxHZQAQ2K1UdQMbshJp"
ZEC_POOL="zec-us-east1.nanopool.org"
ZEC_PORT="6666"


EWBF_VERSION="3_4"  # choose 3_3  or  3_4

# change EWBF_PERCENT to alter donation percent for EWBF Miner
EWBF_PERCENT=0


ZCL_WORKER="nv$IP_AS_WORKER"
ZCL_ADDRESS="fullzero22"
ZCL_POOL="zcl.coinmine.pl"
ZCL_PORT="7007"

ZEN_WORKER="nv$IP_AS_WORKER"
ZEN_ADDRESS="znictSisUCALijmhJrjLS8FozvcJRAiHc29"
ZEN_POOL="us.zenmine.pro"
ZEN_PORT="9009"

HUSH_WORKER="nv$IP_AS_WORKER"
HUSH_ADDRESS="fullzero22"
HUSH_POOL="zdash.suprnova.cc"
HUSH_PORT="4048"

ZCOIN_WORKER="nv$IP_AS_WORKER"
ZCOIN_ADDRESS="fullzero22"
ZCOIN_POOL="stratum+tcp://xzc.suprnova.cc:1569"


# ZPOOL uses your BTC_ADDRESS
ZPOOL_LYRA2V2_POOL="stratum+tcp://lyra2v2.mine.zpool.ca:4533"


# ZPOOL uses your BTC_ADDRESS
ZPOOL_BLAKE2S_POOL="stratum+tcp://blake2s.mine.zpool.ca:5766"


DMD_WORKER="nv$IP_AS_WORKER"
DMD_ADDRESS="fullzero"
DMD_POOL="stratum+tcp://us.miningfield.com:3376"

GRS_WORKER="nv$IP_AS_WORKER"
GRS_ADDRESS="FnN3tyehFmkKgw75qu4GnbgmWxCrARbu8t"
GRS_POOL="stratum+tcp://erebor.dwarfpool.com:3345"

MONA_WORKER="nv$IP_AS_WORKER"
MONA_ADDRESS="fullzero22"
MONA_POOL="stratum+tcp://mona.suprnova.cc:2995"

# if YES ensure you update BTC_ADDRESS
VTC_AUTOCONVERT_TO_BTC="YES"        #YES  NO
VTC_WORKER="nv$IP_AS_WORKER"
VTC_ADDRESS="VsvtYL2mz3YFM3fpt5pb28zHodTbnJodRc"
VTC_POOL="stratum+tcp://lyra2v2.mine.zpool.ca:4533"


BTC_ADDRESS="18Y5HYe3BAwAhTAkFLbD52o8NqtrN3DtpF"


# NICE_ETHASH autoconverts to BTC: ensure you update BTC_ADDRESS if you use NICE_ETHASH
NICE_ETHASH_WORKER="nv$IP_AS_WORKER"
NICE_ETHASH_POOL="stratum+tcp://daggerhashimoto.usa.nicehash.com:3353"
GENOIL_NICE_ETHASH_POOL="daggerhashimoto.usa.nicehash.com:3353"
NICE_ETHASH_EXTENTION_ARGUMENTS=""   # add any additional claymore arguments desired here

# if YES ensure you update BTC_ADDRESS
DGB_AUTOCONVERT_TO_BTC="YES"        #YES  NO
DGB_INTENSITY=26
DGB_ADDRESS="DKhCswL8Ff5UyZWdVEbyUVvDhLYMmfVLP7"
DGB_POOL="stratum+tcp://skein.mine.zpool.ca:4933"

LBC_WORKER="nv$IP_AS_WORKER"
LBC_ADDRESS="fullzero22"
LBC_POOL="stratum+tcp://lbry.suprnova.cc:6256"

FTC_WORKER="nv$IP_AS_WORKER"
FTC_ADDRESS="fullzero22"
FTC_POOL="stratum+tcp://coinotron.com:3337"


USE_ENVIRONMENTAL_VARIBLES="NO"   #YES  NO

ETHERMINEdotORG="NO"

CLAYMORE_VERSION="9_7"    # choose 9_7  or  9_5  or  9_4  or  8_0

GENOILorCLAYMORE="GENOIL"  # choose GENOIL  or  CLAYMORE


ETH_WORKER="nv$IP_AS_WORKER"
ETH_ADDRESS="0x7d9C5BE80dbD885E055Ccb6168068a4c38d8072F"
ETH_POOL="eth-us-east1.nanopool.org:9999"
ETH_EXTENTION_ARGUMENTS=""    # add any additional claymore arguments desired here

ETC_WORKER="nv$IP_AS_WORKER"
ETC_ADDRESS="0xc3eab16bd575e5498efef2b038c8c178598d659e"
ETC_POOL="etc-us-east1.nanopool.org:19999"
ETC_EXTENTION_ARGUMENTS=""    # add any additional claymore arguments desired here

EXP_WORKER="nv$IP_AS_WORKER"
EXP_ADDRESS="0xa7108c64e6fec3193091f2cae2a5c62a36d4396a"
EXP_POOL="exp-us.dwarfpool.com:8018"
EXP_EXTENTION_ARGUMENTS=""    # add any additional claymore arguments desired here

MUSIC_WORKER="nv$IP_AS_WORKER"
MUSIC_ADDRESS="0x48919b296f648bd2edfeb6f336d2b3f66a741ea5"
MUSIC_POOL="stratum+tcp://213.154.202.174:3334"
MUSIC_EXTENTION_ARGUMENTS=""    # add any additional claymore arguments desired here

SC_WORKER="nv$IP_AS_WORKER"
SC_ADDRESS="1569a3353bb3353aedc6e0b79e796787ffcbe45d6caaa28f678ba74a5c50fdb02e735244e706"
SC_POOL="sia-us-east1.nanopool.org:7777"
SC_GW_POOL="sia-us-east1.nanopool.org:9980"

DCR_WORKER="nv$IP_AS_WORKER"
DCR_ADDRESS="fullzero22"
DCR_POOL="stratum+tcp://dcr.suprnova.cc:3252"

PASC_WORKER="nv$IP_AS_WORKER"
PASC_ADDRESS="86646-64.b12a9833f216b5a8"
PASC_POOL="pasc-us-east1.nanopool.org:15555"

# if plusCPU is "YES" replace with your XMR info
XMR_WORKER="nv$IP_AS_WORKER"
XMR_ADDRESS="47sghzufGhJJDQEbScMCwVBimTuq6L5JiRixD8VeGbpjCTA12noXmi4ZyBZLc99e66NtnKff34fHsGRoyZk3ES1s1V4QVcB.23d5f83d0021a50d8f809f4727c8622d3ea25798942bcb1ba0eee40cc157f65c"
XMR_POOL="stratum+tcp://xmr-us-east1.nanopool.org:14444"

#  settings above: ALL ADJUSTABLE SETINGS ABOVE THIS LINE
#########################################################################
#########################################################################
#########################################################################
#########################################################################
#########################################################################
#########################################################################
#########################################################################
#########################################################################
#########################################################################
#########################################################################
#########################################################################
#########################################################################
#  implementation below: NO SETTINGS BELOW

if [ $SALFTER_NICEHASH_PROFIT_SWITCHING == "NO" ]
then
pkill -e miner
fi

XORG="FAIL"

if grep -q "28800" /etc/X11/xorg.conf;
then
XORG="OK"
fi

sudo ldconfig /usr/local/cuda/lib64
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi

if [ $XORG == "FAIL" ]
then
sudo cp '/etc/X11/xorg.conf.backup' '/etc/X11/xorg.conf'
echo ''
echo "Xorg PROBLEM DETECTED"
echo ''
echo "Restoring Xorg"
echo ''
echo "Rebooting in 5"
sleep 5
sudo reboot
fi

IP=$(ifconfig | sed -En 's/127.0.0.1//;s/.*inet (addr:)?(([0-9]*\.){3}[0-9]*).*/\2/p')

echo ""
echo ''
echo rig IP: $IP

if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi

echo ""
echo ''
lspci | grep VGA

if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi

echo ""
echo ''
nvidia-smi
echo ""

if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi

if [ $USE_ENVIRONMENTAL_VARIBLES == "YES" ]
then
export GPU_FORCE_64BIT_PTR="0"
export GPU_MAX_HEAP_SIZE="100"
export GPU_USE_SYNC_OBJECTS="1"
export GPU_MAX_ALLOC_PERCENT="100"
echo ""
echo ENVIRONMENTAL VARIBLES SET
fi

if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi

if [ $POWERLIMIT == "YES" ]
then
sudo nvidia-smi -pl $POWERLIMIT_WATTS
fi

if [[ $INDIVIDUAL_POWERLIMIT == "YES" && $Maxximus007_AUTO_TEMPERATURE_CONTROL == "NO" ]]
then
sudo nvidia-smi -i 0 -pl $INDIVIDUAL_POWERLIMIT_0
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 1 -pl $INDIVIDUAL_POWERLIMIT_1
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 2 -pl $INDIVIDUAL_POWERLIMIT_2
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 3 -pl $INDIVIDUAL_POWERLIMIT_3
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 4 -pl $INDIVIDUAL_POWERLIMIT_4
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 5 -pl $INDIVIDUAL_POWERLIMIT_5
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 6 -pl $INDIVIDUAL_POWERLIMIT_6
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 7 -pl $INDIVIDUAL_POWERLIMIT_7
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 8 -pl $INDIVIDUAL_POWERLIMIT_8
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 9 -pl $INDIVIDUAL_POWERLIMIT_9
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 10 -pl $INDIVIDUAL_POWERLIMIT_10
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 11 -pl $INDIVIDUAL_POWERLIMIT_11
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 12 -pl $INDIVIDUAL_POWERLIMIT_12
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
sudo nvidia-smi -i 13 -pl $INDIVIDUAL_POWERLIMIT_13
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
fi

if [ $TEAMVIEWER == "YES" ]
then
sudo teamviewer --daemon enable
sleep 2
running=$(ps -ef | awk '$NF~"teamviewer" {print $2}')
if [ "$running" == "" ]
then
guake -n teamviewer -r teamviewer -e "teamviewer"
running=""
fi
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
fi

if [ $TEAMVIEWER == "NO" ]
then
sudo teamviewer --daemon disable
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
fi

if [ $SSH == "YES" ]
then
sudo cp '/etc/init/ssh.conf-on' '/etc/init/ssh.conf'
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
fi

if [ $SSH == "NO" ]
then
sudo cp '/etc/init/ssh.conf-off' '/etc/init/ssh.conf'
if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi
fi

if [ $SRR == "YES" ]
then
sudo rm /home/m1/srr_serial
sudo rm /home/m1/srr_slot
sleep 2
HCD='SRR'
sudo -- sh -c -e "echo '$SRR_SERIAL' > /home/m1/srr_serial";
sudo -- sh -c -e "echo '$__SRR_SLOT' > /home/m1/srr_slot";
running=$(ps -ef | awk '$NF~"SRR" {print $2}')
if [ "$running" == "" ]
then
guake -n $HCD -r SRR -e "bash /home/m1/SRR"
running=""
fi
fi

if [ $plusCPU == "YES" ]
then
HCD='/home/m1/cpuOPT/cpuminer'
XMRADDR="$XMR_ADDRESS.$XMR_WORKER"
running=$(ps -ef | awk '$NF~"miner" {print $2}')
if [ "$running" == "" ]
then
guake -n $HCD -r plusCPU -e "$HCD -a cryptonight -o $XMR_POOL -u $XMRADDR -p x -t $threadCOUNT"
running=""
fi
fi

if [ $AUTO_REBOOT == "YES" ]
then
HCD='/home/m1/reboot'
sudo -- sh -c -e "echo '$REBOOT_TIMEOUT_IN_MINUTES' > /home/m1/reboot_timeout";
running=$(ps -ef | awk '$NF~"reboot" {print $2}')
if [ "$running" == "" ]
then
guake -n $HCD -r AUTO_REBOOT -e "bash /home/m1/reboot"
running=""
fi
fi


if [ $IAmNotAJeep_and_Maxximus007_WATCHDOG == "YES" ]
then
echo ""
echo "LAUNCHING:  IAmNotAJeep_and_Maxximus007_WATCHDOG "
HCD='/home/m1/IAmNotAJeep_and_Maxximus007_WATCHDOG'
running=$(ps -ef | awk '$NF~"IAmNotAJeep_and_Maxximus007_WATCHDOG" {print $2}')
if [ "$running" == "" ]
then
guake -n $HCD -r IJ_M7_WATCHDOG -e "bash /home/m1/IAmNotAJeep_and_Maxximus007_WATCHDOG"
running=""
fi
  echo ""
  echo "process in Guake Tab"
fi

if [ $Maxximus007_AUTO_TEMPERATURE_CONTROL == "YES" ]
then

cd /home/m1

rm /home/m1/p0
rm /home/m1/p1
rm /home/m1/p2
rm /home/m1/p3
rm /home/m1/p4
rm /home/m1/p5
rm /home/m1/p6
rm /home/m1/p7
rm /home/m1/p8
rm /home/m1/p9
rm /home/m1/p10
rm /home/m1/p11
rm /home/m1/p12
rm /home/m1/p13
rm /home/m1/t0
rm /home/m1/t1
rm /home/m1/t2
rm /home/m1/t3
rm /home/m1/t4
rm /home/m1/t5
rm /home/m1/t6
rm /home/m1/t7
rm /home/m1/t8
rm /home/m1/t9
rm /home/m1/t10
rm /home/m1/t11
rm /home/m1/t12
rm /home/m1/t13
rm /home/m1/fa
rm /home/m1/pa
rm /home/m1/td
rm /home/m1/rpl

sleep 2

echo $INDIVIDUAL_POWERLIMIT_0 > '/home/m1/p0'
echo $INDIVIDUAL_POWERLIMIT_1 > '/home/m1/p1'
echo $INDIVIDUAL_POWERLIMIT_2 > '/home/m1/p2'
echo $INDIVIDUAL_POWERLIMIT_3 > '/home/m1/p3'
echo $INDIVIDUAL_POWERLIMIT_4 > '/home/m1/p4'
echo $INDIVIDUAL_POWERLIMIT_5 > '/home/m1/p5'
echo $INDIVIDUAL_POWERLIMIT_6 > '/home/m1/p6'
echo $INDIVIDUAL_POWERLIMIT_7 > '/home/m1/p7'
echo $INDIVIDUAL_POWERLIMIT_8 > '/home/m1/p8'
echo $INDIVIDUAL_POWERLIMIT_9 > '/home/m1/p9'
echo $INDIVIDUAL_POWERLIMIT_10 > '/home/m1/p10'
echo $INDIVIDUAL_POWERLIMIT_11 > '/home/m1/p11'
echo $INDIVIDUAL_POWERLIMIT_12 > '/home/m1/p12'
echo $INDIVIDUAL_POWERLIMIT_13 > '/home/m1/p13'

echo $TARGET_TEMP_0 > '/home/m1/t0'
echo $TARGET_TEMP_1 > '/home/m1/t1'
echo $TARGET_TEMP_2 > '/home/m1/t2'
echo $TARGET_TEMP_3 > '/home/m1/t3'
echo $TARGET_TEMP_4 > '/home/m1/t4'
echo $TARGET_TEMP_5 > '/home/m1/t5'
echo $TARGET_TEMP_6 > '/home/m1/t6'
echo $TARGET_TEMP_7 > '/home/m1/t7'
echo $TARGET_TEMP_8 > '/home/m1/t8'
echo $TARGET_TEMP_9 > '/home/m1/t9'
echo $TARGET_TEMP_10 > '/home/m1/t10'
echo $TARGET_TEMP_11 > '/home/m1/t11'
echo $TARGET_TEMP_12 > '/home/m1/t12'
echo $TARGET_TEMP_13 > '/home/m1/t13'

echo $__FAN_ADJUST > '/home/m1/fa'
echo $POWER_ADJUST > '/home/m1/pa'
echo $ALLOWED_TEMP_DIFF > '/home/m1/td'
echo $RESTORE_POWER_LIMIT > '/home/m1/rpl'
echo ""
echo "LAUNCHING:  Maxximus007_AUTO_TEMPERATURE_CONTROL "

HCD='/home/m1/Maxximus007_AUTO_TEMPERATURE_CONTROL'
running=$(ps -ef | awk '$NF~"Maxximus007_AUTO_TEMPERATURE_CONTROL" {print $2}')
if [ "$running" == "" ]
then
guake -n $HCD -r Maxximus007_AUTO_TEMPERATURE_CONTROL -e "bash /home/m1/Maxximus007_AUTO_TEMPERATURE_CONTROL"
running=""
fi
  echo ""
  echo "process in Guake Tab"
  echo ""
fi

___1050_or_1050ti="NO"

NORMAL="NO"

nvidia-smi -L > /tmp/tempa

if grep -q "1050" /tmp/tempa;
then
___1050_or_1050ti="YES"
fi

if grep -q "1060" /tmp/tempa;
then
NORMAL="YES"
fi

if grep -q "1070" /tmp/tempa;
then
NORMAL="YES"
fi

if grep -q "1080" /tmp/tempa;
then
NORMAL="YES"
fi

if grep -q "1080ti" /tmp/tempa;
then
NORMAL="YES"
fi

rm /tmp/tempa

if [ "$FAN_SPEED" -lt "40" ]
then
    FAN_SPEED=40
fi

GPUS=$(nvidia-smi --query-gpu=count --format=csv,noheader,nounits | tail -1)

NVD=nvidia-settings

if [ $SALFTER_NICEHASH_PROFIT_SWITCHING == "YES" ]
then

HOSTEDIT="YES"

if grep -q "api.nicehash.com" /etc/hosts;
then
HOSTEDIT="NO"
fi

if [ $HOSTEDIT == "YES" ]
then
sudo -- sh -c -e "echo '' >> /etc/hosts";
sudo -- sh -c -e "echo '104.20.158.21 api.nicehash.com' >> /etc/hosts";
echo UPDATED HOSTS FILE WITH IPv6 FIX
echo ""
echo ""
fi

rm /home/m1/currency
rm /home/m1/pwrcost
rm /home/m1/minprofit
rm /home/m1/paymentaddr
rm /home/m1/minername
rm /home/m1/f
rm /home/m1/g
rm /home/m1/h
#rm /home/m1/ii
rm /home/m1/j
rm /home/m1/k
rm /home/m1/l
#rm /home/m1/m
rm /home/m1/n
rm /home/m1/o
rm /home/m1/p
#rm /home/m1/q
rm /home/m1/r
rm /home/m1/s
rm /home/m1/t
#rm /home/m1/u
rm /home/m1/v
rm /home/m1/ww
rm /home/m1/x
#rm /home/m1/y
#rm /home/m1/z
#rm /home/m1/za
#rm /home/m1/zb
#rm /home/m1/zc
sleep 2

cd /home/m1

echo $CURRENCY > '/home/m1/currency'
echo $POWER_COST > '/home/m1/pwrcost'
echo $MINIMUM_PROFIT > '/home/m1/minprofit'
echo $PAYMENT_ADDRESS > '/home/m1/paymentaddr'
echo $WORKER_NAME > '/home/m1/minername'

echo $daggerhashimoto_POWERLIMIT_WATTS > '/home/m1/f'
echo $__daggerhashimoto_CORE_OVERCLOCK > '/home/m1/g'
echo $daggerhashimoto_MEMORY_OVERCLOCK > '/home/m1/h'
#echo $_______daggerhashimoto_FAN_SPEED > '/home/m1/ii'

echo $equihash_POWERLIMIT_WATTS > '/home/m1/j'
echo $__equihash_CORE_OVERCLOCK > '/home/m1/k'
echo $equihash_MEMORY_OVERCLOCK > '/home/m1/l'
#echo $_______equihash_FAN_SPEED > '/home/m1/m'

echo $neoscrypt_POWERLIMIT_WATTS > '/home/m1/n'
echo $__neoscrypt_CORE_OVERCLOCK > '/home/m1/o'
echo $neoscrypt_MEMORY_OVERCLOCK > '/home/m1/p'
#echo $_______neoscrypt_FAN_SPEED > '/home/m1/q'

echo $lyra2rev2_POWERLIMIT_WATTS > '/home/m1/r'
echo $__lyra2rev2_CORE_OVERCLOCK > '/home/m1/s'
echo $lyra2rev2_MEMORY_OVERCLOCK > '/home/m1/t'
#echo $_______lyra2rev2_FAN_SPEED > '/home/m1/u'

echo $lbry_POWERLIMIT_WATTS > '/home/m1/v'
echo $__lbry_CORE_OVERCLOCK > '/home/m1/ww'
echo $lbry_MEMORY_OVERCLOCK > '/home/m1/x'
#echo $_______lbry_FAN_SPEED > '/home/m1/y'

#echo $pascal_POWERLIMIT_WATTS > '/home/m1/z'
#echo $__pascal_CORE_OVERCLOCK > '/home/m1/za'
#echo $pascal_MEMORY_OVERCLOCK > '/home/m1/zb'
#echo $_______pascal_FAN_SPEED > '/home/m1/zc'

echo "LAUNCHING:  SALFTER_NICEHASH_PROFIT_SWITCHING "
echo ""

python2.7 '/home/m1/switch'

if [ $LOCALorREMOTE == "LOCAL" ]
then
guake -n 1 -r SALFTER_NICEHASH_PROFIT_SWITCHING -e "screen -r miner"
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
  echo ""
  cat current-profit
  echo ""

  if [ $LOCALorREMOTE == "LOCAL" ]
  then
  guake -r SALFTER_NICEHASH_PROFIT_SWITCHING -e "screen -r miner"
  echo ""
  echo "mining process in Guake Tab"
  echo ""
  sleep $PROFIT_CHECK_TIMEOUT
  python2.7 '/home/m1/switch'
  fi

  if [ $LOCALorREMOTE == "REMOTE" ]
  then
  echo "ENTER:"
  echo "" 
  echo "screen -r miner"
  echo ""
  echo "in a terminal to view mining process"
  sleep $PROFIT_CHECK_TIMEOUT
  python2.7 '/home/m1/switch'
  fi
done
fi

if [ $SALFTER_NICEHASH_PROFIT_SWITCHING == "NO" ]
then

if [ $INDIVIDUAL_CLOCKS == "NO" ]
then
__CORE_OVERCLOCK_0=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_0=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_1=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_1=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_2=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_2=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_3=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_3=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_4=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_4=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_5=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_5=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_6=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_6=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_7=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_7=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_8=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_8=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_9=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_9=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_10=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_10=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_11=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_11=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_12=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_12=$MEMORY_OVERCLOCK
__CORE_OVERCLOCK_13=$__CORE_OVERCLOCK
MEMORY_OVERCLOCK_13=$MEMORY_OVERCLOCK
fi

TI="3"

if [ $___1050_or_1050ti == "YES" ]
then
    TI="2"
if [ $NORMAL == "YES" ]
then
    TI="2 3"
fi
fi

if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi

for j in $TI
  do
    ${NVD} -a [gpu:0]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_0}
    ${NVD} -a [gpu:0]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_0}

if [ $GPUS == 2 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
fi

if [ $GPUS == 3 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
    ${NVD} -a [gpu:2]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_2}
    ${NVD} -a [gpu:2]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_2}
fi

if [ $GPUS == 4 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
    ${NVD} -a [gpu:2]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_2}
    ${NVD} -a [gpu:2]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_2}
    ${NVD} -a [gpu:3]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_3}
    ${NVD} -a [gpu:3]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_3}
fi

if [ $GPUS == 5 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
    ${NVD} -a [gpu:2]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_2}
    ${NVD} -a [gpu:2]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_2}
    ${NVD} -a [gpu:3]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_3}
    ${NVD} -a [gpu:3]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_3}
    ${NVD} -a [gpu:4]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_4}
    ${NVD} -a [gpu:4]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_4}
fi

if [ $GPUS == 6 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
    ${NVD} -a [gpu:2]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_2}
    ${NVD} -a [gpu:2]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_2}
    ${NVD} -a [gpu:3]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_3}
    ${NVD} -a [gpu:3]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_3}
    ${NVD} -a [gpu:4]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_4}
    ${NVD} -a [gpu:4]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_4}
    ${NVD} -a [gpu:5]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_5}
    ${NVD} -a [gpu:5]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_5}
fi

if [ $GPUS == 7 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
    ${NVD} -a [gpu:2]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_2}
    ${NVD} -a [gpu:2]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_2}
    ${NVD} -a [gpu:3]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_3}
    ${NVD} -a [gpu:3]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_3}
    ${NVD} -a [gpu:4]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_4}
    ${NVD} -a [gpu:4]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_4}
    ${NVD} -a [gpu:5]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_5}
    ${NVD} -a [gpu:5]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_5}
    ${NVD} -a [gpu:6]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_6}
    ${NVD} -a [gpu:6]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_6}
fi

if [ $GPUS == 8 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
    ${NVD} -a [gpu:2]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_2}
    ${NVD} -a [gpu:2]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_2}
    ${NVD} -a [gpu:3]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_3}
    ${NVD} -a [gpu:3]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_3}
    ${NVD} -a [gpu:4]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_4}
    ${NVD} -a [gpu:4]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_4}
    ${NVD} -a [gpu:5]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_5}
    ${NVD} -a [gpu:5]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_5}
    ${NVD} -a [gpu:6]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_6}
    ${NVD} -a [gpu:6]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_6}
    ${NVD} -a [gpu:7]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_7}
    ${NVD} -a [gpu:7]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_7}
fi

if [ $GPUS == 9 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
    ${NVD} -a [gpu:2]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_2}
    ${NVD} -a [gpu:2]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_2}
    ${NVD} -a [gpu:3]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_3}
    ${NVD} -a [gpu:3]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_3}
    ${NVD} -a [gpu:4]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_4}
    ${NVD} -a [gpu:4]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_4}
    ${NVD} -a [gpu:5]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_5}
    ${NVD} -a [gpu:5]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_5}
    ${NVD} -a [gpu:6]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_6}
    ${NVD} -a [gpu:6]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_6}
    ${NVD} -a [gpu:7]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_7}
    ${NVD} -a [gpu:7]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_7}
    ${NVD} -a [gpu:8]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_8}
    ${NVD} -a [gpu:8]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_8}
fi

if [ $GPUS == 10 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
    ${NVD} -a [gpu:2]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_2}
    ${NVD} -a [gpu:2]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_2}
    ${NVD} -a [gpu:3]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_3}
    ${NVD} -a [gpu:3]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_3}
    ${NVD} -a [gpu:4]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_4}
    ${NVD} -a [gpu:4]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_4}
    ${NVD} -a [gpu:5]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_5}
    ${NVD} -a [gpu:5]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_5}
    ${NVD} -a [gpu:6]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_6}
    ${NVD} -a [gpu:6]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_6}
    ${NVD} -a [gpu:7]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_7}
    ${NVD} -a [gpu:7]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_7}
    ${NVD} -a [gpu:8]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_8}
    ${NVD} -a [gpu:8]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_8}
    ${NVD} -a [gpu:9]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_9}
    ${NVD} -a [gpu:9]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_9}
fi

if [ $GPUS == 11 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
    ${NVD} -a [gpu:2]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_2}
    ${NVD} -a [gpu:2]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_2}
    ${NVD} -a [gpu:3]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_3}
    ${NVD} -a [gpu:3]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_3}
    ${NVD} -a [gpu:4]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_4}
    ${NVD} -a [gpu:4]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_4}
    ${NVD} -a [gpu:5]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_5}
    ${NVD} -a [gpu:5]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_5}
    ${NVD} -a [gpu:6]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_6}
    ${NVD} -a [gpu:6]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_6}
    ${NVD} -a [gpu:7]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_7}
    ${NVD} -a [gpu:7]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_7}
    ${NVD} -a [gpu:8]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_8}
    ${NVD} -a [gpu:8]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_8}
    ${NVD} -a [gpu:9]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_9}
    ${NVD} -a [gpu:9]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_9}
    ${NVD} -a [gpu:10]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_10}
    ${NVD} -a [gpu:10]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_10}
fi

if [ $GPUS == 12 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
    ${NVD} -a [gpu:2]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_2}
    ${NVD} -a [gpu:2]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_2}
    ${NVD} -a [gpu:3]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_3}
    ${NVD} -a [gpu:3]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_3}
    ${NVD} -a [gpu:4]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_4}
    ${NVD} -a [gpu:4]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_4}
    ${NVD} -a [gpu:5]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_5}
    ${NVD} -a [gpu:5]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_5}
    ${NVD} -a [gpu:6]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_6}
    ${NVD} -a [gpu:6]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_6}
    ${NVD} -a [gpu:7]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_7}
    ${NVD} -a [gpu:7]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_7}
    ${NVD} -a [gpu:8]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_8}
    ${NVD} -a [gpu:8]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_8}
    ${NVD} -a [gpu:9]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_9}
    ${NVD} -a [gpu:9]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_9}
    ${NVD} -a [gpu:10]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_10}
    ${NVD} -a [gpu:10]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_10}
    ${NVD} -a [gpu:11]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_11}
    ${NVD} -a [gpu:11]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_11}
fi

if [ $GPUS == 13 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
    ${NVD} -a [gpu:2]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_2}
    ${NVD} -a [gpu:2]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_2}
    ${NVD} -a [gpu:3]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_3}
    ${NVD} -a [gpu:3]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_3}
    ${NVD} -a [gpu:4]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_4}
    ${NVD} -a [gpu:4]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_4}
    ${NVD} -a [gpu:5]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_5}
    ${NVD} -a [gpu:5]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_5}
    ${NVD} -a [gpu:6]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_6}
    ${NVD} -a [gpu:6]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_6}
    ${NVD} -a [gpu:7]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_7}
    ${NVD} -a [gpu:7]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_7}
    ${NVD} -a [gpu:8]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_8}
    ${NVD} -a [gpu:8]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_8}
    ${NVD} -a [gpu:9]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_9}
    ${NVD} -a [gpu:9]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_9}
    ${NVD} -a [gpu:10]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_10}
    ${NVD} -a [gpu:10]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_10}
    ${NVD} -a [gpu:11]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_11}
    ${NVD} -a [gpu:11]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_11}
    ${NVD} -a [gpu:12]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_12}
    ${NVD} -a [gpu:12]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_12}
fi

if [ $GPUS == 14 ]
then
    ${NVD} -a [gpu:1]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_1}
    ${NVD} -a [gpu:1]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_1}
    ${NVD} -a [gpu:2]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_2}
    ${NVD} -a [gpu:2]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_2}
    ${NVD} -a [gpu:3]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_3}
    ${NVD} -a [gpu:3]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_3}
    ${NVD} -a [gpu:4]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_4}
    ${NVD} -a [gpu:4]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_4}
    ${NVD} -a [gpu:5]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_5}
    ${NVD} -a [gpu:5]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_5}
    ${NVD} -a [gpu:6]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_6}
    ${NVD} -a [gpu:6]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_6}
    ${NVD} -a [gpu:7]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_7}
    ${NVD} -a [gpu:7]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_7}
    ${NVD} -a [gpu:8]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_8}
    ${NVD} -a [gpu:8]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_8}
    ${NVD} -a [gpu:9]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_9}
    ${NVD} -a [gpu:9]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_9}
    ${NVD} -a [gpu:10]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_10}
    ${NVD} -a [gpu:10]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_10}
    ${NVD} -a [gpu:11]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_11}
    ${NVD} -a [gpu:11]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_11}
    ${NVD} -a [gpu:12]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_12}
    ${NVD} -a [gpu:12]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_12}
    ${NVD} -a [gpu:13]/GPUGraphicsClockOffset[${j}]=${__CORE_OVERCLOCK_13}
    ${NVD} -a [gpu:13]/GPUMemoryTransferRateOffset[${j}]=${MEMORY_OVERCLOCK_13}
fi
done

if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi

if [[ $MANUAL_FAN == "YES" && $Maxximus007_AUTO_TEMPERATURE_CONTROL == "NO" ]]
then
    ${NVD} -a [gpu:0]/GPUFanControlState=1
    ${NVD} -a [fan:0]/GPUTargetFanSpeed=${FAN_SPEED}

if [ $GPUS == 2 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
fi

if [ $GPUS == 3 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:2]/GPUFanControlState=1
    ${NVD} -a [fan:2]/GPUTargetFanSpeed=${FAN_SPEED}
fi

if [ $GPUS == 4 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:2]/GPUFanControlState=1
    ${NVD} -a [fan:2]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:3]/GPUFanControlState=1
    ${NVD} -a [fan:3]/GPUTargetFanSpeed=${FAN_SPEED}
fi

if [ $GPUS == 5 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:2]/GPUFanControlState=1
    ${NVD} -a [fan:2]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:3]/GPUFanControlState=1
    ${NVD} -a [fan:3]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:4]/GPUFanControlState=1
    ${NVD} -a [fan:4]/GPUTargetFanSpeed=${FAN_SPEED}
fi

if [ $GPUS == 6 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:2]/GPUFanControlState=1
    ${NVD} -a [fan:2]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:3]/GPUFanControlState=1
    ${NVD} -a [fan:3]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:4]/GPUFanControlState=1
    ${NVD} -a [fan:4]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:5]/GPUFanControlState=1
    ${NVD} -a [fan:5]/GPUTargetFanSpeed=${FAN_SPEED}
fi

if [ $GPUS == 7 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:2]/GPUFanControlState=1
    ${NVD} -a [fan:2]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:3]/GPUFanControlState=1
    ${NVD} -a [fan:3]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:4]/GPUFanControlState=1
    ${NVD} -a [fan:4]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:5]/GPUFanControlState=1
    ${NVD} -a [fan:5]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:6]/GPUFanControlState=1
    ${NVD} -a [fan:6]/GPUTargetFanSpeed=${FAN_SPEED}
fi

if [ $GPUS == 8 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:2]/GPUFanControlState=1
    ${NVD} -a [fan:2]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:3]/GPUFanControlState=1
    ${NVD} -a [fan:3]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:4]/GPUFanControlState=1
    ${NVD} -a [fan:4]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:5]/GPUFanControlState=1
    ${NVD} -a [fan:5]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:6]/GPUFanControlState=1
    ${NVD} -a [fan:6]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:7]/GPUFanControlState=1
    ${NVD} -a [fan:7]/GPUTargetFanSpeed=${FAN_SPEED}
fi

if [ $GPUS == 9 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:2]/GPUFanControlState=1
    ${NVD} -a [fan:2]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:3]/GPUFanControlState=1
    ${NVD} -a [fan:3]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:4]/GPUFanControlState=1
    ${NVD} -a [fan:4]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:5]/GPUFanControlState=1
    ${NVD} -a [fan:5]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:6]/GPUFanControlState=1
    ${NVD} -a [fan:6]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:7]/GPUFanControlState=1
    ${NVD} -a [fan:7]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:8]/GPUFanControlState=1
    ${NVD} -a [fan:8]/GPUTargetFanSpeed=${FAN_SPEED}
fi

if [ $GPUS == 10 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:2]/GPUFanControlState=1
    ${NVD} -a [fan:2]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:3]/GPUFanControlState=1
    ${NVD} -a [fan:3]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:4]/GPUFanControlState=1
    ${NVD} -a [fan:4]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:5]/GPUFanControlState=1
    ${NVD} -a [fan:5]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:6]/GPUFanControlState=1
    ${NVD} -a [fan:6]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:7]/GPUFanControlState=1
    ${NVD} -a [fan:7]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:8]/GPUFanControlState=1
    ${NVD} -a [fan:8]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:9]/GPUFanControlState=1
    ${NVD} -a [fan:9]/GPUTargetFanSpeed=${FAN_SPEED}
fi

if [ $GPUS == 11 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:2]/GPUFanControlState=1
    ${NVD} -a [fan:2]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:3]/GPUFanControlState=1
    ${NVD} -a [fan:3]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:4]/GPUFanControlState=1
    ${NVD} -a [fan:4]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:5]/GPUFanControlState=1
    ${NVD} -a [fan:5]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:6]/GPUFanControlState=1
    ${NVD} -a [fan:6]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:7]/GPUFanControlState=1
    ${NVD} -a [fan:7]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:8]/GPUFanControlState=1
    ${NVD} -a [fan:8]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:9]/GPUFanControlState=1
    ${NVD} -a [fan:9]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:10]/GPUFanControlState=1
    ${NVD} -a [fan:10]/GPUTargetFanSpeed=${FAN_SPEED}
fi

if [ $GPUS == 12 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:2]/GPUFanControlState=1
    ${NVD} -a [fan:2]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:3]/GPUFanControlState=1
    ${NVD} -a [fan:3]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:4]/GPUFanControlState=1
    ${NVD} -a [fan:4]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:5]/GPUFanControlState=1
    ${NVD} -a [fan:5]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:6]/GPUFanControlState=1
    ${NVD} -a [fan:6]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:7]/GPUFanControlState=1
    ${NVD} -a [fan:7]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:8]/GPUFanControlState=1
    ${NVD} -a [fan:8]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:9]/GPUFanControlState=1
    ${NVD} -a [fan:9]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:10]/GPUFanControlState=1
    ${NVD} -a [fan:10]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:11]/GPUFanControlState=1
    ${NVD} -a [fan:11]/GPUTargetFanSpeed=${FAN_SPEED}
fi

if [ $GPUS == 13 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:2]/GPUFanControlState=1
    ${NVD} -a [fan:2]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:3]/GPUFanControlState=1
    ${NVD} -a [fan:3]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:4]/GPUFanControlState=1
    ${NVD} -a [fan:4]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:5]/GPUFanControlState=1
    ${NVD} -a [fan:5]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:6]/GPUFanControlState=1
    ${NVD} -a [fan:6]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:7]/GPUFanControlState=1
    ${NVD} -a [fan:7]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:8]/GPUFanControlState=1
    ${NVD} -a [fan:8]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:9]/GPUFanControlState=1
    ${NVD} -a [fan:9]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:10]/GPUFanControlState=1
    ${NVD} -a [fan:10]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:11]/GPUFanControlState=1
    ${NVD} -a [fan:11]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:12]/GPUFanControlState=1
    ${NVD} -a [fan:12]/GPUTargetFanSpeed=${FAN_SPEED}
fi

if [ $GPUS == 14 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=1
    ${NVD} -a [fan:1]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:2]/GPUFanControlState=1
    ${NVD} -a [fan:2]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:3]/GPUFanControlState=1
    ${NVD} -a [fan:3]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:4]/GPUFanControlState=1
    ${NVD} -a [fan:4]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:5]/GPUFanControlState=1
    ${NVD} -a [fan:5]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:6]/GPUFanControlState=1
    ${NVD} -a [fan:6]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:7]/GPUFanControlState=1
    ${NVD} -a [fan:7]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:8]/GPUFanControlState=1
    ${NVD} -a [fan:8]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:9]/GPUFanControlState=1
    ${NVD} -a [fan:9]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:10]/GPUFanControlState=1
    ${NVD} -a [fan:10]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:11]/GPUFanControlState=1
    ${NVD} -a [fan:11]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:12]/GPUFanControlState=1
    ${NVD} -a [fan:12]/GPUTargetFanSpeed=${FAN_SPEED}
    ${NVD} -a [gpu:13]/GPUFanControlState=1
    ${NVD} -a [fan:13]/GPUTargetFanSpeed=${FAN_SPEED}
fi
fi

if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi

if [[ $MANUAL_FAN == "NO" && $Maxximus007_AUTO_TEMPERATURE_CONTROL == "NO" ]]
then
    ${NVD} -a [gpu:0]/GPUFanControlState=0

if [ $GPUS == 2 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
fi

if [ $GPUS == 3 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
    ${NVD} -a [gpu:2]/GPUFanControlState=0
fi

if [ $GPUS == 4 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
    ${NVD} -a [gpu:2]/GPUFanControlState=0
    ${NVD} -a [gpu:3]/GPUFanControlState=0
fi

if [ $GPUS == 5 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
    ${NVD} -a [gpu:2]/GPUFanControlState=0
    ${NVD} -a [gpu:3]/GPUFanControlState=0
    ${NVD} -a [gpu:4]/GPUFanControlState=0
fi

if [ $GPUS == 6 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
    ${NVD} -a [gpu:2]/GPUFanControlState=0
    ${NVD} -a [gpu:3]/GPUFanControlState=0
    ${NVD} -a [gpu:4]/GPUFanControlState=0
    ${NVD} -a [gpu:5]/GPUFanControlState=0
fi

if [ $GPUS == 7 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
    ${NVD} -a [gpu:2]/GPUFanControlState=0
    ${NVD} -a [gpu:3]/GPUFanControlState=0
    ${NVD} -a [gpu:4]/GPUFanControlState=0
    ${NVD} -a [gpu:5]/GPUFanControlState=0
    ${NVD} -a [gpu:6]/GPUFanControlState=0
fi

if [ $GPUS == 8 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
    ${NVD} -a [gpu:2]/GPUFanControlState=0
    ${NVD} -a [gpu:3]/GPUFanControlState=0
    ${NVD} -a [gpu:4]/GPUFanControlState=0
    ${NVD} -a [gpu:5]/GPUFanControlState=0
    ${NVD} -a [gpu:6]/GPUFanControlState=0
    ${NVD} -a [gpu:7]/GPUFanControlState=0
fi

if [ $GPUS == 9 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
    ${NVD} -a [gpu:2]/GPUFanControlState=0
    ${NVD} -a [gpu:3]/GPUFanControlState=0
    ${NVD} -a [gpu:4]/GPUFanControlState=0
    ${NVD} -a [gpu:5]/GPUFanControlState=0
    ${NVD} -a [gpu:6]/GPUFanControlState=0
    ${NVD} -a [gpu:7]/GPUFanControlState=0
    ${NVD} -a [gpu:8]/GPUFanControlState=0
fi

if [ $GPUS == 10 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
    ${NVD} -a [gpu:2]/GPUFanControlState=0
    ${NVD} -a [gpu:3]/GPUFanControlState=0
    ${NVD} -a [gpu:4]/GPUFanControlState=0
    ${NVD} -a [gpu:5]/GPUFanControlState=0
    ${NVD} -a [gpu:6]/GPUFanControlState=0
    ${NVD} -a [gpu:7]/GPUFanControlState=0
    ${NVD} -a [gpu:8]/GPUFanControlState=0
    ${NVD} -a [gpu:9]/GPUFanControlState=0
fi

if [ $GPUS == 11 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
    ${NVD} -a [gpu:2]/GPUFanControlState=0
    ${NVD} -a [gpu:3]/GPUFanControlState=0
    ${NVD} -a [gpu:4]/GPUFanControlState=0
    ${NVD} -a [gpu:5]/GPUFanControlState=0
    ${NVD} -a [gpu:6]/GPUFanControlState=0
    ${NVD} -a [gpu:7]/GPUFanControlState=0
    ${NVD} -a [gpu:8]/GPUFanControlState=0
    ${NVD} -a [gpu:9]/GPUFanControlState=0
    ${NVD} -a [gpu:10]/GPUFanControlState=0
fi

if [ $GPUS == 12 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
    ${NVD} -a [gpu:2]/GPUFanControlState=0
    ${NVD} -a [gpu:3]/GPUFanControlState=0
    ${NVD} -a [gpu:4]/GPUFanControlState=0
    ${NVD} -a [gpu:5]/GPUFanControlState=0
    ${NVD} -a [gpu:6]/GPUFanControlState=0
    ${NVD} -a [gpu:7]/GPUFanControlState=0
    ${NVD} -a [gpu:8]/GPUFanControlState=0
    ${NVD} -a [gpu:9]/GPUFanControlState=0
    ${NVD} -a [gpu:10]/GPUFanControlState=0
    ${NVD} -a [gpu:11]/GPUFanControlState=0
fi
if [ $GPUS == 13 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
    ${NVD} -a [gpu:2]/GPUFanControlState=0
    ${NVD} -a [gpu:3]/GPUFanControlState=0
    ${NVD} -a [gpu:4]/GPUFanControlState=0
    ${NVD} -a [gpu:5]/GPUFanControlState=0
    ${NVD} -a [gpu:6]/GPUFanControlState=0
    ${NVD} -a [gpu:7]/GPUFanControlState=0
    ${NVD} -a [gpu:8]/GPUFanControlState=0
    ${NVD} -a [gpu:9]/GPUFanControlState=0
    ${NVD} -a [gpu:10]/GPUFanControlState=0
    ${NVD} -a [gpu:11]/GPUFanControlState=0
    ${NVD} -a [gpu:12]/GPUFanControlState=0
fi
if [ $GPUS == 14 ]
then
    ${NVD} -a [gpu:1]/GPUFanControlState=0
    ${NVD} -a [gpu:2]/GPUFanControlState=0
    ${NVD} -a [gpu:3]/GPUFanControlState=0
    ${NVD} -a [gpu:4]/GPUFanControlState=0
    ${NVD} -a [gpu:5]/GPUFanControlState=0
    ${NVD} -a [gpu:6]/GPUFanControlState=0
    ${NVD} -a [gpu:7]/GPUFanControlState=0
    ${NVD} -a [gpu:8]/GPUFanControlState=0
    ${NVD} -a [gpu:9]/GPUFanControlState=0
    ${NVD} -a [gpu:10]/GPUFanControlState=0
    ${NVD} -a [gpu:11]/GPUFanControlState=0
    ${NVD} -a [gpu:12]/GPUFanControlState=0
    ${NVD} -a [gpu:13]/GPUFanControlState=0
fi
fi

if [ $GPUPowerMizerMode_Adjust == "YES" ]
then
  gpu=0
  while [ $gpu -lt $GPUS ]
    do
      sudo ${NVD} -a [gpu:$gpu]/GPUPowerMizerMode=${GPUPowerMizerMode}
      let gpu=gpu+1
    done
fi

if [ $SLOW_USB_KEY_MODE == "YES" ]
then
sleep 6
fi

if [ $COIN == "NICE_ETHASH" ]
then

if [ $GENOILorCLAYMORE == "GENOIL" ]
then
HCD='/home/m1/eth/Genoil-U/ethminer'

NICEADDR="$BTC_ADDRESS.$NICE_ETHASH_WORKER"

screen -dmS miner $HCD -SP 2 -S $GENOIL_NICE_ETHASH_POOL -O $NICEADDR:x -U

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $GENOILorCLAYMORE == "CLAYMORE" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

NICEADDR="$BTC_ADDRESS.$NICE_ETHASH_WORKER"

screen -dmS miner $HCD -epool $NICE_ETHASH_POOL -ewal $NICEADDR -epsw x -esm 3 -allpools 1 -estale 0 -dbg -1 $NICE_ETHASH_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi
fi

if [ $COIN == "ZEC" ]
then

if [ $EWBF_VERSION == "3_3" ]
then
HCD='/home/m1/zec/v3_3/miner'
fi

if [ $EWBF_VERSION == "3_4" ]
then
HCD='/home/m1/zec/v3_4/miner'
fi

ZECADDR="$ZEC_ADDRESS.$ZEC_WORKER"

screen -dmS miner $HCD --eexit 3 --fee $EWBF_PERCENT --pec --server $ZEC_POOL --user $ZECADDR --pass z --port $ZEC_PORT;

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "ZCL" ]
then

if [ $EWBF_VERSION == "3_3" ]
then
HCD='/home/m1/zec/v3_3/miner'
fi

if [ $EWBF_VERSION == "3_4" ]
then
HCD='/home/m1/zec/v3_4/miner'
fi

ZCLADDR="$ZCL_ADDRESS.$ZCL_WORKER"

screen -dmS miner $HCD --eexit 3 --fee $EWBF_PERCENT --pec --server $ZCL_POOL --user $ZCLADDR --pass z --port $ZCL_PORT;

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "ZEN" ]
then

if [ $EWBF_VERSION == "3_3" ]
then
HCD='/home/m1/zec/v3_3/miner'
fi

if [ $EWBF_VERSION == "3_4" ]
then
HCD='/home/m1/zec/v3_4/miner'
fi

ZENADDR="$ZEN_ADDRESS.$ZEN_WORKER"

screen -dmS miner $HCD --eexit 3 --fee $EWBF_PERCENT --pec --server $ZEN_POOL --user $ZENADDR --pass z --port $ZEN_PORT;

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "HUSH" ]
then

if [ $EWBF_VERSION == "3_3" ]
then
HCD='/home/m1/zec/v3_3/miner'
fi

if [ $EWBF_VERSION == "3_4" ]
then
HCD='/home/m1/zec/v3_4/miner'
fi

HUSHADDR="$HUSH_ADDRESS.$HUSH_WORKER"

screen -dmS miner $HCD --eexit 3 --fee $EWBF_PERCENT --pec --server $HUSH_POOL --user $HUSHADDR --pass z --port $HUSH_PORT;

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "ZCOIN" ]
then
HCD='/home/m1/TPccminer/ccminer'

ADDR="$ZCOIN_ADDRESS.$ZCOIN_WORKER"

screen -dmS miner $HCD -a lyra2 -o $ZCOIN_POOL -u $ADDR -p x

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "ZPOOL_LYRA2V2" ]
then
HCD='/home/m1/SPccminer/ccminer'

screen -dmS miner $HCD -a lyra2v2 -o $ZPOOL_LYRA2V2_POOL -u $BTC_ADDRESS -p c=BTC

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "ZPOOL_BLAKE2S" ]
then
HCD='/home/m1/SPccminer/ccminer'

screen -dmS miner $HCD -a blake2s -o $ZPOOL_BLAKE2S_POOL -u $BTC_ADDRESS -p c=BTC

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "MONA" ]
then
HCD='/home/m1/SPccminer/ccminer'
ADDR="$MONA_ADDRESS.$MONA_WORKER"

screen -dmS miner $HCD -a lyra2v2 -o $MONA_POOL -u $ADDR -p x

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DMD" ]
then
HCD='/home/m1/TPccminer/ccminer'
ADDR="$DMD_ADDRESS.$DMD_WORKER"

screen -dmS miner $HCD -a groestl -o $DMD_POOL -u $ADDR -p x

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "GRS" ]
then
HCD='/home/m1/TPccminer/ccminer'
ADDR="$GRS_ADDRESS.$GRS_WORKER"

screen -dmS miner $HCD -a groestl -o $GRS_POOL -u $ADDR -p x

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "VTC" ]
then
HCD='/home/m1/SPccminer/ccminer'
ADDR="$VTC_ADDRESS.$VTC_WORKER"

if [ $VTC_AUTOCONVERT_TO_BTC == "YES" ]
then
ADDR="$BTC_ADDRESS.$VTC_WORKER"

screen -dmS miner $HCD -a lyra2v2 -o $VTC_POOL -u $ADDR -p c=BTC

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $VTC_AUTOCONVERT_TO_BTC == "NO" ]
then

screen -dmS miner $HCD -a lyra2v2 -o $VTC_POOL -u $ADDR -p c=VTC

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi
fi

if [ $COIN == "DGB" ]
then
HCD='/home/m1/TPccminer/ccminer'
ADDR="$DGB_ADDRESS"

if [ $DGB_AUTOCONVERT_TO_BTC == "YES" ]
then
ADDR="$BTC_ADDRESS"

screen -dmS miner $HCD -a skein -o $DGB_POOL -u $ADDR -p c=BTC -i $DGB_INTENSITY

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $DGB_AUTOCONVERT_TO_BTC == "NO" ]
then

screen -dmS miner $HCD -a skein -o $DGB_POOL -u $ADDR -p c=DGB -i $DGB_INTENSITY

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi
fi

if [ $COIN == "LBC" ]
then
HCD='/home/m1/SPccminer/ccminer'
ADDR="$LBC_ADDRESS.$LBC_WORKER"

screen -dmS miner $HCD -a lbry -o $LBC_POOL -u $ADDR -p x

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "FTC" ]
then
HCD='/home/m1/SPccminer/ccminer'
ADDR="$FTC_ADDRESS.$FTC_WORKER"

screen -dmS miner $HCD -a neoscrypt -o $FTC_POOL -u $ADDR -p x

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "ETC" ]
then

if [ $GENOILorCLAYMORE == "GENOIL" ]
then
HCD='/home/m1/eth/Genoil-U/ethminer'

ETCADDR="$ETC_ADDRESS/$ETC_WORKER"

if [ $ETHERMINEdotORG == "YES" ]
then
ETCADDR="$ETC_ADDRESS.$ETC_WORKER"
fi

screen -dmS miner $HCD -S $ETC_POOL -O $ETCADDR:x -U

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $GENOILorCLAYMORE == "CLAYMORE" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

ETCADDR="$ETC_ADDRESS/$ETC_WORKER"

if [ $ETHERMINEdotORG == "YES" ]
then
ETCADDR="$ETC_ADDRESS.$ETC_WORKER"
fi

screen -dmS miner $HCD -epool $ETC_POOL -ewal $ETCADDR -epsw x -mode 1 -dbg -1 $ETC_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi
fi

if [ $COIN == "EXP" ]
then

if [ $GENOILorCLAYMORE == "GENOIL-CURRENTLY-NOT-SUPPORTED" ]
then
HCD='/home/m1/eth/Genoil-U/ethminer'

EXPADDR="$EXP_ADDRESS/$EXP_WORKER"

screen -dmS miner $HCD -S $EXP_POOL -O $EXPADDR:x -U

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

#if [ $GENOILorCLAYMORE == "CLAYMORE" ]
#then
if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

EXPADDR="$EXP_ADDRESS/$EXP_WORKER"

screen -dmS miner $HCD -epool $EXP_POOL -ewal $EXPADDR -epsw x -mode 1 -allpools 1 -dbg -1 $EXP_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi
#fi

if [ $COIN == "ETH" ]
then

if [ $GENOILorCLAYMORE == "GENOIL" ]
then
HCD='/home/m1/eth/Genoil-U/ethminer'

ETHADDR="$ETH_ADDRESS/$ETH_WORKER"

if [ $ETHERMINEdotORG == "YES" ]
then
ETHADDR="$ETH_ADDRESS.$ETH_WORKER"
fi

screen -dmS miner $HCD -S $ETH_POOL -O $ETHADDR:x -U

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $GENOILorCLAYMORE == "CLAYMORE" ]
then
if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

ETHADDR="$ETH_ADDRESS/$ETH_WORKER"

if [ $ETHERMINEdotORG == "YES" ]
then
ETHADDR="$ETH_ADDRESS.$ETH_WORKER"
fi

screen -dmS miner $HCD -epool $ETH_POOL -ewal $ETHADDR -epsw x -mode 1 -dbg -1 $ETH_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi
fi

if [ $COIN == "MUSIC" ]
then

if [ $GENOILorCLAYMORE == "GENOIL-CURRENTLY-NOT-SUPPORTED" ]
then
HCD='/home/m1/eth/Genoil-U/ethminer'

MUSICADDR="$MUSIC_ADDRESS/$MUSIC_WORKER"

screen -dmS miner $HCD -S $MUSIC_POOL -O $MUSICADDR:x -U

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

#if [ $GENOILorCLAYMORE == "CLAYMORE" ]
#then
if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

MUSICADDR="$MUSIC_ADDRESS/$MUSIC_WORKER"

screen -dmS miner $HCD -epool $MUSIC_POOL -ewal $MUSICADDR -epsw x -mode 1 -allpools 1 -dbg -1 $MUSIC_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi
#fi

if [ $COIN == "DCR" ]
then
HCD='/home/m1/pasc/sgminer'
ADDR="$DCR_ADDRESS.$DCR_WORKER"

screen -dmS miner $HCD -k decred -o $DCR_POOL -u $ADDR -p x -p x -I 21 -w 64 -g2

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "PASC" ]
then
HCD='/home/m1/pasc/sgminer'
ADDR="$PASC_ADDRESS..$PASC_WORKER"

screen -dmS miner $HCD -k pascal -o $PASC_POOL -u $ADDR -p x -p x -I 21 -w 64 -g2

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "SIA" ]
then
HCD='/home/m1/SPccminer/ccminer'
SCADDR="$SC_ADDRESS/$SC_WORKER"

screen -dmS miner $HCD -a sia -o $SC_GW_POOL -u $SCADDR -p x

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_ETC_DCR" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

ETCADDR="$ETC_ADDRESS/$ETC_WORKER"

if [ $ETHERMINEdotORG == "YES" ]
then
ETCADDR="$ETC_ADDRESS.$ETC_WORKER"
fi

DADDR="$DCR_ADDRESS.$DCR_WORKER"

screen -dmS miner $HCD -epool $ETC_POOL -ewal $ETCADDR -epsw x -dpool $DCR_POOL -dwal $DADDR -dpsw x -dbg -1 $ETC_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_ETC_PASC" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

ETCADDR="$ETC_ADDRESS/$ETC_WORKER"

if [ $ETHERMINEdotORG == "YES" ]
then
ETCADDR="$ETC_ADDRESS.$ETC_WORKER"
fi

ADDR="$PASC_ADDRESS..$PASC_WORKER"

screen -dmS miner $HCD -epool $ETC_POOL -ewal $ETCADDR -epsw x -dpool $PASC_POOL -dwal $ADDR -dpsw x -dcoin pasc -dbg -1 $ETC_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_ETC_LBC" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

ETCADDR="$ETC_ADDRESS/$ETC_WORKER"

if [ $ETHERMINEdotORG == "YES" ]
then
ETCADDR="$ETC_ADDRESS.$ETC_WORKER"
fi

ADDR="$LBC_ADDRESS.$LBC_WORKER"

screen -dmS miner $HCD -epool $ETC_POOL -ewal $ETCADDR -epsw x -dpool $LBC_POOL -dwal $ADDR -dpsw x -dcoin lbc -dbg -1 $ETC_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_ETC_SC" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

ETCADDR="$ETC_ADDRESS/$ETC_WORKER"

if [ $ETHERMINEdotORG == "YES" ]
then
ETCADDR="$ETC_ADDRESS.$ETC_WORKER"
fi

SCADDR="$SC_ADDRESS/$SC_WORKER"

screen -dmS miner $HCD -epool $ETC_POOL -ewal $ETCADDR -epsw x -allpools 1 -dpool $SC_POOL -dwal $SCADDR -dpsw x -dcoin sc -dcri 70 -dbg -1 $ETC_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_EXP_DCR" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

EXPADDR="$EXP_ADDRESS/$EXP_WORKER"
DADDR="$DCR_ADDRESS.$DCR_WORKER"

screen -dmS miner $HCD -epool $EXP_POOL -ewal $EXPADDR -epsw x -allpools 1 -dpool $DCR_POOL -dwal $DADDR -dpsw x $EXP_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_EXP_PASC" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

EXPADDR="$EXP_ADDRESS/$EXP_WORKER"
ADDR="$PASC_ADDRESS..$PASC_WORKER"

screen -dmS miner $HCD -epool $EXP_POOL -ewal $EXPADDR -epsw x -allpools 1 -dpool $PASC_POOL -dwal $ADDR -dpsw x -dcoin pasc -dbg -1 $EXP_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_EXP_LBC" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

EXPADDR="$EXP_ADDRESS/$EXP_WORKER"
ADDR="$LBC_ADDRESS.$LBC_WORKER"

screen -dmS miner $HCD -epool $EXP_POOL -ewal $EXPADDR -epsw x -allpools 1 -dpool $LBC_POOL -dwal $ADDR -dpsw x -dcoin lbc -dbg -1 $EXP_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_EXP_SC" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

EXPADDR="$EXP_ADDRESS/$EXP_WORKER"
SCADDR="$SC_ADDRESS/$SC_WORKER"

screen -dmS miner $HCD -epool $EXP_POOL -ewal $EXPADDR -epsw x -allpools 1 -dpool $SC_POOL -dwal $SCADDR -dpsw x -dcoin sc -dcri 70 -dbg -1 $EXP_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_MUSIC_DCR" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

MUSICADDR="$MUSIC_ADDRESS/$MUSIC_WORKER"
DADDR="$DCR_ADDRESS.$DCR_WORKER"

screen -dmS miner $HCD -epool $MUSIC_POOL -ewal $MUSICADDR -epsw x -allpools 1 -dpool $DCR_POOL -dwal $DADDR -dpsw x -dbg -1 $MUSIC_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_MUSIC_PASC" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

MUSICADDR="$MUSIC_ADDRESS/$MUSIC_WORKER"
ADDR="$PASC_ADDRESS..$PASC_WORKER"

screen -dmS miner $HCD -epool $MUSIC_POOL -ewal $MUSICADDR -epsw x -allpools 1 -dpool $PASC_POOL -dwal $ADDR -dpsw x -dcoin pasc -dbg -1 $MUSIC_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_MUSIC_LBC" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

MUSICADDR="$MUSIC_ADDRESS/$MUSIC_WORKER"
ADDR="$LBC_ADDRESS.$LBC_WORKER"

screen -dmS miner $HCD -epool $MUSIC_POOL -ewal $MUSICADDR -epsw x -allpools 1 -dpool $LBC_POOL -dwal $ADDR -dpsw x -dcoin lbc -dbg -1 $MUSIC_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_MUSIC_SC" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

MUSICADDR="$MUSIC_ADDRESS/$MUSIC_WORKER"
SCADDR="$SC_ADDRESS/$SC_WORKER"

screen -dmS miner $HCD -epool $MUSIC_POOL -ewal $MUSICADDR -epsw x -allpools 1 -dpool $SC_POOL -dwal $SCADDR -dpsw x -dcoin sc -dcri 70 -dbg -1 $MUSIC_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_ETH_DCR" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

ETHADDR="$ETH_ADDRESS/$ETH_WORKER"

if [ $ETHERMINEdotORG == "YES" ]
then
ETHADDR="$ETH_ADDRESS.$ETH_WORKER"
fi

DADDR="$DCR_ADDRESS.$DCR_WORKER"

screen -dmS miner $HCD -epool $ETH_POOL -ewal $ETHADDR -epsw x -dpool $DCR_POOL -dwal $DADDR -dpsw x -dbg -1 $ETH_EXTENTION_ARGUMENTS


if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_ETH_PASC" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

ETHADDR="$ETH_ADDRESS/$ETH_WORKER"

if [ $ETHERMINEdotORG == "YES" ]
then
ETHADDR="$ETH_ADDRESS.$ETH_WORKER"
fi

ADDR="$PASC_ADDRESS..$PASC_WORKER"

screen -dmS miner $HCD -epool $ETH_POOL -ewal $ETHADDR -epsw x -dpool $PASC_POOL -dwal $ADDR -dpsw x -dcoin pasc -dbg -1 $ETH_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_ETH_LBC" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

ETHADDR="$ETH_ADDRESS/$ETH_WORKER"

if [ $ETHERMINEdotORG == "YES" ]
then
ETHADDR="$ETH_ADDRESS.$ETH_WORKER"
fi

ADDR="$LBC_ADDRESS.$LBC_WORKER"

screen -dmS miner $HCD -epool $ETH_POOL -ewal $ETHADDR -epsw x -dpool $LBC_POOL -dwal $ADDR -dpsw x -dcoin lbc -dbg -1 $ETH_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

if [ $COIN == "DUAL_ETH_SC" ]
then

if [ $CLAYMORE_VERSION == "9_7" ]
then
HCD='/home/m1/eth/9_7/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_5" ]
then
HCD='/home/m1/eth/9_5/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "9_4" ]
then
HCD='/home/m1/eth/9_4/ethdcrminer64'
fi

if [ $CLAYMORE_VERSION == "8_0" ]
then
HCD='/home/m1/eth/8_0/ethdcrminer64'
fi

ETHADDR="$ETH_ADDRESS/$ETH_WORKER"

if [ $ETHERMINEdotORG == "YES" ]
then
ETHADDR="$ETH_ADDRESS.$ETH_WORKER"
fi

SCADDR="$SC_ADDRESS/$SC_WORKER"

screen -dmS miner $HCD -epool $ETH_POOL -ewal $ETHADDR -epsw x -allpools 1 -dpool $SC_POOL -dwal $SCADDR -dpsw x -dcoin sc -dcri 70 -dbg -1 $ETH_EXTENTION_ARGUMENTS

if [ $LOCALorREMOTE == "LOCAL" ]
then
screen -r miner
fi

BITCOIN="theGROUND"

while [ $BITCOIN == "theGROUND" ]
do
sleep 60
done
fi

fi
