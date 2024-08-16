---
date: 2022-03-31
type: 🧠
tags:
  - MAC/2/RC
---

**Topics:** [[Computer Network]] - [[IP Address]]

---

`180.55.0.0` will be used for exemplification.

# Borrowing less than one octet

When we borrow less than one [[octet]], the process is mostly the same to [[Class C Subnetting]].

Let's say we borrow 4 bits from the host portion, such that we build `180.55.0.0/20`:

![[Class B Subnetting-1.png]]

That gives us $n = 4$ and $m = 12$, so:
- $2^4 - 2 = 14$ [[Subnetwork|subnetworks]]
- $2^{12} - 2 = 4094$ [[Host|hosts]]

The change factor is $2^4 = 16$. With that, we can build the network table:

| Subnetwork | Subnetwork IP | First Host   | Last Host      | Broadcast      |
| ---------- | ------------- | ------------ | -------------- | -------------- |
| 0          | 180.55.0.0    | 180.55.0.1   | 180.55.15.254  | 180.55.15.255  |
| 1          | 180.55.16.0   | 180.55.16.1  | 180.55.31.254  | 180.55.31.255  |
| 2          | 180.55.32.0   | 180.55.32.1  | 180.55.47.254  | 180.55.47.255  |
| 3          | 180.55.48.0   | 180.55.48.1  | 180.55.63.254  | 180.55.63.255  |
| 4          | 180.55.64.0   | 180.55.64.1  | 180.55.79.254  | 180.55.79.255  |
| 5          | 180.55.80.0   | 180.55.80.1  | 180.55.95.254  | 180.55.95.255  |
| 6          | 180.55.96.0   | 180.55.96.1  | 180.55.111.254 | 180.55.111.255 |
| 7          | 180.55.112.0  | 180.55.112.1 | 180.55.127.254 | 180.55.127.255 |
| 8          | 180.55.128.0  | 180.55.128.1 | 180.55.143.254 | 180.55.143.255 |
| 9          | 180.55.144.0  | 180.55.144.1 | 180.55.159.254 | 180.55.159.255 |
| 10         | 180.55.160.0  | 180.55.160.1 | 180.55.175.254 | 180.55.175.255 |
| 11         | 180.55.176.0  | 180.55.176.1 | 180.55.191.254 | 180.55.191.255 |
| 12         | 180.55.192.0  | 180.55.192.1 | 180.55.207.254 | 180.55.207.255 |
| 13         | 180.55.208.0  | 180.55.208.1 | 180.55.223.254 | 180.55.223.255 |
| 14         | 180.55.224.0  | 180.55.224.1 | 180.55.239.254 | 180.55.239.255 |
| 15         | 180.55.240.0  | 180.55.240.1 | 180.55.255.254 | 180.55.255.255 |

> [!hint]- We change more than one octet
> Notice how, unlike class C subnetting, with class B subnetting we change the values of the two least significant octets, instead of just one. This is why we can have so many hosts per subnetwork.

> [!tip]- An address and a gateway for each subnetwork
> Remember: we use the subnetwork IP to identify a whole subnetwork (the whole group of devices under it). It's good practice to use the first host address for the gateway.

Finally, the [[subnet mask]] for this subnet is `255.255.240.0`.

# Borrowing one octet

The process for borrowing one octet is easy and straightforward.

Since we borrow one octet, we will build `180.55.0.0/24`:

![[Class B Subnetting-2.png]]

That gives us $n = 8$ and $m = 8$, so:
- $2^8 - 2 = 254$ subnetworks
- $2^8 - 2 = 254$ hosts

That gives us a change factor of $1$. We have too many subnetworks to feasibly build a complete table, but we can determine the addresses for a given $n$subnetwork easily enough:

| Subnetwork | Subnetwork IP    | First Host   | Last Host      | Broadcast      |
| ---------- | ---------------- | ------------ | -------------- | -------------- |
| 10         | 180.55.==10==.0  | 180.55.10.1  | 180.55.10.254  | 180.55.10.255  |
| 82         | 180.55.==82==.0  | 180.55.82.1  | 180.55.82.254  | 180.55.82.255  |
| 101        | 180.55.==101==.0 | 180.55.101.1 | 180.55.101.254 | 180.55.01      |
| 128        | 180.55.==128==.0 | 180.55.128.1 | 180.55.128.254 | 180.55.128.255 |
| 200        | 180.55.==200==.0 | 180.55.200.1 | 180.55.200.254 | 180.55.200.255 |

The corresponding subnet mask is `255.255.255.0`.

# Borrowing more than one octet

When we borrow more than one octet, the process is a bit more complicated.

Let's say we borrow 11 bits, such that we build `180.55.0.0/27`:

![[Class B Subnetting-3.png]]

That gives us $n = 11$ and $m = 5$, so:
- $2^{11} - 2 = 2046$ subnetworks
- $2^5 - 2 = 30$ hosts

We have no change factor this time around. Instead, we will follow an algorithm to determine the address.

Notice how, below the table (in red), we have the values corresponding to each bit relative to the octet they're in, while above the table (in orange) we have the values corresponding to each bit relative to the total amount of bits we're borrowing.

To get the address for a given $n$ subnetwork, we take the values from below such that they sum $n$. Then, for each octet, we take the corresponding bit values and add them. The result will be the value that will go to the IP address for that specific octet.

For example, for the 10th subnetwork, we take the values $2^3 + 2^1 = 8 + 2 = 10$. The corresponding bit values relative to the octets are $1$ (for the second octet) and $64$ (for the first octet). Thus, we get the address `180.55.1.64`.

We have way too many subnetworks to feasibly build a complete table, but we can determine the addresses for a few subnetworks:

| Subnet | Subnet IP      | First Host     | Last Host      | Broadcast     |
| ------ | -------------- | -------------- | -------------- | ------------- |
| 10     | 180.55.1.64    | 180.55.1.65    | 180.55.1.94    | 180.55.1.95   |
| 11     | 180.55.1.96    | 180.55.1.97    | 180.55.1.116   | 180.55.117    |
| 20     | 180.55.2.128   | 180.55.2.129   | 180.55.2.158   | 180.55.2.159  |
| 21     | 180.55.2.160   | 180.55.2.161   | 180.55.2.180   | 180.55.2.181  |
| 128    | 180.55.16.0    | 180.55.16.1    | 180.55.16.30   | 180.55.16.31  |
| 260    | 180.55.32.128  | 180.55.32.129  | 180.59.32.158  | 180.59.32.159 |
| 1000   | 180.55.125.0   | 180.55.125.1   | 180.55.125.30  | 180.55.125.31 |
| 2046   | 180.55.255.224 | 180.55.255.225 | 180.55.255.254 | 180.55.255.255              |

The corresponding subnet mask is `255.255.255.224`.
