# IP Address

In real life scenario we need address to go certain location. Likewise, Internet Protocol Address also known as Logical Address is used to locate a device on the network. An IP address is like a mailing address of a house.

# How IP addresses function

- Every device should be assigned with an unique IP address. On a network IP Address is either assigned manually by the Network Engineer to devices or it can be auto distributed by a central DHCP server.

- IP address is assigned to devices with certain range available.

- Communication happens using the device IP address and MAC address.

- IP address can be dynamic if not static. i.e. IP address can change.

- Every network will provide a new IP address to the device.

# Classes of IP address

- Class A
- Class B
- Class C
- Class D
- Class E

> Class A, B and C are used in networking \
> Class D is used for Multicast \
> Class E is reserved for Research

IPv4 is a 32-bit address which is divide into 4 octets.

| 1st    | 2nd     | 3rd     | 4th     |
| ------ | ------- | ------- | ------- |
| \_\_\_ | .\_\_\_ | .\_\_\_ | .\_\_\_ |

Each has a length of 8-bits. \
Value in the First Octet determines the Class of IP. \
Values that can be given within an Octet are:

- 1st Octet: 1 to 223
- 2nd, 3rd, 4th: 0 to 255

Every Class of IP has two parts.

- Network ID: Devices that belong to same network will have the same Network ID.
- Host ID: Devices in the network will have an unique Host ID.

| Class | First octet range | Network ID octets         | Host ID octets        | No. of Hosts |
| ----- | ----------------- | ------------------------- | --------------------- | ------------ |
| A     | 1 - 126           | 1st Octet only            | 2nd, 3rd & 4th Octets | 16,777,214   |
| B     | 127 - 191         | 1st & 2nd Octet only      | 3rd & 4th Octets      | 65,534       |
| C     | 192 - 223         | 1st, 2nd & 3rd Octet only | 4th Octets            | 254          |
| D     | 224 - 239         | N/A                       | N/A                   | N/A          |
| E     | 240               | N/A                       | N/A                   | N/A          |
