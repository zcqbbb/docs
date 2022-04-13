## 功能描述
- 通用告警屏蔽
	- 设备屏蔽
	- 监控项的屏蔽
	- 标签屏蔽
- ZABBIX告警屏蔽

## 注意点
- 通用告警屏蔽
   - 设备与监控项生效原则
   ```
   1. 不选择任何告警规则，则屏蔽该服务器的所有告警规则；
   2. 规则必须归属于已选中的设备；
   ```
   - 标签屏蔽
   ```
   1. 可用标签来源于监控规则；（可以使用执行表达式查看可用标签）；
   2. 为避免贪婪屏蔽，必须制定规则ID；
   3. 标签之间仅仅支持and逻辑运算；
   4. 标签与值对应关系仅仅支持等于；
   5. 与设备以及监控项关系属于平行关系(并集)
   ```
- ZABBIX告警屏蔽
  - 仅仅支持线上ZABBIX屏蔽

## 操作步骤
### 通用告警屏蔽
1. 进入【告警】-【告警屏蔽】-【通用告警屏蔽】，点击“新增”

![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612346151107.png)

![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612346272798.png)

![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612346364665.png)

2. 点击“管理”


![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612346455755.png)


2. 添加设备屏蔽


![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612346584253.png)


![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612346609502.png)


![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612346626983.png)

==注意：交换机以及主机组的屏蔽操作方式与服务器类似==

3. 新增或者变更规则屏蔽


![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612346728329.png)


![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612346795810.png)

==注意：支持规则支持搜索以及多选；==

4. 标签屏蔽

![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612346895629.png)


![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612348711511.png)

- 标签获取方式
  - 基于已经存在告警事件，可以在事件详情中获取事件id以及具体规则，进而获取可用标签

![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612348497171.png)

![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612348469505.png)

  -【告警模板】-【告警规则】-【监控项】可以查看规则，进而获取可用标签

### ZABBIX告警屏蔽
进入【告警】-【告警屏蔽】-【ZABBIX告警屏蔽】，点击“新增”

![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612350116453.png)

![上传成功！](https://ceph-dev-pub.dz11.com/fed-doc/1612350099071.png)