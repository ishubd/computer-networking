# MAC Address

In order to transfer data from one computer to another computer we need some addresses. MAC address also known as Physical address or Hardware address is an identifier assigned to every network devices to uniquely identify itself on a network. MAC address works at the Data Link Layer of the OSI-model. Here, MAC address is used in the sublayer of the Data Link Layer called Media Access Control (MAC).

MAC address is made up of a 48-bits hexadecimal number that is present into every NIC (Network Interface Card) by the manufacturer itself during the time of manufacturing of the devices.

Example of MAC address:
The MAC addresses are formatted in different ways. Such as:

> On Windows \
> 00-00-5E-00-53-AF \
> On Apple & Linux \
> 00:00:5E:00:53:AF \
> On Cisco \
> 0000.5E00.53AF

Here in this MAC address the first 3 byte i.e. 00-00-5E identify the manufacturer of the NIC. \
And the last 3 byte are the unique number that are from the manufracturer that identifies each device on the network.

If a Computer A needs Computer B's MAC address then it sends ARP (Address Resolution Protocol) broadcast on the network to every device with default MAC address FFFF.FFFF.FFFF asking the Computer B to identify itself by asking for its MAC address. And when the Computer B tells its MAC address to Computer A, hence the communication is taken place.

# Finding MAC Address

Command for Unix/Linux

```console
    ifconfig -a
    ip link list
    ip address show
```

Command for Windows OS

```console
    ipconfig/all
```

For MacOS \
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TCP/IP Control Panel

## Note

- IP address can change but the MAC address donot change. They are permanent.
- An IP address tells us where a networking device is located. But a MAC address tells us who the device is.
- IP address also helps to get the MAC address of devices.
- A computer can have one or more MAC addresses. It depends on how many network interfaces it has.
