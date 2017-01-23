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


> Written with [StackEdit](https://stackedit.io/).