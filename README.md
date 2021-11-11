### 翻译zabbix 文档

~~~ 
1、SNMP没有采集到数据 - No SNMP data collection
2、Ping 丢包率过高 - High ICMP ping loss
3、Ping响应时间过长 -  High ICMP ping response time
4、系统名称已经被改变(新名称为：{ITEM.VALUE})- System name has changed (new name: {ITEM.VALUE})
5、Ping不可达  - Unavailable by ICMP ping
6、{HOST.NAME} 已经重新启动,更新时间小于十分钟-{HOST.NAME} has been restarted (uptime < 10m)

7、接口{#IFNAME}({#IFALIAS}): 以太网的速度比以前低了
Interface {#IFNAME}({#IFALIAS}): Ethernet has changed to lower speed than it was before
8、接口{#IFNAME}({#IFALIAS}): 带宽利用率大于{$IF.UTIL.MAX:"{#IFNAME}"}%
Interface {#IFNAME}({#IFALIAS}): High bandwidth usage ( > {$IF.UTIL.MAX:"{#IFNAME}"}% )
9、接口{#IFNAME}({#IFALIAS}): 已断开连接
Interface {#IFNAME}({#IFALIAS}): Link down
10、接口{#IFNAME}({#IFALIAS}): 错误率较高，持续5分钟大于{$IF.ERRORS.WARN:"{#IFNAME}"}
Interface {#IFNAME}({#IFALIAS}): High error rate ( > {$IF.ERRORS.WARN:"{#IFNAME}"} for 5m)
11、接口{#IFNAME}({#IFALIAS}): 在半双工模式下
Interface {#IFNAME}({#IFALIAS}): In half-duplex mode

12、CPU使用率过高,持续5分钟超过{$CPU.UTIL.CRIT}%
High CPU utilization (over {$CPU.UTIL.CRIT}% for 5m)
13、内存使用率过高,持续5分钟超过{$MEMORY.UTIL.MAX}%
High memory utilization ( >{$MEMORY.UTIL.MAX}% for 5m)
14、在{ITEM.VALUE2}中，可用内存小于{$MEMORY.AVAILABLE.MIN}
Lack of available memory ( < {$MEMORY.AVAILABLE.MIN} of {ITEM.VALUE2})
15、交换空间使用率过高，可用剩余{$SWAP.PFREE.MIN.WARN}%
High swap space usage ( less than {$SWAP.PFREE.MIN.WARN}% free)

16、{#FSNAME}: 磁盘空间剩余极少,使用率大于{$VFS.FS.PUSED.MAX.CRIT:"{#FSNAME}"}%
{#FSNAME}: Disk space is critically low (used > {$VFS.FS.PUSED.MAX.CRIT:"{#FSNAME}"}%)
17、{#FSNAME}: 磁盘空间剩余少,使用率大于{$VFS.FS.PUSED.MAX.WARN:"{#FSNAME}"}%
{#FSNAME}: Disk space is low (used > {$VFS.FS.PUSED.MAX.WARN:"{#FSNAME}"}%)

18、平均负载太高，持续5秒钟每个CPU负载超过{$LOAD_AVG_PER_CPU.MAX.WARN}
Load average is too high (per CPU load over {$LOAD_AVG_PER_CPU.MAX.WARN} for 5m)

19、{#FSNAME}: 磁盘空间剩余极低，使用率大于{$VFS.FS.PUSED.MAX.CRIT:"{#FSNAME}"}%
{#FSNAME}: Disk space is critically low (used > {$VFS.FS.PUSED.MAX.CRIT:"{#FSNAME}"}%)

20、{#FSNAME}: 耗尽可用的索引节点,可用节点小于{$VFS.FS.INODE.PFREE.MIN.WARN:"{#FSNAME}"}%
{#FSNAME}: Running out of free inodes (free < {$VFS.FS.INODE.PFREE.MIN.WARN:"{#FSNAME}"}%)
21、{#FSNAME}: 磁盘空间太低,使用率大于{$VFS.FS.PUSED.MAX.WARN:"{#FSNAME}"}%
{#FSNAME}: Disk space is low (used > {$VFS.FS.PUSED.MAX.WARN:"{#FSNAME}"}%)

22、#{#SNMPINDEX}: 风扇状态异常
#{#SNMPINDEX}: Fan is in critical state

23、{#SNMPVALUE}: 温度高于临界值,当前临界值为：{$TEMP_CRIT:""}
{#SNMPVALUE}: Temperature is above critical threshold: >{$TEMP_CRIT:""}
24、{#SNMPVALUE}: 温度太低，小于{$TEMP_CRIT_LOW:""}
{#SNMPVALUE}: Temperature is too low: <{$TEMP_CRIT_LOW:""}
25、{#SNMPVALUE}: 温度高于临界值,当前临界值为：{$TEMP_WARN:""}
{#SNMPVALUE}: Temperature is above warning threshold: >{$TEMP_WARN:""}

~~~