---
description: Understanding how the VM connects
---

# Networking

I need to know how network connectivity works before I can continue. I can check if I have network connectivity by doing updates. This will take a few minutes over a good internet connection.

```
sudo apt-get update
sudo apt-get upgrade -y
```

When that is finished, lets check networking on the host. At the command prompt, I type&#x20;

**ipconfig /all**

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

I have two network adapters. The first Ethernet adapter is the one connecting to Azure and the rest of the world. The second adapter (WSL) is a virtual adapter which Windows created for a network inside the host computer. The IPv4 address space is 172.26.0.0/20 and my host computer is .1

Let us check networking on the VM. At the command prompt, I type&#x20;

**ip addr**&#x20;

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

My VM has an address 172.26.4.199/20.&#x20;

A logical diagram of the network would look something like this.

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

Note that the host computer can access this network as if it is an ordinary node. But it also provides a NAT router service to allow the VM to connect to outside world. A NAT router is a bit like your home Internet connection, it translates IPv4 addresses on an internal network, to addresses which can be used externally.
