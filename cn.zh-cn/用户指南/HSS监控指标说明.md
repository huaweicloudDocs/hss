# HSS监控指标说明<a name="hss_01_0527"></a>

## 功能说明<a name="section1563963116197"></a>

本节定义了主机安全服务上报云监控服务的监控指标的命名空间，监控指标列表和维度定义，用户可以通过云监控服务提供管理控制台或API接口来检索主机安全服务产生的监控指标和告警信息。

## 命名空间<a name="section20825105342312"></a>

SYS.HSS

## 监控指标<a name="section86155218720"></a>

**表 1**  主机安全服务支持的监控指标

<a name="table596465321015"></a>
<table><thead align="left"><tr id="row19964253181016"><th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.1"><p id="p696412530101"><a name="p696412530101"></a><a name="p696412530101"></a>指标ID</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.2"><p id="p9964195310106"><a name="p9964195310106"></a><a name="p9964195310106"></a>指标名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.3"><p id="p5965353101011"><a name="p5965353101011"></a><a name="p5965353101011"></a>指标含义</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.4"><p id="p169658538108"><a name="p169658538108"></a><a name="p169658538108"></a>取值范围</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.5"><p id="p19965195316105"><a name="p19965195316105"></a><a name="p19965195316105"></a>测量对象</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.6"><p id="p2965553121017"><a name="p2965553121017"></a><a name="p2965553121017"></a>监控周期（原始指标）</p>
</th>
</tr>
</thead>
<tbody><tr id="row149651538108"><td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.1 "><p id="p19097192119"><a name="p19097192119"></a><a name="p19097192119"></a>host_num</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.2 "><p id="p109094191115"><a name="p109094191115"></a><a name="p109094191115"></a>服务器总数</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.3 "><p id="p1490951912115"><a name="p1490951912115"></a><a name="p1490951912115"></a>该指标用于统计服务器总数</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.4 "><p id="p9965115318108"><a name="p9965115318108"></a><a name="p9965115318108"></a>≥0个</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.5 "><p id="p13965753171011"><a name="p13965753171011"></a><a name="p13965753171011"></a>服务器</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.6 "><p id="p20965125320103"><a name="p20965125320103"></a><a name="p20965125320103"></a>300秒</p>
</td>
</tr>
<tr id="row19651653171015"><td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.1 "><p id="p1390910198110"><a name="p1390910198110"></a><a name="p1390910198110"></a>unprotected_host_num</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.2 "><p id="p390951921117"><a name="p390951921117"></a><a name="p390951921117"></a>未开启防护服务器数量</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.3 "><p id="p1890951911115"><a name="p1890951911115"></a><a name="p1890951911115"></a>该指标用于统计未开启防护的服务器数量</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.4 "><p id="p8431109112216"><a name="p8431109112216"></a><a name="p8431109112216"></a>≥0个</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.5 "><p id="p19965125311105"><a name="p19965125311105"></a><a name="p19965125311105"></a>服务器</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.6 "><p id="p7965135310102"><a name="p7965135310102"></a><a name="p7965135310102"></a>300秒</p>
</td>
</tr>
<tr id="row1596515536103"><td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.1 "><p id="p13910219181120"><a name="p13910219181120"></a><a name="p13910219181120"></a>risky_host_num</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.2 "><p id="p091081910113"><a name="p091081910113"></a><a name="p091081910113"></a>有风险服务器数量</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.3 "><p id="p7910819201115"><a name="p7910819201115"></a><a name="p7910819201115"></a>该指标用于统计经检测判定存在风险的服务器的数量</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.4 "><p id="p9363107229"><a name="p9363107229"></a><a name="p9363107229"></a>≥0个</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.5 "><p id="p16965353131015"><a name="p16965353131015"></a><a name="p16965353131015"></a>服务器</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.6 "><p id="p129651353201014"><a name="p129651353201014"></a><a name="p129651353201014"></a>300秒</p>
</td>
</tr>
<tr id="row496545331012"><td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.1 "><p id="p9910111917112"><a name="p9910111917112"></a><a name="p9910111917112"></a>uninstalled_or_offline_agent_num</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.2 "><p id="p1291031913118"><a name="p1291031913118"></a><a name="p1291031913118"></a>未安装/已离线agent数量</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.3 "><p id="p12910191919118"><a name="p12910191919118"></a><a name="p12910191919118"></a>该指标用于统计未安装agent或者状态为离线的agent的数量</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.4 "><p id="p146151910122220"><a name="p146151910122220"></a><a name="p146151910122220"></a>≥0个</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.5 "><p id="p1396616538106"><a name="p1396616538106"></a><a name="p1396616538106"></a>服务器</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.6 "><p id="p59668531102"><a name="p59668531102"></a><a name="p59668531102"></a>300秒</p>
</td>
</tr>
</tbody>
</table>

## 维度<a name="section16974201271520"></a>

**表 2**  维度列表

<a name="table1235835819219"></a>
<table><thead align="left"><tr id="row83594584215"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p17359185813211"><a name="p17359185813211"></a><a name="p17359185813211"></a>key</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p9359185882118"><a name="p9359185882118"></a><a name="p9359185882118"></a>Value</p>
</th>
</tr>
</thead>
<tbody><tr id="row183591758132117"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1135965892119"><a name="p1135965892119"></a><a name="p1135965892119"></a>hss_enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p13591558122117"><a name="p13591558122117"></a><a name="p13591558122117"></a>企业项目，取值为企业项目ID。</p>
</td>
</tr>
</tbody>
</table>

