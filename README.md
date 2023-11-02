# Open5GS & OpenAirInterface UE / RAN, simple UPF by focous on accessing to File_sharing_Platform, Streaming and Sip_Call_Server Sample Configuration

## Table of Contents
* [Introduction to 5GS Network Components Functionality](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#introduction-to-5gs-network-components-functionality)
* [Design](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#design)
* [Requirements](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#Requirements)
* [Description of tap device](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#description-of-tap-device)
* [Running Virtual Machines](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#running-virtual-machines)
* [Configuring network setting of virtual machines](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#configuring-network-setting-of-virtual-machines)
* [Configuring 5G network Components](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#configuring-5g-network-Components)
* [Configuring U-Plane](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#configuring-u-plane)
* [Configuring_UE_RAN](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#configuring_ue_ran)
* [Configuring Core_Plane](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#configuring-core_plane)
* [Running C-Plane](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#running-c-plane)
* [Adding UEs](https://github.com/FRA-UAS/mobcom-project-lte#adding-ues)
* [Glossary](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#glossary)
* [PacketTraces](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/README.md#PacketTraces)




# Introduction to 5GS Network Components Functionality

In a 5G network, several core network components work together to provide end-to-end connectivity and service delivery to users. 
Here is a high-level overview of how these components work together:


* User Equipment (UE): The UE is the user's device, such as a smartphone or tablet, that connects to the 5G network.

* Radio Access Network (RAN): The RAN consists of base stations that provide wireless connectivity between the UE and the 5G core network.

* 5G Core Network: The 5G core network is a set of network functions that provide key services such as authentication, session management, policy control, and charging.

* Access and Mobility Management Function (AMF): The AMF is responsible for managing user authentication, authorization, and mobility within the network.

* Session Management Function (SMF): The SMF is responsible for establishing and managing data sessions between the user's device and the network.

* Policy Control Function (PCF): The PCF manages policy rules that control how network resources are allocated and used by different network services and users.

* Network Repository Function (NRF): The NRF maintains a registry of available network functions and their associated capabilities, which other network functions can query to discover available services.

* User Plane Function (UPF): The UPF is responsible for routing data packets between the user's device and the network, and for enforcing policy rules related to QoS and network resources.





These components work together to provide end-to-end connectivity and service delivery to users. For example, when a user initiates a data session, the UE communicates with the RAN to establish a wireless connection to the 5G core network. The AMF authenticates the user and authorizes their access to the network, while the SMF establishes and manages the data session. The PCF enforces policy rules related to QoS and network resources, while the UPF routes data packets between the user's device and the network. The NRF helps other network functions discover available services and make informed service selection decisions. Overall, these components work together to provide a flexible, service-oriented network architecture that can support a wide range of use cases and service requirements.




# Design 

Figure 1. Overall infrastructure

![Overal infrastructure](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/Overall/infra.jpg)


Figure 1 illustrates the overall setting used for the virtual machines to setup the system.


Note that in our C-Plane machine Its asked to config SMF, NRF and PCF.
This networked is configues to have access to Sip-Call-Server, Streaming and File-Sharing Service.


# Requirements

Here is the minimum requirements for our Network.

Table 1. Virtual machines for the simulating of UE/RAN and deploying C-Plane and single U-Plane.

| Machine ID | Function              | IP/MAC Address <br> enp0s3  | IP/MAC Address  <br> enp0s4  | RAM  | CPU | HDD |Operating system |
| ---------- | --------------------- | ------------- | ------------- | ---- | --- | --- | ------------------ |
| machine 01 | UE/RAN Simulation     | 192.168.0.120 <br> 52:54:00:12:34:51 | 192.168.0.125 <br> 52:54:00:12:34:61 | 8 GB | 2 | 40GB | Ubuntu 18.04 |
| machine 02 | C-Plane               | 192.168.0.121 <br> 52:54:00:12:34:52 | 192.168.0.126 <br> 52:54:00:12:34:62 | 8 GB | 2 | 40GB | Ubuntu 18.04 |
| machine 03 | UPF                   | 192.168.0.122 <br> 52:54:00:12:34:53 | 192.168.0.127 <br> 52:54:00:12:34:63 | 8 GB | 2 | 40GB |Ubuntu 18.04 |




The system ’s main IP address is 192.168.0.0/24, indicating that all machines within the system are interconnected via this designated network range. 



## Description of tap device:
➡ Tap devices are often used in virtualization technologies such as containers and virtual machines to imitate a network interface that so many other virtual devices can access.

A tap device is a virtual network interface that allows data to be diverted from one network device to another. 

It is also known as a virtual tap interface or TAP interface.

In virtualization environments, tap devices are used to connect virtual machines or containers to a virtual network, enabling communication between virtual devices and the outside world.

The exact number and configuration of tap devices used in Open5GS will depend on the specific use case and network topology being simulated.

here according to the project description, we configured 2 tap devices for each virtual machine.

for example, each upf has 3 Tap devices because it has 3 interfaces N3, N4 and N6 respectively for connecting to OAI-RAN, 5GS-core-Network and Internet.

or UE-RAN has 3 tap devices because it has 3 interfaces named N1 for connecting UE from UE-RAN to the 5GS-Core-Network, N2 for connecting OAI-RAN from UE-RAN to the 5GS-Core-Network and N3 for connecting UE-RAN to the UPF.

or C-Plane virtual machine has 3 tap devices because it has 3 interfaces named N1 for connecting to UE from UE-RAN, N2 for connecting to OAI-RAN from UE-RAN and N3 for connecting UE-RAN to the UPF.




## Initializing tap devices 

Here we have used Tap devices for data transmission between one network device to another. 
In addition, to have access from this 5G network elements to the Internet.



To create a tap devices we use the following script, which iterates for 
6 times and create a new tap device in each iteration. We dedicate two 
tap devices for each virtual machine.


```bash
sudo brctl addbr ggbr0
sudo ip link set ggbr0 up


for i in 1 2 3 4 5 6 
do
    sudo ip tuntap add dev ggtap$i mode tap user student
    sudo ip link set dev ggtap$i up
    sudo brctl addif ggbr0 ggtap$i
done
```

We have used this code on our own main system which is an Ubuntu system.

Here is the result of executing the above code

![TapDevicesInitialization](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/Overall/ggtap.jpg)


⭐ Note that each time after termination of your system you should run this code again because after system termination this settings will disapper.



#### Code description


```bash
sudo brctl addbr ggbr0
```
With this command, we will create a virtual bridge named "ggbr0".

This command is used to create a virtual bridge named "ggbr0" using the brctl tool on a Linux system. 

The brctl tool is used to manage and manipulate the Linux bridge, which is a layer 2 virtual device that can be used to connect multiple network interfaces together, creating a single virtual network interface.

The addbr option is used to create a new bridge and the ggbr0 is the name of the bridge.



```bash
sudo ip tuntap add dev ggtap${i} mode tap u
```
This is a command in Linux to create a TUN/TAP device. 

The options used in this command are:

dev ggtap${i} specifies the name of the TUN/TAP device to be created. In this case, the device name is "ggtap${i}".

mode tap specifies the type of device to create, either TUN (network TUNnel) or TAP (Ethernet TAP). In this case, TAP mode is selected.

u specifies that the device should be created with user ownership, meaning that it can be used by a non-root user.

⭐ This command requires root privileges, which is why sudo is used to run it with elevated permissions.



<br>



```bash
sudo ip link set dev ggtap${i} up
```

This is a command in Linux to activate a network interface.

The options used in this command are:

dev ggtap${i} specifies the name of the network interface to be activated. In this case, the interface name is "ggtap${i}".

up specifies the state of the interface, either "up" to activate it or "down" to deactivate it. In this case, the interface is set to "up" to activate it.

This command requires root privileges, which is why sudo is used to run it with elevated permissions. 

⭐ Once the interface is activated, it becomes visible to the system and can be used for network communication.


<br>

```bash
sudo brctl addif ggbr0 ggtap${i}
```
This is a command in Linux to add a network interface to a bridge device.


The options used in this command are:

ggbr0 specifies the name of the bridge device. A bridge device is a software-defined network switch that allows multiple network interfaces to be connected together.

ggtap${i} specifies the name of the network interface to be added to the bridge.

This command requires root privileges, which is why sudo is used to run it with elevated permissions. 

⭐ After the network interface is added to the bridge, it becomes part of the bridge and will participate in the network communication through the bridge.


....................................................................................................................................................................................................................................


As we run the script using the `ip` command, we can see the tap devices are 
created and added to our bridge properly.
```bash
$ sudo ip addr show | egrep ggtap*
135: ggtap1: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast master ggbr0 state UP group default qlen 1000
136: ggtap2: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast master ggbr0 state UP group default qlen 1000
137: ggtap3: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast master ggbr0 state UP group default qlen 1000
138: ggtap4: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast master ggbr0 state UP group default qlen 1000
139: ggtap5: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast master ggbr0 state UP group default qlen 1000
141: ggtap6: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast master ggbr0 state UP group default qlen 1000
```

....................................................................................................................................................................................................................................


We set the interfaces for each virtual machine: Here is the setting process for UERANSIM as an example


![TapDevices](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/Overall/Tapdevices.jpg)



....................................................................................................................................................................................................................................

## Running Virtual Machines 
The following script is utilized for the purpose of running virtual machines, wherein it accepts 
a single argument in the form of an integer. This integer serves as an indication of the ID 
of the virtual machine that is to be initiated. The table 1, presented in this study, provides 
a comprehensive summary of the various machine IDs that have been incorporated in the design process.

The script uses QEMU as the platform for virtualization. The virtual machine is being configured with the 
following parameters:

* `initrd`: We use initrd image "initrd.img-5.4.0-84-generic" 
* `kernel`: The kernel "vmlinuz-5.4.0-84-generic" is used 
* `nographic -monitor none -serial stdio`: As we have limited bandwidth the the server running virtual machine, we decided to use terminal interface, and therefore no graphical display and no monitor is used, and we set the output with serial output as the console
* `-append`: Appending "root=/dev/vda1 console=ttyS0" to the kernel command line
* `-machine q35 -cpu host`: Using the Q35 machine type and host CPU
* `-drive`: Attaching a qcow2 formatted disk image as a virtio drive
* `-enable-kvm`: Enabling KVM for hardware acceleration
* `-device ... -netdev ...` For the networking configuration 2 virtio 
network devices, each connected to a separate TAP interface 
`ggtap${tap1}` and `ggtap${tap2}`
* `-net user, ... `: For the purpose of connecting to virtual machine with `ssh` we forwarded host port `1002${machineName}` to port 22 on the virtual machine
* `-m MEMORY -smp CORES`: We Allocated 8GB of memory and 2 CPU cores to the virtual machine.
```bash
#!/usr/bin/env bash

set -ex


machineName=$1
tap1=$machineName
tap2=$((machineName+5))

STTY_SETTINGS="$( stty -g )"

stty intr ^]
stty susp ^]

cnt=$(($cnt+1))
# Parameters.
id=ubuntu-18.04.6-desktop-amd64
disk_img="base.img"
disk_img_snapshot="machine-0${machineName}.snapshot.qcow2"

if [[ $machineName == help ]]; then
        echo "virtual-manager.sh is a script for running virtual machines"
        echo "usage virtual-manager.sh image [tap|proxy] [index]"
fi


qemu-system-x86_64 \
        -initrd initrd.img-5.4.0-84-generic \
        -kernel vmlinuz-5.4.0-84-generic \
        -nographic -monitor none -serial stdio \
        -append 'root=/dev/vda1 console=ttyS0' \
        -machine q35 -cpu host \
        -drive "file=${disk_img_snapshot},format=qcow2,if=virtio" \
        -enable-kvm \
        -netdev tap,ifname=ggtap${tap1},script=no,downscript=no,vhost=on,id=nInt\
        -device virtio-net-pci,mac=52:54:00:12:34:5${tap1},netdev=nInt \
        -netdev tap,ifname=ggtap${tap2},script=no,downscript=no,vhost=on,id=mInt\
        -device virtio-net-pci,mac=52:54:00:12:34:6${tap1},netdev=mInt \
        -net user,hostfwd=tcp::1002${machineName}-:22 \
        -net nic \
        -m 8G \
        -smp 2 \
        ;

stty "$STTY_SETTINGS"
```


## Configuring network setting of virtual machines 

We set the ip addresses of the two interfaces our VMS have by adding the 
following files to `/etc/network/` directory.

```
# /etc/network/interfaces
# interfaces(5) file used by ifup(8) and ifdown(8)
auto lo
iface lo inet loopback
source /etc/network/interfaces.d/*
```

```
# /etc/network/interfaces.d/enp0s8
auto enp0s8
iface enp0s3 inet static
address 192.168.0.120
netmask 255.255.255.0
network 192.168.0.0
broadcast 192.168.0.255
```

```
# /etc/network/interfaces.d/enp0s9
auto enp0s9
iface enp0s4 inet static
address 192.168.0.125
netmask 255.255.255.0
network 192.168.0.0
broadcast 192.168.0.255
```

After network configuration of all the virtual machines, we were able to 
ping each virtual machine from the other one. The following code block 
shows that ping messages traverse each virtual machine interface to 
its tap device and from the tap device via bridge to the other tap device
and to the virtual machine of destination.

```
$ ping 192.168.0.121
PING 192.168.0.121 (192.168.0.121) 56(84) bytes of data.
64 bytes from 192.168.0.121: icmp_seq=1 ttl=64 time=0.523 ms
64 bytes from 192.168.0.121: icmp_seq=2 ttl=64 time=0.692 ms
```


```
$ sudo tcpdump -i ggtap1
tcpdump: verbose output suppressed, use -v[v]... for full protocol decode
listening on ggtap1, link-type EN10MB (Ethernet), snapshot length 262144 bytes
21:16:11.623712 IP 192.168.0.120 > 192.168.0.121: ICMP echo request, id 8327, seq 5, length 64
21:16:11.624145 IP 192.168.0.121 > 192.168.0.120: ICMP echo reply, id 8327, seq 5, length 64      
```

```
$ sudo tcpdump -i ggtap2
tcpdump: verbose output suppressed, use -v[v]... for full protocol decode
listening on ggtap2, link-type EN10MB (Ethernet), snapshot length 262144 bytes
21:16:21.779241 ARP, Request who-has 192.168.0.120 tell 192.168.0.121, length 28
21:16:21.779680 ARP, Reply 192.168.0.120 is-at 52:54:00:12:34:51 (oui Unknown), length 28
21:16:21.863620 IP 192.168.0.120 > 192.168.0.121: ICMP echo request, id 8327, seq 15, length 64
21:16:21.863924 IP 192.168.0.121 > 192.168.0.120: ICMP echo reply, id 8327, seq 15, length 64
```







....................................................................................................................................................................................................................................

### Tap device Configurations


hen we create a tap device inside `U-Plane` virtual machine using 
the following command.

```bash
sudo ip tuntap add dev osgtun1 mode tap
sudo ip link set dev osgtun1 up
sudo ip addr add 10.45.0.1/16 dev osgtun1
sudo iptables -t nat -A postrouting -s 10.46.0.0/16 ! -o ogstun2 -j MASQUERADE
```


The natting Command here is:

```
sudo iptables -t nat -A POSTROUTING -s 10.47.0.0/16 ! -o ogstun3 -j MASQUERADE
```
This command sets up NAT rules for traffic coming from the 10.47.0.0/16 subnet, so that it can be translated by the NAT gateway and sent out to the Internet through the appropriate interface while hiding the private IP addresses of the hosts in that subnet.




at the time of configuration of osgtun I have received numerous errors the result of that was My user was guest after changing it to client I fixed the issue.



so till now a tap device is created.


Then we should restart the network by command:


```
sudo systemctl restart networking
```




after 

```
sudo systemctl restart networking
```

the networking service is restarted, which involves stopping the service, making any necessary changes or updates, and then starting the service again with the new configuration.



After Configuration by this command we have checked if the network interfaces Ip addresses has changed:

```bash
ip addr show
```

sudo ip link set osgtun up


..........................................................................................................................................................................

# Prepairing Virtual Machines by Installing Open5gs and OpenAirInterface on them

* On 2 of Virtual Machines (C-Plane and U-Plane) we install Open5GS
* on UERAN machine we will install OpenAirInterface


To check if the Open5GS is installed and its functions are working:

```
sudo service open5gs-amfd status
```

or

```
systemctl status open5gs*
```



..........................................................................................................................................................................

# Configuring 5G network Components


## Configuring_UE_RAN


### Changes in configuration files of RAN:



 * "rcc.band7.tm1.nfapi.conf"
 
 
```
cd Projects/enb/ci-scripts-conf_files
vim rcc.band7.tm1.nfapi.conf
```
 
 
 Here the configured part is shows 
 
 

![RANConfig](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/NewVersion/NewVersion/UERANSIM/OAI/rccbandtm1nfapi.jpg)

![RANConfig1](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/NewVersion/NewVersion/UERANSIM/OAI/rccbandpart2.jpg)



### Changes in configuration files of UE:  

* "ue.nfapi.conf"

```
cd Projects/ue/ci-scripts/conf_files
vim ue.nfapi.conf
```

 Here the configured part is shows


![nfapi](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/NewVersion/NewVersion/UERANSIM/UE/nfapi.jpg)


## Configuring Core_Plane


* configuring mme


```
cd Projects/open5gs/install/etc/open5gs
vim mme.yaml
```

Here the configured part is shows



![mme](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/NewVersion/NewVersion/CorePlane/mme1.jpg)

![mme1](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/NewVersion/NewVersion/CorePlane/mme2.png)


* configuring sgwc


```
cd Projects/open5gs/install/etc/open5gs
vim sgwc.yaml
```

Here the configured part is shows


![sgwc](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/NewVersion/NewVersion/CorePlane/sgwc.jpg)

![Sgwc1](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/NewVersion/NewVersion/CorePlane/sgwc1.jpg)



* configuring smf


```
cd Projects/open5gs/install/etc/open5gs
vim smf.yaml
```

Here the configured part is shows


![smf](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/NewVersion/NewVersion/CorePlane/smf.jpg)

![smf1](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/NewVersion/NewVersion/CorePlane/smf1.jpg)



## Configuring U_Plane

➡ UPF (User Plane Function) is a key component in the architecture of 5G networks. It is responsible for forwarding user data (the "user plane") between the 5G Radio Access Network (RAN) and the core network. The UPF is the main point of interaction between the RAN and the core network, and it performs functions such as packet filtering, routing, and traffic management.

The UPF is designed to handle the large amounts of data traffic generated by 5G devices and networks, and to ensure that this data is delivered quickly, reliably, and securely. The UPF is a critical component in enabling the high speeds and low latency that are key features of 5G networks.


By enetring upf.yaml and going to line 173, we have changed the ip address to the ip address that we considered for upf of Sip U-Plane. Which is the ip address of enp0s9 which we considered as 192.168.0.127.

* configuring upf


```
cd Projects/open5gs/install/etc/open5gs
vim upf.yaml
```

This is a configuration file written in YAML format. 
It contains information about network settings for a certain application or system.


```bash
  1 upf:
  2     pfcp:
  3       - addr: 192.168.0.127
  4     gtpu:
  5       - addr: 192.168.0.127
  6     subnet:
  7       - addr: 10.45.0.1/16
  8         dnn: streaming
  9         dev: osgtun1
  10        addr: 10.46.0.1/16
  11         dnn: voip
  12        dev: osgtun2
  13        addr: 10.47.0.1/16
  14        dnn: filesharing
  15        dev: osgtun3
  16    metrics:
  17      - addr: 127.0.0.7
  18        port: 9090

```


Here's what each line means:

It is a configuration file written in YAML format.
It contains information about network settings for a certain application or system. (Here Sip_Call_Server, FileSharing and Streaming)


1) "upf" refers to a user plane function. This configuration is for a single UPF. 
2) The UPF has a PFCP (Packet Forwarding Control Protocol) configuration.
    The PFCP configuration has a single address (192.168.0.127).
3) The UPF also has a GTP-U (GPRS Tunnelling Protocol - User Plane) configuration.
     The GTP-U configuration also has a single address (192.168.0.127).
4) The UPF has a subnet configuration with public addresses of ( 10.45.0.1/16, 10.46.0.1/16, 10.47.0.1/16). This address is the network address for a subnet with a subnet mask of 255.255.0.0. 
    The subnet is associated with a Data Network Name (DNN) of filesharing for File_Sharing, Voip for Sip_Call_Server and Streaming for Streaming use, and is accessible through the devices osgtun3, osgtun2 and osgtun1 respectively.
    The subnet configuration also specifies a DNN.
    The subnet configuration also specifies the device (osgtun2 for example) through which the subnet is accessible.
5) The UPF has a metrics configuration with a single address (127.0.0.7) and a port (9090). This configuration could be used for monitoring or other management purposes.


Hints:

*  SIP clients usually use port number 5060 for non-encrypted signaling traffic(UDP) to connect to SIP servers and other SIP endpoints.


Here the configured part is shows

![upf](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/NewVersion/NewVersion/UPlane/upf.jpg)


* configuring sgwu


```
cd Projects/open5gs/install/etc/open5gs
vim sgwu.yaml
```


By enetring sgwu.yaml and going to line 98, we have changed the ip address to the ip address that we considered for sgwu of U-Plane. Which is the ip address of enp0s8 which we considered as 192.168.0.122.

Here the configured part is shows

![sgw](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/NewVersion/NewVersion/UPlane/sgwu.jpg)


..........................................................................................................................................................................



1. We run mmed using the following command
```
client@client:~/open5gs/install/bin$ sudo ./open5gs-mmed
Open5GS daemon v2.6.0-15-gb790572

02/08 22:17:04.766: [app] INFO: Configuration: '/home/client/open5gs/install/etc/open5gs/mme.yaml' (../lib/app/ogs-init.c:126)
02/08 22:17:04.766: [app] INFO: File Logging: '/home/client/open5gs/install/var/log/open5gs/mme.log' (../lib/app/ogs-init.c:129)
02/08 22:17:04.784: [metrics] INFO: metrics_server() [http://127.0.0.2]:9090 (../lib/metrics/prometheus/context.c:511)
02/08 22:17:04.852: [gtp] INFO: gtp_server() [127.0.0.2]:2123 (../lib/gtp/path.c:31)
02/08 22:17:04.852: [gtp] INFO: gtp_connect() [127.0.0.3]:2123 (../lib/gtp/path.c:61)
02/08 22:17:04.852: [mme] INFO: s1ap_server() [192.168.0.121]:36412 (../src/mme/s1ap-sctp.c:63)
02/08 22:17:04.852: [sctp] INFO: MME initialize...done (../src/mme/app-init.c:33)
```
as you can see the MME initialiyation is done by using the protocol sctp.



2. We run control plane gateway using the following command
```
client@client:~/open5gs/install/bin$ sudo ./open5gs-sgwcd
Open5GS daemon v2.6.0-15-gb790572

02/08 22:19:28.244: [app] INFO: Configuration: '/home/client/open5gs/install/etc/open5gs/sgwc.yaml' (../lib/app/ogs-init.c:126)
02/08 22:19:28.244: [app] INFO: File Logging: '/home/client/open5gs/install/var/log/open5gs/sgwc.log' (../lib/app/ogs-init.c:129)
02/08 22:19:28.264: [gtp] INFO: gtp_server() [127.0.0.3]:2123 (../lib/gtp/path.c:31)
02/08 22:19:28.264: [pfcp] INFO: pfcp_server() [192.168.0.121]:8805 (../lib/pfcp/path.c:31)
02/08 22:19:28.264: [pfcp] INFO: ogs_pfcp_connect() [192.168.0.122]:8805 (../lib/pfcp/path.c:62)
02/08 22:19:28.264: [pfcp] INFO: ogs_pfcp_connect() [192.168.0.123]:8805 (../lib/pfcp/path.c:62)
02/08 22:19:28.264: [pfcp] INFO: ogs_pfcp_connect() [192.168.0.124]:8805 (../lib/pfcp/path.c:62)
02/08 22:19:28.265: [app] INFO: SGW-C initialize...done (../src/sgwc/app.c:31)
02/08 22:19:35.773: [pfcp] WARNING: [1] LOCAL  No Reponse. Give up! for step 1 type 5 peer [192.168.0.122]:8805 (../lib/pfcp/xact.c:619)
02/08 22:19:35.773: [pfcp] WARNING: [2] LOCAL  No Reponse. Give up! for step 1 type 5 peer [192.168.0.123]:8805 (../lib/pfcp/xact.c:619)
02/08 22:19:35.773: [pfcp] WARNING: [3] LOCAL  No Reponse. Give up! for step 1 type 5 peer [192.168.0.124]:8805 (../lib/pfcp/xact.c:619)
02/08 22:19:39.268: [sgwc] WARNING: Retry to association with peer [192.168.0.122]:8805 failed (../src/sgwc/pfcp-sm.c:106)
02/08 22:19:39.269: [sgwc] WARNING: Retry to association with peer [192.168.0.123]:8805 failed (../src/sgwc/pfcp-sm.c:106)
02/08 22:19:39.269: [sgwc] WARNING: Retry to association with peer [192.168.0.124]:8805 failed (../src/sgwc/pfcp-sm.c:106)
02/08 22:19:46.777: [pfcp] WARNING: [4] LOCAL  No Reponse. Give up! for step 1 type 5 peer [192.168.0.122]:8805 (../lib/pfcp/xact.c:619)
02/08 22:19:46.777: [pfcp] WARNING: [5] LOCAL  No Reponse. Give up! for step 1 type 5 peer [192.168.0.123]:8805 (../lib/pfcp/xact.c:619)
02/08 22:19:46.777: [pfcp] WARNING: [6] LOCAL  No Reponse. Give up! for step 1 type 5 peer [192.168.0.124]:8805 (../lib/pfcp/xact.c:619)
```

..........................................................................................................................................................................


## Adding UEs

We can ass sucscribers by the following command

```
UE # IMSI APN OP/OPc
```

for example

```
UE0 001010000000100 internet1 OPc
```

or

```
UE3 001010000000102 streaming OPc
```


##### here is the description of the code:


* UE: UE stands for User Equipment. It is a mobile device that can connect to a 5G network.

* IMSI: IMSI stands for International Mobile Subscriber Identity. It is a unique identification number assigned to a SIM card. This number is used to identify the subscriber and authenticate them on the network.

* APN: APN stands for Access Point Name. It is the name of the gateway between a mobile network and another network, such as the Internet. Each mobile operator has its own APN.

* OP/OPc: OP/OPc refers to the Operator Variant and Operator Variant Configuration. These are unique identifiers used to authenticate the mobile device on the network. They are used to protect the network from unauthorized access.

In summary, UE is the mobile device, IMSI is the unique identification number of the SIM card, APN is the gateway between the mobile network and another network, and OP/OPc are unique identifiers used to authenticate the mobile device on the network.



## Glossary

| Abbreviation         | Explanation        |
| -------------------- | ------- |
| [amf](#amf)          | Access and Mobility Management Function  |
| [nrf](#nrf)          |  Network Repository Function  |
| [pcf](#pcf)          | Policy Control Function  |
| [mmed](#mmed)        | Mobility Management Entity Deamon |
| [sgwcd](#sgwcd)      | Serving Gateway Control Plane Deamon |
| [smfd](#smfd)          | Service Management Function Deamon |
| [hssd](#hssd)        | Home Subscriber Server Deamon |



### amf
AMF (Access and Mobility Management Function), is a key component of the 5G core network that is responsible for managing user authentication, authorization, and mobility within the network.

The AMF performs several functions, including:

*    Authentication: The AMF authenticates the user's identity and verifies that they are authorized to access the network.

*    Authorization: The AMF determines the user's access rights based on their subscription profile, which includes information such as the services they are authorized to use and their quality of service (QoS) requirements.

*    Session Management: The AMF manages the user's connection to the network, including establishing and terminating sessions, monitoring user activity, and enforcing policies.

 *   Mobility Management: The AMF manages the user's mobility within the network, including handovers between different cells or base stations, and tracking the user's location as they move through the network.

Overall, the AMF plays a critical role in ensuring that users can securely and reliably access 5G network services, while also maintaining the quality of service and managing network resources efficiently.




### nrf
In 5G, NRF stands for "Network Repository Function". It is a core network component responsible for storing and managing network function descriptions, which are used by other network functions to discover and access network services.

The NRF performs several functions, including:

* Service discovery: The NRF maintains a registry of available network functions and their associated capabilities, which other network functions can query to discover available services.

* Network function selection: The NRF can provide recommendations on which network function to use for a particular service, based on factors such as network conditions, QoS requirements, and network policies.

* Load balancing: The NRF can distribute requests for network services across multiple network functions to ensure that resources are used efficiently and that service availability is maintained.

* Network slicing: The NRF can help to manage network slicing, which is a key feature of 5G that allows network resources to be partitioned and allocated to different services or user groups.


Overall, the NRF plays a critical role in enabling the dynamic, service-oriented nature of 5G networks, where network functions can be quickly discovered, accessed, and composed to support a wide range of use cases and service requirements.




### pcf

n 5G, PCF stands for "Policy Control Function". It is a core network component responsible for managing policy rules that control how network resources are allocated and used by different network services and users.

The PCF performs several functions, including:

* Policy rule management: The PCF manages policy rules that define how network resources are allocated and used by different network services and users. These rules can be based on factors such as user identity, QoS requirements, and network conditions.


* Policy decision making: The PCF makes policy decisions based on input from other network functions, such as the SMF and the UPF. These decisions can determine how network resources are allocated and used, and can be based on real-time network conditions and user needs.


* Policy enforcement: The PCF enforces policy rules across the network, ensuring that resources are used efficiently and that the quality of service for different services and users is maintained.

* Charging: The PCF is responsible for tracking network usage and generating usage records for charging purposes.

Overall, the PCF plays a critical role in enabling 5G networks to support a wide range of use cases and service requirements, while also managing network resources efficiently and maintaining a high quality of service for users.



### mmed
MME (Mobility Management Entity) is a key component in 5G networks responsible for managing and controlling the flow 
of user data in the network. The MME is responsible for several functions, including user authentication, network entry 
and exit, and handling of user mobility between different cells in the network.

In 5G networks, the MME operates in the control plane and is separate from the UPF (User Plane Function), 
which is responsible for forwarding user data in the user plane. The MME is responsible for maintaining information 
about the location of each user and ensuring that user data is correctly forwarded to the appropriate network 
elements as the user moves between different cells in the network.

The MME also plays a key role in maintaining the security of the network, as it is responsible for authenticating 
users and encrypting user data to ensure its confidentiality. In addition, the MME is responsible for handling 
the signaling required for the establishment and release of user connections, and for handling the handover of 
user connections between different cells in the network.

In summary, the MME is a central control element in 5G networks that plays a critical role in managing and controlling 
the flow of user data, maintaining network security, and supporting user mobility.


### sgwcd
SGW-C stands for Serving Gateway Control plane in 5G networks. It is a key component of the 5G core network architecture 
and is responsible for managing and controlling the flow of user data between the mobile network and the external packet 
data network (PDN). The SGW-C performs several important functions, including user plane traffic forwarding, policy 
enforcement, and management of user mobility between different cells in the network.

In 5G networks, the SGW-C operates in the control plane and is separate from the Serving Gateway User Plane (SGW-U), 
which is responsible for forwarding user data in the user plane. The split between the SGW-C and SGW-U allows for 
greater scalability and flexibility in the network, enabling the network to efficiently manage and control the large 
volumes of user data that are generated in a 5G network.


### smfd
SMF (Service Management Function) is a key component in 5G networks responsible for managing and controlling the 
flow of user data in the network. The SMF is responsible for several functions, including network slice selection, 
policy enforcement, and user plane traffic forwarding.

The SMF performs functions, including:

* Session establishment: The SMF is responsible for establishing data sessions between the user's device and the network, including setting up security associations and negotiating QoS parameters.

* Policy enforcement: The SMF enforces policy rules related to user access, QoS, and network resources. This includes ensuring that the user is authorized to access the requested service and that the network has sufficient resources to support the session.

* Charging: The SMF tracks and records usage data for charging purposes, including the amount of data transmitted and received, and the duration of the session.

* Session termination: The SMF is responsible for terminating data sessions when the user has completed their session or when an event triggers the session to end.




In 5G networks, the SMF is implemented as a network function that operates in the control plane and is separate from 
the UPF (User Plane Function), which is responsible for forwarding user data in the user plane. The split between the SMF 
and UPF allows for greater scalability and flexibility in the network, enabling the network to efficiently manage and 
control the large volumes of user data that are generated in a 5G network. 

It works closely with other 5G core network components, such as the AMF and UPF (User Plane Function), 
to ensure that data sessions are established and managed efficiently and securely. 



The SMF also plays a key role in supporting network slicing, which is a key feature of 5G networks. Network slicing 
allows different types of user traffic to be separated and treated differently, based on their specific requirements. 
The SMF is responsible for selecting the appropriate network slice for each user session and managing the flow of user 
data through the appropriate slice. 

Overall, the SMF plays a critical role in enabling 5G network services and ensuring a high quality of service for users.


### hssd
HSS stands for Home Subscriber Server in 5G networks. It is a central database that stores information about subscribers 
and their services, such as their identities, profiles, and security keys. The HSS is a key component of the 5G core 
network architecture and is used by other network functions, such as the MME (Mobility Management Entity) and the SMF 
(Service Management Function), to manage and control the flow of user data in the network.

In 5G networks, the HSS plays a critical role in managing user identities and maintaining the security of the network. 
It stores user-specific information, such as authentication and authorization data, and provides this information to 
other network functions as needed. The HSS also plays a key role in supporting network slicing, which is a key feature 
of 5G networks. Network slicing allows different types of user traffic to be separated and treated differently, 
based on their specific requirements. The HSS is responsible for storing information about the network slices available 
to each user and providing this information to the SMF, which is responsible for selecting the appropriate network 
slice for each user session.



# PacketTraces

* Uplane and Coreplane


![CorePlaneToUplane](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/WiresharkDetails/CplaneUplane/cplaneuplane.jpg)


* Enodeb to Core-lane

![EnodeBtoCorePlane](https://github.com/FRA-UAS/mobcom-project-lte/blob/main/Figures/WiresharkDetails/enb-cplane/enb-cplane.jpg)



## Help and Suppurt
Please ask your question by [email](mahdieh.pirmoradian@stud.fra-uas.de), if you haev any question or problem related to this project or in configuration of it.
maximum in 2 weeks I will answer :)

