## 概述
English：[readme.md](doc/en/readme.md)

   本工程主要更新Robomaster2019裁判系统串口协议。Robomaster2019裁判系统通过电源模块的user串口对外输出数据，用于比赛信息的数据获取。
   ### 文档

   中文版：
   
   <a href="doc/cn/裁判系统串口协议附录 V2.0.pdf" target="_blank">2019 裁判系统串口协议附录 V2.0.pdf</a>

   <a href="doc/cn/2020年裁判系统串口协议附录 V1.0.pdf" target="_blank">2020年裁判系统串口协议附录 V1.0.pdf</a>

   <a href="doc/cn/2020年裁判系统串口协议附录 V1.1.pdf" target="_blank">2020年裁判系统串口协议附录 V1.1.pdf</a>
   
   英文版：
   
   <a href="doc/en/Referee System Serial Port Protocol Appendix V2.0.pdf" target="_blank">2019 Referee System Serial Port Protocol Appendix V2.0.pdf</a>


   <a href="doc/en/2020 Referee System Serial Port Protocol Appendix V1.0.pdf" target="_blank">2020 Referee System Serial Port Protocol Appendix V1.1.pdf</a>
   
   
   <a href="doc/en/2020 Referee System Serial Port Protocol Appendix V1.1.pdf" target="_blank">2020 Referee System Serial Port Protocol Appendix V1.1.pdf</a>

   ### 主要更新点

   2020.5.15

   1.增加飞镖机器人客户端指令数据

   2.交互数据ID说明中增加缺少的雷达站ID

   2020.2.25

   1.2020年首次发布

   2019.7.11

   1.修改比赛机器人存活情况为比赛机器人血量；

   2.修改空中机器人发射时间描述；

   3.修改场地事件，增加小能量机关描述，基地护盾描述；

   4.修改伤害信息描述；

   5.增加裁判警告信息；

   6.增加子弹剩余发射数，仅支持空中机器人与哨兵机器人；

   7.增加客户端自定义图形。
   ### 更新点介绍

   1.双方均可以获取全场机器人血量，可以用于哨兵机器人等机器人上进行自动瞄准的优化，

   2.主要为根据总决赛规则的修改，减少为30s；

   3.主要为根据总决赛规则的修改，加入的小能量机关的bit，故而之后的bit位整体后移了一位，添加了基地护盾的描述

   4.伤害信息类型的修改，添加了超射速，装甲撞击类型

   5.添加了一个新的cmd_id，判罚信息，对于参赛队机器人，可以添加一个自动防御的状态，用于判罚时子弹的躲避。

   6.根据总决赛规则添加了剩余子弹数，因为哨兵机器人和空中机器人均500颗子弹，可以获取到剩余子弹的发射量，用于控制策略的优化

   7.添加了一种新的人机交互形式，参赛队可以使用该命令进行客户端的画图，辅助参赛队操作手体验。以下进行详细介绍


