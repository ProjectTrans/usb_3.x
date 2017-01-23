---
layout: single
title: USB 3.1 规范
date: 2017-1-23 8:41:00
category: USB
---


# 通用串行总线 3.1 规范

惠普
因特尔
微软
瑞萨
意法-爱立信
德州仪器

1.0修订版
2013年7月26日

## 版本历史

| 修订版本 | 	说明 | 签发日期 |
| -------|
| 1.0 | USB 3.0 初始版本 | 2008.11.12 |
| | 合并勘误表和工程变更通知 | 2011.6.6 |
| 1.0 | USB 3.1 初始版本 | 2013.7.26 |
| | |

**知识产权声明**

本协议只是提供给您原始文件，不对以下描述情况做任何担保，包括可销售性，是否侵权，适用于其他任何特殊目的。本规范作者对以下情形免责，包括本规范中应用的，使用的或实现的知识产权，本规范不提供您任何直接或间接的知识产权许可。


请	发送您的意见到 techsup@usb.org.

请到USB-IF的网站 http://www.usb.org 查阅行业资讯。

所有产品名称都是相应拥有者已注册的商标。

Copyright © 2007-2013, Hewlett-Packard Company, Intel Corporation, Microsoft Corporation, Renesas Corporation, STEricsson,
and Texas Instruments

所有权利保留

-------------------
由于本人对法律方面翻译确实够烂，现提供原本的知识产权声明，如有懂法律方面的朋友，欢迎帮助修正:

> **INTELLECTUAL PROPERTY DISCLAIMER**
THIS SPECIFICATION IS PROVIDED TO YOU “AS IS” WITH NO WARRANTIES WHATSOEVER, INCLUDING ANY
WARRANTY OF MERCHANTABILITY, NON-INFRINGEMENT, OR FITNESS FOR ANY PARTICULAR PURPOSE. THE
AUTHORS OF THIS SPECIFICATION DISCLAIM ALL LIABILITY, INCLUDING LIABILITY FOR INFRINGEMENT OF ANY
PROPRIETARY RIGHTS, RELATING TO USE OR IMPLEMENTATION OF INFORMATION IN THIS SPECIFICATION. THE
PROVISION OF THIS SPECIFICATION TO YOU DOES NOT PROVIDE YOU WITH ANY LICENSE, EXPRESS OR
IMPLIED, BY ESTOPPEL OR OTHERWISE, TO ANY INTELLECTUAL PROPERTY RIGHTS.

## 鸣谢 - 致技术贡献者

**献词**

致Brad Hosler，他发明的通用串行总线接口，作为最成功的技术创新之一，在个人电脑领域产生了深远的影响。

本规范的作者把所有参加USB 3.0总线规范技术工作组的人员按照以下清单列出。我们同时也感谢其他的业内人士，他们给我们提供的大量的反馈意见，对本规范的开发工作做出了巨大贡献。

**发起公司人员**

Alan Berkema，Hewlett-Packard Company
Walter Fry，  Hewlett-Packard Company
Anthony Hudson， Hewlett-Packard Company
David Roderick， Hewlett-Packard Company
Kok Hong Chan， Intel Corporation
Huimin Chen， Intel Corporation
Bob Dunstan， Intel Corporation
Dan Froelich， Intel Corporation
Howard Heck， Intel Corporation
Brad Hosler， Intel Corporation
John Howard， Intel Corporation
Rahman Ismail， Intel Corporation
John Keys,， Intel Corporation
Yun Ling， Intel Corporation
Andy Martwick， Intel Corporation
Steve McGowan， Intel Corporation
Ramin Neshati，Intel Corporation
Duane Quiet， Intel Corporation
Jeff Ravencraft， Intel Corporation
Brad Saunders， Intel Corporation
Joe Schaefer， Intel Corporation
Sarah Sharp， Intel Corporation
Micah Sheller， Intel Corporation
Gary Solomon， Intel Corporation
Karthi Vadivelu， Intel Corporation
Clint Walker， Intel Corporation
Jim Walsh， Intel Corporation
Randy Aull， Microsoft Corporation
Fred Bhesania， Microsoft Corporation
Martin Borve， Microsoft Corporation
Jim Bovee， Microsoft Corporation
Stephen Cooper， Microsoft Corporation
Lars Giusti， Microsoft Corporation
Robbie Harris， Microsoft Corporation
Allen Marshall， Microsoft Corporation
Kiran Muthabatulla， Microsoft Corporation
Tomas Perez-Rodriguez， Microsoft Corporation
Mukund Sankaranarayan， Microsoft Corporation
Nathan Sherman， Microsoft Corporation
Glen Slick， Microsoft Corporation
David Wooten， Microsoft Corporation
Rob Young， Microsoft Corporation
Nobuo Furuya， NEC Corporation
Hiroshi Kariya， NEC Corporation
Masami Katagiri， NEC Corporation
Yuichi Mizoguchi， NEC Corporation
Kats Nakazawa， NEC Corporation
Nobuyuki Mizukoshi， NEC Corporation
Yutaka Noguchi， NEC Corporation
Hajime Nozaki， NEC Corporation
Kenji Oguma， NEC Corporation
Satoshi Ohtani， NEC Corporation
Takanori Saeki， NEC Corporation
Eiji Sakai， NEC Corporation
Hiro Sakamoto， NEC Corporation
Hajime Sakuma， NEC Corporation
Makoto Sato， NEC Corporation
Hock Seow， NEC Corporation
"Peter" Chu Tin Teng， NEC Corporation
Yoshiyuki Tomoda， NEC Corporation
Satomi Yamauchi， NEC Corporation
Yoshiyuki Yamada， NEC Corporation
Susumu Yasuda， NEC Corporation
Alan Chang， ST-NXP Wireless
Wing Yan Chung， ST-NXP Wireless
Socol Constantin， ST-NXP Wireless
Knud Holtvoeth， NXP Semiconductors, B.V.
Linus Kerk， ST-NXP Wireless
Martin Klein， NXP Semiconductors, B.V.
Geert Knapen， NXP Semiconductors, B.V.
Chee Ee Lee，ST-NXP Wireless
Christian Paquet， NXP Semiconductors, B.V.
Veerappan Rajaram， ST-NXP Wireless
Shaun Reemeyer， ST-NXP Wireless
Dave Sroka， ST-NXP Wireless
Chee-Yen TEE， ST-NXP Wireless
Jerome Tjia， ST-NXP Wireless
Bart Vertenten， NXP Semiconductors, B.V.
Hock Meng Yeo， ST-NXP Wireless
Olivier Alavoine， Texas Instruments.
David Arciniega， Texas Instruments
Richard Baker， Texas Instruments
Sujoy Chakravarty， Texas Instruments
T. Y. Chan， Texas Instruments
Romit Dasgupta， Texas Instruments.
Alex Davidson， Texas Instruments
Eric Desmarchelier， Texas Instruments
Christophe Gautier， Texas Instruments
Dan Harmon， Texas Instruments
Will Harris， Texas Instruments
Richard Hubbard， Texas Instruments
Ivo Huber， Texas Instruments
Scott Kim， Texas Instruments
Grant Ley， Texas Instruments
Karl Muth， Texas Instruments
Lee Myers， Texas Instruments
Julie Nirchi， Texas Instruments
Wes Ray ，Texas Instruments
Matthew Rowley， Texas Instruments
Bill Sherry， Texas Instruments
Mitsuru Shimada， Texas Instruments
James Skidmore， Texas Instruments
Yoram Solomon， Texas Instruments.
Sue Vining， Texas Instruments
Jin-sheng Wang， Texas Instruments
Roy Wojciechowski， Texas Instruments

**贡献公司人员**

Glen Chandler， Acon
John Chen， Acon
Roger Hou， Acon
Charles Wang， Acon
Norman Wu， Acon
Steven Yang， Acon
George Yee， Acon
George Olear， Contech Research
Sophia Liu， Electronics Testing Center, Taiwan (ETC)
William Northey， FCI
Tom Sultzer， FCI
Garry Biddle， Foxconn
Kuan-Yu Chen， Foxconn
Jason Chou， Foxconn
Gustavo Duenas， Foxconn
Bob Hall， Foxconn
Jiayong He， Foxconn
Jim Koser， Foxconn
Joe Ortega， Foxconn
Ash Raheja， Foxconn
James Sabo， Foxconn
Pei Tsao， Foxconn
Kevin Walker， Foxconn
Tsuneki Watanabe， Foxconn
Chong Yi， Foxconn
Taro Hishinuma， Hirose Electric
Kaz Ichikawa， Hirose Electric
Ryozo Koyama， Hirose Electric
Karl Kwiat， Hirose Electric
Tadashi Sakaizawa， Hirose Electric
Shinya Tono， Hirose Electric
Eiji Wakatsuki， Hirose Electric
Takashi Ehara， Japan Aviation Electronics Industry Ltd. (JAE)
Ron Muir， Japan Aviation Electronics Industry Ltd. (JAE)
Kazuhiro Saito， Japan Aviation Electronics Industry Ltd. (JAE)
Hitoshi Kawamura， Mitsumi
Takashi Kawasaki， Mitsumi
Atsushi Nishio， Mitsumi
Yasuhiko Shinohara， Mitsumi
Tom Lu， Molex Inc.
Edmund Poh， Molex Inc.
Scott Sommers， Molex Inc.
Jason Squire， Molex Inc.
Dat Ba Nguyen， NTS/National Technical System
Jan Fahllund， Nokia
Richard Petrie， Nokia
Panu Ylihaavisto， Nokia
Martin Furuhjelm， Seagate Technology LLC
Julian Gorfajn， Seagate Technology LLC
Marc Hildebrant， Seagate Technology LLC
Tony Priborsky， Seagate Technology LLC
Harold To， Seagate Technology LLC
Robert Lefferts， Synopsys, Inc.
Saleem Mohammad， Synopsys, Inc.
Matthew Myers， Synopsys, Inc.
Daniel Weinlader， Synopsys, Inc.
Mike Engbretson， Tektronix, Inc.
Thomas Grzysiewicz， Tyco Electronics
Masaaki Iwasaki， Tyco Electronics
Kazukiyo Osada， Tyco Electronics
Hiroshi Shirai，Tyco Electronics
Scott Shuey， Tyco Electronics
Masaru Ueno， Tyco Electronics
Egbert Stellinga， Tyco Electronics Corp., a TE Connectivity Ltd. company
Noah Zhang， Tyco Electronics Corp., a TE Connectivity Ltd. company
Marvin DeForest， Western Digital Technologies, Inc.
Larry McMillan， Western Digital Technologies, Inc.
Cristian Roman Del Nido， Western Digital Technologies, Inc.
Curtis Stevens， Western Digital Technologies, Inc.

[TOC]

## 1 简介

### 1.1 背景

人们需要有一种用户友好的将外设插入到PC的即插即用方法，因此USB应运而生。USB不仅仅能够把外设插入到PC上，打印机可以直接通过USB接口连接照相机，移动设备可以通过USB接口连接鼠标和键盘。USB技术在汽车，电视，和机顶盒等都很常见。作为一种协议，也可以在很多非传统的应用，如工业自动化领域采用USB协议。并且，在移动设备上，电源的充电方案采用USB技术已经在国际同行内得到了广泛的认可。

最开始，USB只提供两种供外设使用的速度(12 Mbps和1.5Mbps)。随着PC的性能变得越来越强大，具备了处理更大规模数据的能力，用户需要跟PC交互更多的数据。这导致在2000年，USB 2.0规范应运而生，它提供了高达480Mbps的第三种传输速度。到2006年，业内出现了两件事情：HDDs 的	传输速度超过了100MB/s, 超出了USB 2.0的最高32MB/s的带宽，同时，数字内容用户的数量也达到了空前的规模。因此，USB 社区为了响应这个问题，提出了传输速率高达450MB/s的USB 3.0，并且可以向后兼容 USB 2.0. 

现在更快更大的存储，高清视频，USB作为系统的外部扩展的需求的发展，带宽更宽已经成为一个持续发展的趋势。在这种背景下，USB 3.1 通过把高速USB的时钟频率提高到10Gbps，加强数据编码效率后， 把USB的带宽提升到1GB/s.

### 1.2 规范目的

本文档定义了最新的USB工业标准，USB 3.1. 本规范描述了协议定义，传输类型，总线管理，设计和构建兼容本规范的系统和外设的编程接口。USB 3.1主要是对USB 3.0的增强，使之能够提供双倍的带宽，服务于像SSD和高清显示器这样的设备。

本规范设计的增强高速集合了应用于USB 3.0和USB 3.1的特性或需求。另外，那些特定的与USB 3.0定义不同的差异，被称为SSP(SuperSpeedPlus). 通常，SS使指5Gbps的操作，SSP指的是10Gbps的操作。

USB 3.1的目标仍然是提供一个开放的架构，使来自不同厂家的设备能够互通，维护和利用现存的USB基础架构(设备驱动，软件接口等)。本规范作为一个面向PC架构，包括笔记本电脑，商用电脑，和家庭环境，简单的设备于设备通信的增强。本规范的目的是给系统OEMs, 外设开发者足够的空间来丰富产品和市场，避免产品间由于封闭的接口而造成的不兼容问题。

### 1.3 文档范围

本规范主要面向外设开发者和平台/转接器开发者，但是也为平台操作系统，BIOS，设备驱动，IHVs/ISVs转接器，和系统OEMs. 本规范可以用来开发新产品和对应的软件。

使用本规范的设备开发者需要先了解USB 2.0 规范。尤其是，USB 3.1 设备必须实现USB 2.0规范定义的设备框架命令和描述符。工作在10Gbps速度的设备必须实现本规范版本定义的SSP - 超高速+。

### 1.4 USB 产品兼容

USB 3.1 规范的使用者，必须签署 USB 3.0 使用者协议，该协议给他们从发起者和开放其跟USB3.1规范兼容的应用于其产品中的知识产权的其他使用者处获取访问一个合理，非歧视性(RANDZ) 许可。使用者可以使用USB-IF提供的测试工具测试其产品的兼容性。通过本规范兼容性测试的产品，允许使用在标志许可中定义的USB-IF标志。

从USB 3.1 规范开始，产品兼容性需求禁止使用非认证的线缆和连接器。在有许可证的情况下，才可以在产品上，文档中，或包装上使用任何注册的图标或标志，而这个许可证只有产品通过相应的认证才能获得。

### 1.5 文档组织结构

第1章到第4章是总览部分，第5章到第11章包含了详细的技术描述。

读者应该联系操作系统供应商绑定操作系统到USB 3.1.

### 1.6 设计目标

USB 3.0 是USB的一个革命性的进程。USB 3.1 是 USB 3.0的进化版本，以增加USB的带宽。但是目的还是一样: 终端用户可以把他们看做是USB 2.0 和 USB 3.1，只是更快而已。为了达到这个目标而做的一些关键设计列举如下: 

* 保留智能主机和简单外设的USB模型。
* 兼容现存的USB基础设施。如今有巨量的USB设备在运行。他们流行的很大一部分原因是因为现存的稳定的软件接口，简单的设备驱动开发，和大量的通用接口标准设备族驱动(HID, 大容量存储，音频等)。增强的超高速USB设备完整的保留了这些软件基础设施，以支持开发者能够继续使用相同的接口，兼容他们已完成的开发工作。
* 极大的提高了功耗管理。提供了一系列丰富的管理机制以允许设备让总线进入低功耗状态，降低了传送数据的功耗和待机功耗。
* 易用性是所有USB变种已知保持的关键设计目标。
* 保持投资。大量的PC只支持USB 2.0. 大量的USB 2.0 设备在使用。向后兼容的设计允许加强的超高速设备可以使用Type-A的连接器与USB 2.0的高速设备连接。
* 允许主机控制器在不改变操作系统的前提下就能利用USB 3.1的速度和特性。

### 1.7 关联文档

Universal Serial Bus Specification, Revision 2.0

USB On-the-Go Supplement to the USB 2.0 Specification, Revision 1.3

USB On-the-Go and Embedded Host Supplement to the USB 3.0 Specification, Revision 1.0

Universal Serial Bus Micro-USB Cables and Connectors Specification, Revision 1.01

EIA-364-1000.01: Environmental Test Methodology for Assessing the Performance of Electrical

Connectors and Sockets Used in Business Office Applications

USB 3.0 Connectors and Cable Assemblies Compliance Document

USB SuperSpeed Electrical Test Methodology white paper

USB 3.0 Jitter Budgeting white paper

INCITS TR-35-2004, INCITS Technical Report for Information Technology – Fibre Channel – Methodologies for Jitter and Signal Quality Specification (FC-MJSQ)

Universal Serial Bus 3.0 Specification (including errata and ECNs through May 1, 2011)

Universal Serial Bus Power Delivery Specification, Revision 1.0 Including Errata through 31-October-2012

## 2 术语和缩略语

本章列举，定义了本规范中使用的术语和缩略语。注意，本章没有列举的术语或缩略语，请参考一般意义或查字典。

| 术语/缩略语 | 说明 |
| ----
| ACK | 握手包，肯定确认 |
| ACK Tx Header Sequence Number | 期望的被认可的连接控制字头中的序列号 |
| active device | 上电的并且没有挂起的设备 |
| asynchronous data | 没有严格的时间间隔的数据包 |
| attached | 例如U盘attached在PC上 |
| AWG# | 电线横截面测量，美国线规标准定义 |


> Written with [StackEdit](https://stackedit.io/)