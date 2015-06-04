---
layout: default
title: 计算机网络：自顶向下方法(第四版)
---

{{ page.title }}
================


## Chapter 1


### 1.1

#### 1.1.1
Hosts(End System) connect each other through communication link and packet switch.
ISPs follow IP protocol.
IETF develop RFC.
IEEE 802 develop Ethernet and WiFi(802.11).
Internet <-> Intranet

#### 1.1.2
API

#### 1.1.3


### 1.2
Hosts: 1. Server, 2. Client.

#### 1.2.1

#### 1.2.2
Access Network: the edge router to connect end system.
Physical Medium Access: DSL, HFC.
Up-link, down-link and bi-direction link transmit
Transmission speed depends on distance, physical link quality, electromagnetic disturb and other factors.
LAN. Edge router chooses path for hosts not in LAN.
Wireless LAN: base stations are within 100 meters.
3G: EVDO, HSDPA

#### 1.2.3
UTP.


### 1.3

#### 1.3.1
Circuit Switch: establish a connected status(circuit). Used in phone not Internet. TDM(1 frame divided to slots, each circuit has one slot), FDM(bandwidth).
Packet Switch: best effort.
Message: combined by several packet.
Packet switch: i.e. router and link-layer switch.
Store-and-forward transmission: get all packet before transmit. Has a delay.
Buffer = queue. A queue delay. May cause packet loss.
Statistical multiplexing.

#### 1.3.2
Router has a forwarding table. It check IP address of packets
[www.traceroute.org](https://www.net.princeton.edu/traceroute.html)

#### 1.3.3
tier-1 ISP: Internet backbone. connect with other tier-1 ISP.
tier-2 ISP: customer of tier-1 ISP, which is provider.
When two ISPs connected, they are peer to each other.
POP: the point where two ISPs connected. Is a group of routers.

