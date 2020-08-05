# HSS授权项说明<a name="hss_01_0006"></a>

## 支持的授权项<a name="section677212217497"></a>

策略包含系统策略和自定义策略，如果系统策略不满足授权要求，管理员可以创建自定义策略，并通过给用户组授予自定义策略来进行精细的访问控制。策略支持的操作与API相对应，授权项列表说明如下：

-   权限：允许或拒绝某项操作。
-   授权项：自定义策略中支持的Action，在自定义策略中的Action中写入授权项，可以实现授权项对应的权限功能。
-   依赖的授权项：部分Action存在对其他Action的依赖，需要将依赖的Action同时写入授权项，才能实现对应的权限功能。
-   IAM项目\(Project\)/企业项目\(Enterprise Project\)：自定义策略的授权范围，包括IAM项目与企业项目。授权范围如果同时支持IAM项目和企业项目，表示此授权项对应的自定义策略，可以在IAM和企业管理两个服务中给用户组授权并生效。如果仅支持IAM项目，不支持企业项目，表示仅能在IAM中给用户组授权并生效，如果在企业管理中授权，则该自定义策略不生效。关于IAM项目与企业项目的区别，详情请参见：[IAM与企业管理的区别](https://support.huaweicloud.com/iam_faq/iam_01_0101.html)。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >“√”表示支持，“x”表示暂不支持。


企业主机安全服务（HSS）支持的自定义策略授权项如下所示：

[授权列表](#section15113173595712)，包含HSS对应的授权项，如查询主机安全防护列表、云服务器开启或关闭防护、手动检测等。

## 授权列表<a name="section15113173595712"></a>

<a name="table8211143315354"></a>
<table><thead align="left"><tr id="row144381133183517"><th class="cellrowborder" valign="top" width="18.14%" id="mcps1.1.6.1.1"><p id="p1443820332357"><a name="p1443820332357"></a><a name="p1443820332357"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="22.770000000000003%" id="mcps1.1.6.1.2"><p id="p19438733133512"><a name="p19438733133512"></a><a name="p19438733133512"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="19.689999999999998%" id="mcps1.1.6.1.3"><p id="p10212221012"><a name="p10212221012"></a><a name="p10212221012"></a>依赖的授权项</p>
</th>
<th class="cellrowborder" valign="top" width="16.220000000000002%" id="mcps1.1.6.1.4"><p id="p1834910910535"><a name="p1834910910535"></a><a name="p1834910910535"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="23.18%" id="mcps1.1.6.1.5"><p id="p95277361933"><a name="p95277361933"></a><a name="p95277361933"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row84382333355"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p94384333351"><a name="p94384333351"></a><a name="p94384333351"></a>查询主机安全防护列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1543833320356"><a name="p1543833320356"></a><a name="p1543833320356"></a>hss:hosts:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p114779181502"><a name="p114779181502"></a><a name="p114779181502"></a>vpc:ports:get</p>
<p id="p378516477505"><a name="p378516477505"></a><a name="p378516477505"></a>vpc:publicIps:list</p>
<p id="p1943858115019"><a name="p1943858115019"></a><a name="p1943858115019"></a>ecs:cloudServers:list</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1187205916317"><a name="p1187205916317"></a><a name="p1187205916317"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p13581103214526"><a name="p13581103214526"></a><a name="p13581103214526"></a>√</p>
</td>
</tr>
<tr id="row3438233163513"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p143893353510"><a name="p143893353510"></a><a name="p143893353510"></a>云服务器开启或关闭防护</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1843833313350"><a name="p1843833313350"></a><a name="p1843833313350"></a>hss:hosts:switchVersion</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1213142504"><a name="p1213142504"></a><a name="p1213142504"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p614311203416"><a name="p614311203416"></a><a name="p614311203416"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1361223217523"><a name="p1361223217523"></a><a name="p1361223217523"></a>√</p>
</td>
</tr>
<tr id="row843813332359"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p243853313517"><a name="p243853313517"></a><a name="p243853313517"></a>手动检测</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p5438103313515"><a name="p5438103313515"></a><a name="p5438103313515"></a>hss:hosts:manualDetect</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p195581455926"><a name="p195581455926"></a><a name="p195581455926"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1519414204417"><a name="p1519414204417"></a><a name="p1519414204417"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p0651153218529"><a name="p0651153218529"></a><a name="p0651153218529"></a>√</p>
</td>
</tr>
<tr id="row15438333173516"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p184381733133513"><a name="p184381733133513"></a><a name="p184381733133513"></a>手动检测返回检测状态</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p5438203317353"><a name="p5438203317353"></a><a name="p5438203317353"></a>hss:manualDetectStatus:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1760211552219"><a name="p1760211552219"></a><a name="p1760211552219"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p524952018412"><a name="p524952018412"></a><a name="p524952018412"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p106735328528"><a name="p106735328528"></a><a name="p106735328528"></a>√</p>
</td>
</tr>
<tr id="row2438833113519"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p14439183316351"><a name="p14439183316351"></a><a name="p14439183316351"></a>查询弱口令检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1343918338356"><a name="p1343918338356"></a><a name="p1343918338356"></a>hss:weakPwds:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p96532551822"><a name="p96532551822"></a><a name="p96532551822"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p527110207410"><a name="p527110207410"></a><a name="p527110207410"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p76891532175217"><a name="p76891532175217"></a><a name="p76891532175217"></a>√</p>
</td>
</tr>
<tr id="row44391033103510"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p9439153316352"><a name="p9439153316352"></a><a name="p9439153316352"></a>查询账户破解防护报告</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p5439123318357"><a name="p5439123318357"></a><a name="p5439123318357"></a>hss:accountCracks:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p16758551024"><a name="p16758551024"></a><a name="p16758551024"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p2291152012411"><a name="p2291152012411"></a><a name="p2291152012411"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p20708163265212"><a name="p20708163265212"></a><a name="p20708163265212"></a>√</p>
</td>
</tr>
<tr id="row2439203317357"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p154397332352"><a name="p154397332352"></a><a name="p154397332352"></a>账户破解防护解除拦截IP</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p243953312353"><a name="p243953312353"></a><a name="p243953312353"></a>hss:accountCracks:unblock</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p17700125511219"><a name="p17700125511219"></a><a name="p17700125511219"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p143118201447"><a name="p143118201447"></a><a name="p143118201447"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p7724153217529"><a name="p7724153217529"></a><a name="p7724153217529"></a>√</p>
</td>
</tr>
<tr id="row19439203313511"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p043963383517"><a name="p043963383517"></a><a name="p043963383517"></a>查询恶意程序检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p194391433183510"><a name="p194391433183510"></a><a name="p194391433183510"></a>hss:maliciousPrograms:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p177251555323"><a name="p177251555323"></a><a name="p177251555323"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p163315201747"><a name="p163315201747"></a><a name="p163315201747"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p6741153275219"><a name="p6741153275219"></a><a name="p6741153275219"></a>√</p>
</td>
</tr>
<tr id="row13439733173510"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p10439133311357"><a name="p10439133311357"></a><a name="p10439133311357"></a>查询异地登录检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p24396335354"><a name="p24396335354"></a><a name="p24396335354"></a>hss:abnorLogins:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p177496558214"><a name="p177496558214"></a><a name="p177496558214"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p535110201744"><a name="p535110201744"></a><a name="p535110201744"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p07581332105218"><a name="p07581332105218"></a><a name="p07581332105218"></a>√</p>
</td>
</tr>
<tr id="row843963383520"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p143913303513"><a name="p143913303513"></a><a name="p143913303513"></a>查询关键文件变更报告</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p84391533123518"><a name="p84391533123518"></a><a name="p84391533123518"></a>hss:keyfiles:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p57701655225"><a name="p57701655225"></a><a name="p57701655225"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p113761420649"><a name="p113761420649"></a><a name="p113761420649"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p13772163285215"><a name="p13772163285215"></a><a name="p13772163285215"></a>√</p>
</td>
</tr>
<tr id="row94391333123511"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p174396335354"><a name="p174396335354"></a><a name="p174396335354"></a>查询开放端口信息列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1743920337358"><a name="p1743920337358"></a><a name="p1743920337358"></a>hss:ports:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p197955551326"><a name="p197955551326"></a><a name="p197955551326"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p4396172015419"><a name="p4396172015419"></a><a name="p4396172015419"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p3788332175218"><a name="p3788332175218"></a><a name="p3788332175218"></a>√</p>
</td>
</tr>
<tr id="row1943993316358"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p0439153315356"><a name="p0439153315356"></a><a name="p0439153315356"></a>查询漏洞列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p13439173383512"><a name="p13439173383512"></a><a name="p13439173383512"></a>hss:vuls:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1681711551210"><a name="p1681711551210"></a><a name="p1681711551210"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1042382017417"><a name="p1042382017417"></a><a name="p1042382017417"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p180343216524"><a name="p180343216524"></a><a name="p180343216524"></a>√</p>
</td>
</tr>
<tr id="row144398331352"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1243903317358"><a name="p1243903317358"></a><a name="p1243903317358"></a>批量操作漏洞</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p11439113383518"><a name="p11439113383518"></a><a name="p11439113383518"></a>hss:vuls:operate</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p484115511216"><a name="p484115511216"></a><a name="p484115511216"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p14446204412"><a name="p14446204412"></a><a name="p14446204412"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1281833218521"><a name="p1281833218521"></a><a name="p1281833218521"></a>√</p>
</td>
</tr>
<tr id="row16439113313515"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p043903333518"><a name="p043903333518"></a><a name="p043903333518"></a>查询账号信息列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p6439123373515"><a name="p6439123373515"></a><a name="p6439123373515"></a>hss:accounts:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p108661755828"><a name="p108661755828"></a><a name="p108661755828"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p246319201047"><a name="p246319201047"></a><a name="p246319201047"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1883363212529"><a name="p1883363212529"></a><a name="p1883363212529"></a>√</p>
</td>
</tr>
<tr id="row1843917337353"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1443963333514"><a name="p1443963333514"></a><a name="p1443963333514"></a>查询软件信息列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p243973343517"><a name="p243973343517"></a><a name="p243973343517"></a>hss:softwares:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p58911755223"><a name="p58911755223"></a><a name="p58911755223"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p148314206417"><a name="p148314206417"></a><a name="p148314206417"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p28517324520"><a name="p28517324520"></a><a name="p28517324520"></a>√</p>
</td>
</tr>
<tr id="row3439123393518"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p9439173373512"><a name="p9439173373512"></a><a name="p9439173373512"></a>查询Web路径列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p18439203311356"><a name="p18439203311356"></a><a name="p18439203311356"></a>hss:webdirs:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1491355515213"><a name="p1491355515213"></a><a name="p1491355515213"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p165030205415"><a name="p165030205415"></a><a name="p165030205415"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p178671932175217"><a name="p178671932175217"></a><a name="p178671932175217"></a>√</p>
</td>
</tr>
<tr id="row1843916332353"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p84391233153516"><a name="p84391233153516"></a><a name="p84391233153516"></a>查询进程信息列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p134391033133516"><a name="p134391033133516"></a><a name="p134391033133516"></a>hss:processes:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p169375554213"><a name="p169375554213"></a><a name="p169375554213"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p205211320741"><a name="p205211320741"></a><a name="p205211320741"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p108824326526"><a name="p108824326526"></a><a name="p108824326526"></a>√</p>
</td>
</tr>
<tr id="row44401133203520"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p11440123317357"><a name="p11440123317357"></a><a name="p11440123317357"></a>查询配置检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p11440153333516"><a name="p11440153333516"></a><a name="p11440153333516"></a>hss:configDetects:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1795705516213"><a name="p1795705516213"></a><a name="p1795705516213"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p95464201248"><a name="p95464201248"></a><a name="p95464201248"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p789563255217"><a name="p789563255217"></a><a name="p789563255217"></a>√</p>
</td>
</tr>
<tr id="row84402033143518"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p17440103343516"><a name="p17440103343516"></a><a name="p17440103343516"></a>查询网站后门检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p19440733113516"><a name="p19440733113516"></a><a name="p19440733113516"></a>hss:webshells:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1497816551422"><a name="p1497816551422"></a><a name="p1497816551422"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p7565320747"><a name="p7565320747"></a><a name="p7565320747"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p391213255217"><a name="p391213255217"></a><a name="p391213255217"></a>√</p>
</td>
</tr>
<tr id="row844013323511"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p164408335355"><a name="p164408335355"></a><a name="p164408335355"></a>查询风险账号检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1644083353511"><a name="p1644083353511"></a><a name="p1644083353511"></a>hss:riskyAccounts:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p899914551829"><a name="p899914551829"></a><a name="p899914551829"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1558642016416"><a name="p1558642016416"></a><a name="p1558642016416"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p892716324528"><a name="p892716324528"></a><a name="p892716324528"></a>√</p>
</td>
</tr>
<tr id="row12440633173515"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p14440203317351"><a name="p14440203317351"></a><a name="p14440203317351"></a>云服务器风险统计</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p18440833123517"><a name="p18440833123517"></a><a name="p18440833123517"></a>hss:riskyDashboard:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p11914562026"><a name="p11914562026"></a><a name="p11914562026"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p7607142020412"><a name="p7607142020412"></a><a name="p7607142020412"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p09415327529"><a name="p09415327529"></a><a name="p09415327529"></a>√</p>
</td>
</tr>
<tr id="row744033312355"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1044017332353"><a name="p1044017332353"></a><a name="p1044017332353"></a>查询口令复杂度策略检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p94401033133513"><a name="p94401033133513"></a><a name="p94401033133513"></a>hss:complexityPolicys:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p13418560214"><a name="p13418560214"></a><a name="p13418560214"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1462818206411"><a name="p1462818206411"></a><a name="p1462818206411"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p8955832145210"><a name="p8955832145210"></a><a name="p8955832145210"></a>√</p>
</td>
</tr>
<tr id="row444016335358"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1442133173511"><a name="p1442133173511"></a><a name="p1442133173511"></a>批量操作恶意程序</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p13442033143515"><a name="p13442033143515"></a><a name="p13442033143515"></a>hss:maliciousPrograms:operate</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p46575616216"><a name="p46575616216"></a><a name="p46575616216"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p56471720243"><a name="p56471720243"></a><a name="p56471720243"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1197053212521"><a name="p1197053212521"></a><a name="p1197053212521"></a>√</p>
</td>
</tr>
<tr id="row144213313518"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p4442173393519"><a name="p4442173393519"></a><a name="p4442173393519"></a>批量操作开放端口</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p104421833183515"><a name="p104421833183515"></a><a name="p104421833183515"></a>hss:ports:operate</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p178505617215"><a name="p178505617215"></a><a name="p178505617215"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p26653200411"><a name="p26653200411"></a><a name="p26653200411"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p119841832135216"><a name="p119841832135216"></a><a name="p119841832135216"></a>√</p>
</td>
</tr>
<tr id="row174429333353"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p18442833113515"><a name="p18442833113515"></a><a name="p18442833113515"></a>操作配置检测风险</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1244243343516"><a name="p1244243343516"></a><a name="p1244243343516"></a>hss:configDetects:operate</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p2107195610219"><a name="p2107195610219"></a><a name="p2107195610219"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p146841920245"><a name="p146841920245"></a><a name="p146841920245"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p91123313527"><a name="p91123313527"></a><a name="p91123313527"></a>√</p>
</td>
</tr>
<tr id="row124421633103516"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p134429333355"><a name="p134429333355"></a><a name="p134429333355"></a>批量操作网站后门</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1442193314352"><a name="p1442193314352"></a><a name="p1442193314352"></a>hss:webshells:operate</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p61294562028"><a name="p61294562028"></a><a name="p61294562028"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p8702202013413"><a name="p8702202013413"></a><a name="p8702202013413"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p317833135215"><a name="p317833135215"></a><a name="p317833135215"></a>√</p>
</td>
</tr>
<tr id="row1644243313359"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p144263393514"><a name="p144263393514"></a><a name="p144263393514"></a>设置常用登录地</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p544212334357"><a name="p544212334357"></a><a name="p544212334357"></a>hss:commonLocations:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p6151856625"><a name="p6151856625"></a><a name="p6151856625"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p16723220041"><a name="p16723220041"></a><a name="p16723220041"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p103193335214"><a name="p103193335214"></a><a name="p103193335214"></a>√</p>
</td>
</tr>
<tr id="row1544263333510"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p4442203311355"><a name="p4442203311355"></a><a name="p4442203311355"></a>查询常用登录地</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p144283314359"><a name="p144283314359"></a><a name="p144283314359"></a>hss:commonLocations:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1217314564216"><a name="p1217314564216"></a><a name="p1217314564216"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p374217203416"><a name="p374217203416"></a><a name="p374217203416"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p7464335527"><a name="p7464335527"></a><a name="p7464335527"></a>√</p>
</td>
</tr>
<tr id="row13442033133516"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1944213373515"><a name="p1944213373515"></a><a name="p1944213373515"></a>设置常用登录IP</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p2442143393519"><a name="p2442143393519"></a><a name="p2442143393519"></a>hss:commonIPs:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p101969564220"><a name="p101969564220"></a><a name="p101969564220"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1876418201419"><a name="p1876418201419"></a><a name="p1876418201419"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1762633145216"><a name="p1762633145216"></a><a name="p1762633145216"></a>√</p>
</td>
</tr>
<tr id="row124425337354"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1844383319354"><a name="p1844383319354"></a><a name="p1844383319354"></a>查询常用登录IP</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p24421233203512"><a name="p24421233203512"></a><a name="p24421233203512"></a>hss:commonIPs:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p621875620218"><a name="p621875620218"></a><a name="p621875620218"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1078415201341"><a name="p1078415201341"></a><a name="p1078415201341"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p17763335218"><a name="p17763335218"></a><a name="p17763335218"></a>√</p>
</td>
</tr>
<tr id="row1144314339358"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1644314332351"><a name="p1644314332351"></a><a name="p1644314332351"></a>设置登录IP白名单</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p7443533163516"><a name="p7443533163516"></a><a name="p7443533163516"></a>hss:whiteIps:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p202411856624"><a name="p202411856624"></a><a name="p202411856624"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p8803420545"><a name="p8803420545"></a><a name="p8803420545"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1791143320525"><a name="p1791143320525"></a><a name="p1791143320525"></a>√</p>
</td>
</tr>
<tr id="row5443833143516"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p2044313318357"><a name="p2044313318357"></a><a name="p2044313318357"></a>查询登录IP白名单</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p144431433153511"><a name="p144431433153511"></a><a name="p144431433153511"></a>hss:whiteIps:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1026410561021"><a name="p1026410561021"></a><a name="p1026410561021"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p18263201642"><a name="p18263201642"></a><a name="p18263201642"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p0106203385218"><a name="p0106203385218"></a><a name="p0106203385218"></a>√</p>
</td>
</tr>
<tr id="row4443533123510"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p944319331350"><a name="p944319331350"></a><a name="p944319331350"></a>设置自定义弱口令</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p7443433163512"><a name="p7443433163512"></a><a name="p7443433163512"></a>hss:weakPwds:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1528611563219"><a name="p1528611563219"></a><a name="p1528611563219"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1984512015410"><a name="p1984512015410"></a><a name="p1984512015410"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1412210335527"><a name="p1412210335527"></a><a name="p1412210335527"></a>√</p>
</td>
</tr>
<tr id="row3443933173516"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1443633133516"><a name="p1443633133516"></a><a name="p1443633133516"></a>查询自定义弱口令</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1644333323511"><a name="p1644333323511"></a><a name="p1644333323511"></a>hss:weakPwds:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p15312856626"><a name="p15312856626"></a><a name="p15312856626"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p2868112020416"><a name="p2868112020416"></a><a name="p2868112020416"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p17138103320529"><a name="p17138103320529"></a><a name="p17138103320529"></a>√</p>
</td>
</tr>
<tr id="row11443633193518"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p20443533173515"><a name="p20443533173515"></a><a name="p20443533173515"></a>设置Web路径</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p12443133383511"><a name="p12443133383511"></a><a name="p12443133383511"></a>hss:webDirs:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p634065610215"><a name="p634065610215"></a><a name="p634065610215"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p588872016411"><a name="p588872016411"></a><a name="p588872016411"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p131542033195215"><a name="p131542033195215"></a><a name="p131542033195215"></a>√</p>
</td>
</tr>
<tr id="row15443123313351"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p444333315353"><a name="p444333315353"></a><a name="p444333315353"></a>查询Web路径</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p15443133173515"><a name="p15443133173515"></a><a name="p15443133173515"></a>hss:webDirs:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p13623561323"><a name="p13623561323"></a><a name="p13623561323"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p199084201348"><a name="p199084201348"></a><a name="p199084201348"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1917243385216"><a name="p1917243385216"></a><a name="p1917243385216"></a>√</p>
</td>
</tr>
<tr id="row184432336357"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p54439338352"><a name="p54439338352"></a><a name="p54439338352"></a>查询双因子认证服务器列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p16443103316354"><a name="p16443103316354"></a><a name="p16443103316354"></a>hss:twofactorAuth:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1138514561221"><a name="p1138514561221"></a><a name="p1138514561221"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p69282206418"><a name="p69282206418"></a><a name="p69282206418"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p121893332527"><a name="p121893332527"></a><a name="p121893332527"></a>√</p>
</td>
</tr>
<tr id="row1344363313510"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p74435331354"><a name="p74435331354"></a><a name="p74435331354"></a>设置双因子认证</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p44437331351"><a name="p44437331351"></a><a name="p44437331351"></a>hss:twofactorAuth:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p164071656527"><a name="p164071656527"></a><a name="p164071656527"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p19954520548"><a name="p19954520548"></a><a name="p19954520548"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p4204103320525"><a name="p4204103320525"></a><a name="p4204103320525"></a>√</p>
</td>
</tr>
<tr id="row24438333351"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p544343315359"><a name="p544343315359"></a><a name="p544343315359"></a>开启或关闭恶意程序自动隔离查杀</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p244393313352"><a name="p244393313352"></a><a name="p244393313352"></a>hss:automaticKillMp:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1643035614213"><a name="p1643035614213"></a><a name="p1643035614213"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1097612202040"><a name="p1097612202040"></a><a name="p1097612202040"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p192231833145210"><a name="p192231833145210"></a><a name="p192231833145210"></a>√</p>
</td>
</tr>
<tr id="row544353318352"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p744383311357"><a name="p744383311357"></a><a name="p744383311357"></a>查询恶意程序自动隔离查杀</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p5443103312356"><a name="p5443103312356"></a><a name="p5443103312356"></a>hss:automaticKillMp:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1845575611211"><a name="p1845575611211"></a><a name="p1845575611211"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1599313201741"><a name="p1599313201741"></a><a name="p1599313201741"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p7243333195215"><a name="p7243333195215"></a><a name="p7243333195215"></a>√</p>
</td>
</tr>
<tr id="row1444393313354"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p94431433123515"><a name="p94431433123515"></a><a name="p94431433123515"></a>订阅安全报告</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p164433334352"><a name="p164433334352"></a><a name="p164433334352"></a>hss:safetyReport:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p04867561028"><a name="p04867561028"></a><a name="p04867561028"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p101411211343"><a name="p101411211343"></a><a name="p101411211343"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p11257143365219"><a name="p11257143365219"></a><a name="p11257143365219"></a>√</p>
</td>
</tr>
<tr id="row4443143373513"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1644473320359"><a name="p1644473320359"></a><a name="p1644473320359"></a>查询安全报告</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p64441233163512"><a name="p64441233163512"></a><a name="p64441233163512"></a>hss:safetyReport:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p175099561324"><a name="p175099561324"></a><a name="p175099561324"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p93382113417"><a name="p93382113417"></a><a name="p93382113417"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p122721433175214"><a name="p122721433175214"></a><a name="p122721433175214"></a>√</p>
</td>
</tr>
<tr id="row18444633123516"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p17444143315358"><a name="p17444143315358"></a><a name="p17444143315358"></a>查询包周期配额</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1144417331355"><a name="p1144417331355"></a><a name="p1144417331355"></a>hss:quotas:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p553013565216"><a name="p553013565216"></a><a name="p553013565216"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1252721644"><a name="p1252721644"></a><a name="p1252721644"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p12871933135210"><a name="p12871933135210"></a><a name="p12871933135210"></a>√</p>
</td>
</tr>
<tr id="row944453320357"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p0444733193515"><a name="p0444733193515"></a><a name="p0444733193515"></a>购买配额</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p044413313515"><a name="p044413313515"></a><a name="p044413313515"></a>hss:quotas:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1755220561326"><a name="p1755220561326"></a><a name="p1755220561326"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p13702021047"><a name="p13702021047"></a><a name="p13702021047"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p203021633105215"><a name="p203021633105215"></a><a name="p203021633105215"></a>√</p>
</td>
</tr>
<tr id="row444443315353"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p19444143343514"><a name="p19444143343514"></a><a name="p19444143343514"></a>查询Agent下载地址</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p5444633173516"><a name="p5444633173516"></a><a name="p5444633173516"></a>hss:installAgent:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p12575175611219"><a name="p12575175611219"></a><a name="p12575175611219"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p6909211141"><a name="p6909211141"></a><a name="p6909211141"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p431663319521"><a name="p431663319521"></a><a name="p431663319521"></a>√</p>
</td>
</tr>
<tr id="row844403313353"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p54441533133513"><a name="p54441533133513"></a><a name="p54441533133513"></a>卸载Agent</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p104441933133515"><a name="p104441933133515"></a><a name="p104441933133515"></a>hss:agent:uninstall</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p195969564212"><a name="p195969564212"></a><a name="p195969564212"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p71091721248"><a name="p71091721248"></a><a name="p71091721248"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p16332193311527"><a name="p16332193311527"></a><a name="p16332193311527"></a>√</p>
</td>
</tr>
<tr id="row1044433323512"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1444412332355"><a name="p1444412332355"></a><a name="p1444412332355"></a>查询主机安全告警</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p18444183333513"><a name="p18444183333513"></a><a name="p18444183333513"></a>hss:alertConfig:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1861815561023"><a name="p1861815561023"></a><a name="p1861815561023"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p14130142120413"><a name="p14130142120413"></a><a name="p14130142120413"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1434819332529"><a name="p1434819332529"></a><a name="p1434819332529"></a>√</p>
</td>
</tr>
<tr id="row1344453314359"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p17444933173510"><a name="p17444933173510"></a><a name="p17444933173510"></a>设置主机安全告警</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1544403363510"><a name="p1544403363510"></a><a name="p1544403363510"></a>hss:alertConfig:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p564110562215"><a name="p564110562215"></a><a name="p564110562215"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p8146172113415"><a name="p8146172113415"></a><a name="p8146172113415"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p2363103320525"><a name="p2363103320525"></a><a name="p2363103320525"></a>√</p>
</td>
</tr>
<tr id="row444419332355"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p944433316352"><a name="p944433316352"></a><a name="p944433316352"></a>查询网页防篡改防护列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p8444133323518"><a name="p8444133323518"></a><a name="p8444133323518"></a>hss:wtpHosts:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p88546448515"><a name="p88546448515"></a><a name="p88546448515"></a>vpc:ports:get</p>
<p id="p248215541513"><a name="p248215541513"></a><a name="p248215541513"></a>vpc:publicIps:list</p>
<p id="p15206122710214"><a name="p15206122710214"></a><a name="p15206122710214"></a>ecs:cloudServers:list</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p8167721047"><a name="p8167721047"></a><a name="p8167721047"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p0379833165216"><a name="p0379833165216"></a><a name="p0379833165216"></a>√</p>
</td>
</tr>
<tr id="row944513336351"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p4445133323512"><a name="p4445133323512"></a><a name="p4445133323512"></a>开启或关闭网页防篡改</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p15445733123513"><a name="p15445733123513"></a><a name="p15445733123513"></a>hss:wtpProtect:switch</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1586716210317"><a name="p1586716210317"></a><a name="p1586716210317"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1518911211643"><a name="p1518911211643"></a><a name="p1518911211643"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p93955337525"><a name="p93955337525"></a><a name="p93955337525"></a>√</p>
</td>
</tr>
<tr id="row1444593303520"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p04455339351"><a name="p04455339351"></a><a name="p04455339351"></a>设置备份服务器</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p144451933143519"><a name="p144451933143519"></a><a name="p144451933143519"></a>hss:wtpBackup:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p9890429317"><a name="p9890429317"></a><a name="p9890429317"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1320862112414"><a name="p1320862112414"></a><a name="p1320862112414"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p16411533135211"><a name="p16411533135211"></a><a name="p16411533135211"></a>√</p>
</td>
</tr>
<tr id="row1445833173516"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1244514339356"><a name="p1244514339356"></a><a name="p1244514339356"></a>查询备份服务器</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p134454338359"><a name="p134454338359"></a><a name="p134454338359"></a>hss:wtpBackup:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1912621732"><a name="p1912621732"></a><a name="p1912621732"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p172291421946"><a name="p172291421946"></a><a name="p172291421946"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p12428183335211"><a name="p12428183335211"></a><a name="p12428183335211"></a>√</p>
</td>
</tr>
<tr id="row244563323515"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1044583383518"><a name="p1044583383518"></a><a name="p1044583383518"></a>设置防护目录</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p94451533113516"><a name="p94451533113516"></a><a name="p94451533113516"></a>hss:wtpDirectorys:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p11935182733"><a name="p11935182733"></a><a name="p11935182733"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p725014211543"><a name="p725014211543"></a><a name="p725014211543"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p12444733115220"><a name="p12444733115220"></a><a name="p12444733115220"></a>√</p>
</td>
</tr>
<tr id="row8445173313352"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p154451033173515"><a name="p154451033173515"></a><a name="p154451033173515"></a>查询防护目录列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1344520335356"><a name="p1344520335356"></a><a name="p1344520335356"></a>hss:wtpDirectorys:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p179571621437"><a name="p179571621437"></a><a name="p179571621437"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p526712216415"><a name="p526712216415"></a><a name="p526712216415"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p20461233205216"><a name="p20461233205216"></a><a name="p20461233205216"></a>√</p>
</td>
</tr>
<tr id="row1344563313350"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p34451336350"><a name="p34451336350"></a><a name="p34451336350"></a>查询网页防篡改防护记录</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p13445933163511"><a name="p13445933163511"></a><a name="p13445933163511"></a>hss:wtpReports:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p16981728315"><a name="p16981728315"></a><a name="p16981728315"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1728719218419"><a name="p1728719218419"></a><a name="p1728719218419"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1947733317528"><a name="p1947733317528"></a><a name="p1947733317528"></a>√</p>
</td>
</tr>
<tr id="row1445203315358"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1445183311357"><a name="p1445183311357"></a><a name="p1445183311357"></a>设置特权进程</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p04451533133518"><a name="p04451533133518"></a><a name="p04451533133518"></a>hss:wtpPrivilegedProcess:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p10310314312"><a name="p10310314312"></a><a name="p10310314312"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p103051121948"><a name="p103051121948"></a><a name="p103051121948"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p149453345215"><a name="p149453345215"></a><a name="p149453345215"></a>√</p>
</td>
</tr>
<tr id="row1244553316355"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p14451533143510"><a name="p14451533143510"></a><a name="p14451533143510"></a>查询特权进程列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p4445103353512"><a name="p4445103353512"></a><a name="p4445103353512"></a>hss:wtpPrivilegedProcesses:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p14281539314"><a name="p14281539314"></a><a name="p14281539314"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p03251211144"><a name="p03251211144"></a><a name="p03251211144"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p14509203319529"><a name="p14509203319529"></a><a name="p14509203319529"></a>√</p>
</td>
</tr>
<tr id="row244543393516"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p134451933103514"><a name="p134451933103514"></a><a name="p134451933103514"></a>设置防护模式</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p174451133183514"><a name="p174451133183514"></a><a name="p174451133183514"></a>hss:wtpProtectMode:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p145310313311"><a name="p145310313311"></a><a name="p145310313311"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p83474218411"><a name="p83474218411"></a><a name="p83474218411"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p18525103385217"><a name="p18525103385217"></a><a name="p18525103385217"></a>√</p>
</td>
</tr>
<tr id="row204450337354"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p14451033183514"><a name="p14451033183514"></a><a name="p14451033183514"></a>查询防护模式</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p4445133143518"><a name="p4445133143518"></a><a name="p4445133143518"></a>hss:wtpProtectMode:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p6801731239"><a name="p6801731239"></a><a name="p6801731239"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p136810211143"><a name="p136810211143"></a><a name="p136810211143"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p175431233205214"><a name="p175431233205214"></a><a name="p175431233205214"></a>√</p>
</td>
</tr>
<tr id="row54452033193511"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p154450332355"><a name="p154450332355"></a><a name="p154450332355"></a>设置防护文件系统</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p244533315354"><a name="p244533315354"></a><a name="p244533315354"></a>hss:wtpFilesystems:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p61071231317"><a name="p61071231317"></a><a name="p61071231317"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p153886212411"><a name="p153886212411"></a><a name="p153886212411"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p4558933205218"><a name="p4558933205218"></a><a name="p4558933205218"></a>√</p>
</td>
</tr>
<tr id="row8445533103510"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1844519336355"><a name="p1844519336355"></a><a name="p1844519336355"></a>查询防护文件系统列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p64457337351"><a name="p64457337351"></a><a name="p64457337351"></a>hss:wtpFilesystems:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p19131133335"><a name="p19131133335"></a><a name="p19131133335"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p154093214410"><a name="p154093214410"></a><a name="p154093214410"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p18575533125211"><a name="p18575533125211"></a><a name="p18575533125211"></a>√</p>
</td>
</tr>
<tr id="row16445233153514"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p444553353511"><a name="p444553353511"></a><a name="p444553353511"></a>设置定时关闭防护</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p54451332351"><a name="p54451332351"></a><a name="p54451332351"></a>hss:wtpScheduledProtections:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p191561431837"><a name="p191561431837"></a><a name="p191561431837"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p342882111417"><a name="p342882111417"></a><a name="p342882111417"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p35901433185213"><a name="p35901433185213"></a><a name="p35901433185213"></a>√</p>
</td>
</tr>
<tr id="row1444593383516"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p114463336356"><a name="p114463336356"></a><a name="p114463336356"></a>查询定时关闭防护设置</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p11445133333512"><a name="p11445133333512"></a><a name="p11445133333512"></a>hss:wtpScheduledProtections:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p5178231338"><a name="p5178231338"></a><a name="p5178231338"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1745116217418"><a name="p1745116217418"></a><a name="p1745116217418"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p10606153305212"><a name="p10606153305212"></a><a name="p10606153305212"></a>√</p>
</td>
</tr>
<tr id="row15446113318355"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p144615331351"><a name="p144615331351"></a><a name="p144615331351"></a>设置网页防篡改告警</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p20446233183516"><a name="p20446233183516"></a><a name="p20446233183516"></a>hss:wtpAlertConfig:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p14202931334"><a name="p14202931334"></a><a name="p14202931334"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1547052118416"><a name="p1547052118416"></a><a name="p1547052118416"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p762319333529"><a name="p762319333529"></a><a name="p762319333529"></a>√</p>
</td>
</tr>
<tr id="row164464336355"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p84461133173515"><a name="p84461133173515"></a><a name="p84461133173515"></a>查询网页防篡改告警</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p10446173323518"><a name="p10446173323518"></a><a name="p10446173323518"></a>hss:wtpAlertConfig:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p9226234313"><a name="p9226234313"></a><a name="p9226234313"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p14931521542"><a name="p14931521542"></a><a name="p14931521542"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p3641133395211"><a name="p3641133395211"></a><a name="p3641133395211"></a>√</p>
</td>
</tr>
<tr id="row44469330356"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p144469336355"><a name="p144469336355"></a><a name="p144469336355"></a>查询网页防篡改统计信息</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1344643312357"><a name="p1344643312357"></a><a name="p1344643312357"></a>hss:wtpDashboard:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p15249631739"><a name="p15249631739"></a><a name="p15249631739"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p85121721346"><a name="p85121721346"></a><a name="p85121721346"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p3659153318522"><a name="p3659153318522"></a><a name="p3659153318522"></a>√</p>
</td>
</tr>
<tr id="row282115810214"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p20424165372313"><a name="p20424165372313"></a><a name="p20424165372313"></a>查询策略组信息</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p68212822114"><a name="p68212822114"></a><a name="p68212822114"></a>hss:policy:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1527111313312"><a name="p1527111313312"></a><a name="p1527111313312"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p115311721544"><a name="p115311721544"></a><a name="p115311721544"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1667817333522"><a name="p1667817333522"></a><a name="p1667817333522"></a>√</p>
</td>
</tr>
<tr id="row201609155211"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p12424553182318"><a name="p12424553182318"></a><a name="p12424553182318"></a>设置策略组信息</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1116091514219"><a name="p1116091514219"></a><a name="p1116091514219"></a>hss:policy:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p13295153539"><a name="p13295153539"></a><a name="p13295153539"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p125511521549"><a name="p125511521549"></a><a name="p125511521549"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p3697733145215"><a name="p3697733145215"></a><a name="p3697733145215"></a>√</p>
</td>
</tr>
<tr id="row15851111772120"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p1142417531238"><a name="p1142417531238"></a><a name="p1142417531238"></a>查询程序运行认证</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p188511417132119"><a name="p188511417132119"></a><a name="p188511417132119"></a>hss:ars:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1321932319"><a name="p1321932319"></a><a name="p1321932319"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p4573132115419"><a name="p4573132115419"></a><a name="p4573132115419"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1071263317520"><a name="p1071263317520"></a><a name="p1071263317520"></a>√</p>
</td>
</tr>
<tr id="row345294119215"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p942410534234"><a name="p942410534234"></a><a name="p942410534234"></a>设置程序运行认证</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1545204112119"><a name="p1545204112119"></a><a name="p1545204112119"></a>hss:ars:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p103431319315"><a name="p103431319315"></a><a name="p103431319315"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p659418211741"><a name="p659418211741"></a><a name="p659418211741"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p147281333135218"><a name="p147281333135218"></a><a name="p147281333135218"></a>√</p>
</td>
</tr>
<tr id="row8222445210"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p9424155314238"><a name="p9424155314238"></a><a name="p9424155314238"></a>查询入侵检测事件列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p32234462110"><a name="p32234462110"></a><a name="p32234462110"></a>hss:event:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p1036816318319"><a name="p1036816318319"></a><a name="p1036816318319"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p13615221748"><a name="p13615221748"></a><a name="p13615221748"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p117441833175213"><a name="p117441833175213"></a><a name="p117441833175213"></a>√</p>
</td>
</tr>
<tr id="row77501646182116"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p7424175316238"><a name="p7424175316238"></a><a name="p7424175316238"></a>入侵检测事件操作</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p16750144662120"><a name="p16750144662120"></a><a name="p16750144662120"></a>hss:event:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p93901033311"><a name="p93901033311"></a><a name="p93901033311"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p163452111418"><a name="p163452111418"></a><a name="p163452111418"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p9759173335212"><a name="p9759173335212"></a><a name="p9759173335212"></a>√</p>
</td>
</tr>
<tr id="row033383714222"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p18424145372318"><a name="p18424145372318"></a><a name="p18424145372318"></a>查询服务器分组信息</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p73338371223"><a name="p73338371223"></a><a name="p73338371223"></a>hss:hostGroup:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p124141232314"><a name="p124141232314"></a><a name="p124141232314"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p116514211412"><a name="p116514211412"></a><a name="p116514211412"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p177583310524"><a name="p177583310524"></a><a name="p177583310524"></a>√</p>
</td>
</tr>
<tr id="row1996665314227"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p11424105322319"><a name="p11424105322319"></a><a name="p11424105322319"></a>设置服务器组</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p99661153202212"><a name="p99661153202212"></a><a name="p99661153202212"></a>hss:hostGroup:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p18443331316"><a name="p18443331316"></a><a name="p18443331316"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p16671521046"><a name="p16671521046"></a><a name="p16671521046"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1879253318523"><a name="p1879253318523"></a><a name="p1879253318523"></a>√</p>
</td>
</tr>
<tr id="row14326194122319"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p11424145311233"><a name="p11424145311233"></a><a name="p11424145311233"></a>文件完整性管理</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p1326104122317"><a name="p1326104122317"></a><a name="p1326104122317"></a>hss:keyfiles:set</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p10469123536"><a name="p10469123536"></a><a name="p10469123536"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p146924211643"><a name="p146924211643"></a><a name="p146924211643"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1980813395219"><a name="p1980813395219"></a><a name="p1980813395219"></a>√</p>
</td>
</tr>
<tr id="row17511313192313"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p3424753102317"><a name="p3424753102317"></a><a name="p3424753102317"></a>查询关键文件变更报告</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p205116133237"><a name="p205116133237"></a><a name="p205116133237"></a>hss:keyfiles:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p13489173637"><a name="p13489173637"></a><a name="p13489173637"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p1871419214415"><a name="p1871419214415"></a><a name="p1871419214415"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p1982423317529"><a name="p1982423317529"></a><a name="p1982423317529"></a>√</p>
</td>
</tr>
<tr id="row1814412235234"><td class="cellrowborder" valign="top" width="18.14%" headers="mcps1.1.6.1.1 "><p id="p242425362310"><a name="p242425362310"></a><a name="p242425362310"></a>查询自动启列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.770000000000003%" headers="mcps1.1.6.1.2 "><p id="p121441923122317"><a name="p121441923122317"></a><a name="p121441923122317"></a>hss:launch:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.1.6.1.3 "><p id="p85131531632"><a name="p85131531632"></a><a name="p85131531632"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.220000000000002%" headers="mcps1.1.6.1.4 "><p id="p17355211249"><a name="p17355211249"></a><a name="p17355211249"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="23.18%" headers="mcps1.1.6.1.5 "><p id="p12840333135216"><a name="p12840333135216"></a><a name="p12840333135216"></a>√</p>
</td>
</tr>
</tbody>
</table>

