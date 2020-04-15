# HSS授权项说明<a name="hss_01_0006"></a>

## 支持的授权项<a name="section677212217497"></a>

策略包含系统策略和自定义策略，如果系统策略不满足授权要求，管理员可以创建自定义策略，并通过给用户组授予自定义策略来进行精细的访问控制。策略支持的操作与API相对应，授权项列表说明如下：

-   权限：允许或拒绝某项操作。
-   授权项：自定义策略中支持的Action，在自定义策略中的Action中写入授权项，可以实现授权项对应的权限功能。
-   授权范围：自定义策略的授权范围，包括IAM项目与企业项目。授权范围如果同时支持IAM项目和企业项目，表示此授权项对应的自定义策略，可以在IAM和企业管理两个服务中给用户组授权并生效。如果仅支持IAM项目，不支持企业项目，表示仅能在IAM中给用户组授权并生效，如果在企业管理中授权，则该自定义策略不生效。关于IAM项目与企业项目的区别，详情请参见：[IAM与企业管理的区别](https://support.huaweicloud.com/iam_faq/iam_01_0101.html)。

企业主机安全服务（HSS）支持的自定义策略授权项如下所示：

[授权列表](#section15113173595712)，包含HSS对应的授权项，如查询主机安全防护列表、云服务器开启或关闭防护、手动检测等。

## 授权列表<a name="section15113173595712"></a>

<a name="table8211143315354"></a>
<table><thead align="left"><tr id="row144381133183517"><th class="cellrowborder" valign="top" width="21.22%" id="mcps1.1.4.1.1"><p id="p1443820332357"><a name="p1443820332357"></a><a name="p1443820332357"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="28.32%" id="mcps1.1.4.1.2"><p id="p19438733133512"><a name="p19438733133512"></a><a name="p19438733133512"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="50.46000000000001%" id="mcps1.1.4.1.3"><p id="p1834910910535"><a name="p1834910910535"></a><a name="p1834910910535"></a>授权范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row84382333355"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p94384333351"><a name="p94384333351"></a><a name="p94384333351"></a>查询主机安全防护列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1543833320356"><a name="p1543833320356"></a><a name="p1543833320356"></a>hss:hosts:list</p>
<p id="p114779181502"><a name="p114779181502"></a><a name="p114779181502"></a>vpc:ports:get</p>
<p id="p378516477505"><a name="p378516477505"></a><a name="p378516477505"></a>vpc:publicIps:list</p>
<p id="p1943858115019"><a name="p1943858115019"></a><a name="p1943858115019"></a>ecs:cloudServers:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul431011172088"></a><a name="ul431011172088"></a><ul id="ul431011172088"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row3438233163513"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p143893353510"><a name="p143893353510"></a><a name="p143893353510"></a>云服务器开启或关闭防护</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1843833313350"><a name="p1843833313350"></a><a name="p1843833313350"></a>hss:hosts:switchVersion</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul750995113119"></a><a name="ul750995113119"></a><ul id="ul750995113119"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row843813332359"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p243853313517"><a name="p243853313517"></a><a name="p243853313517"></a>手动检测</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p5438103313515"><a name="p5438103313515"></a><a name="p5438103313515"></a>hss:hosts:manualDetect</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul2552951191115"></a><a name="ul2552951191115"></a><ul id="ul2552951191115"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row15438333173516"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p184381733133513"><a name="p184381733133513"></a><a name="p184381733133513"></a>手动检测返回检测状态</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p5438203317353"><a name="p5438203317353"></a><a name="p5438203317353"></a>hss:manualDetectStatus:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul456475116117"></a><a name="ul456475116117"></a><ul id="ul456475116117"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row2438833113519"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p14439183316351"><a name="p14439183316351"></a><a name="p14439183316351"></a>查询弱口令检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1343918338356"><a name="p1343918338356"></a><a name="p1343918338356"></a>hss:weakPwds:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul18575451101118"></a><a name="ul18575451101118"></a><ul id="ul18575451101118"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row44391033103510"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p9439153316352"><a name="p9439153316352"></a><a name="p9439153316352"></a>查询账户破解防护报告</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p5439123318357"><a name="p5439123318357"></a><a name="p5439123318357"></a>hss:accountCracks:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul95882051191114"></a><a name="ul95882051191114"></a><ul id="ul95882051191114"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row2439203317357"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p154397332352"><a name="p154397332352"></a><a name="p154397332352"></a>账户破解防护解除拦截IP</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p243953312353"><a name="p243953312353"></a><a name="p243953312353"></a>hss:accountCracks:unblock</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul46041951151115"></a><a name="ul46041951151115"></a><ul id="ul46041951151115"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row19439203313511"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p043963383517"><a name="p043963383517"></a><a name="p043963383517"></a>查询恶意程序检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p194391433183510"><a name="p194391433183510"></a><a name="p194391433183510"></a>hss:maliciousPrograms:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul206191051181110"></a><a name="ul206191051181110"></a><ul id="ul206191051181110"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row13439733173510"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p10439133311357"><a name="p10439133311357"></a><a name="p10439133311357"></a>查询异地登录检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p24396335354"><a name="p24396335354"></a><a name="p24396335354"></a>hss:abnorLogins:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul156341151141112"></a><a name="ul156341151141112"></a><ul id="ul156341151141112"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row843963383520"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p143913303513"><a name="p143913303513"></a><a name="p143913303513"></a>查询关键文件变更报告</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p84391533123518"><a name="p84391533123518"></a><a name="p84391533123518"></a>hss:keyfiles:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul1265115151119"></a><a name="ul1265115151119"></a><ul id="ul1265115151119"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row94391333123511"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p174396335354"><a name="p174396335354"></a><a name="p174396335354"></a>查询开放端口信息列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1743920337358"><a name="p1743920337358"></a><a name="p1743920337358"></a>hss:ports:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul9664205110114"></a><a name="ul9664205110114"></a><ul id="ul9664205110114"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1943993316358"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p0439153315356"><a name="p0439153315356"></a><a name="p0439153315356"></a>查询漏洞列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p13439173383512"><a name="p13439173383512"></a><a name="p13439173383512"></a>hss:vuls:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul1068195141110"></a><a name="ul1068195141110"></a><ul id="ul1068195141110"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row144398331352"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1243903317358"><a name="p1243903317358"></a><a name="p1243903317358"></a>批量操作漏洞</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p11439113383518"><a name="p11439113383518"></a><a name="p11439113383518"></a>hss:vuls:operate</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul66969511116"></a><a name="ul66969511116"></a><ul id="ul66969511116"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row16439113313515"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p043903333518"><a name="p043903333518"></a><a name="p043903333518"></a>查询账号信息列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p6439123373515"><a name="p6439123373515"></a><a name="p6439123373515"></a>hss:accounts:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul14709851191114"></a><a name="ul14709851191114"></a><ul id="ul14709851191114"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1843917337353"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1443963333514"><a name="p1443963333514"></a><a name="p1443963333514"></a>查询软件信息列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p243973343517"><a name="p243973343517"></a><a name="p243973343517"></a>hss:softwares:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul1172220512110"></a><a name="ul1172220512110"></a><ul id="ul1172220512110"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row3439123393518"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p9439173373512"><a name="p9439173373512"></a><a name="p9439173373512"></a>查询Web路径列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p18439203311356"><a name="p18439203311356"></a><a name="p18439203311356"></a>hss:webdirs:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul773595117113"></a><a name="ul773595117113"></a><ul id="ul773595117113"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1843916332353"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p84391233153516"><a name="p84391233153516"></a><a name="p84391233153516"></a>查询进程信息列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p134391033133516"><a name="p134391033133516"></a><a name="p134391033133516"></a>hss:processes:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul1475275112118"></a><a name="ul1475275112118"></a><ul id="ul1475275112118"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row44401133203520"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p11440123317357"><a name="p11440123317357"></a><a name="p11440123317357"></a>查询配置检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p11440153333516"><a name="p11440153333516"></a><a name="p11440153333516"></a>hss:configDetects:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul16766145110117"></a><a name="ul16766145110117"></a><ul id="ul16766145110117"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row84402033143518"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p17440103343516"><a name="p17440103343516"></a><a name="p17440103343516"></a>查询网站后门检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p19440733113516"><a name="p19440733113516"></a><a name="p19440733113516"></a>hss:webshells:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul20782185110112"></a><a name="ul20782185110112"></a><ul id="ul20782185110112"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row844013323511"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p164408335355"><a name="p164408335355"></a><a name="p164408335355"></a>查询风险账号检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1644083353511"><a name="p1644083353511"></a><a name="p1644083353511"></a>hss:riskyAccounts:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul179545110112"></a><a name="ul179545110112"></a><ul id="ul179545110112"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row12440633173515"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p14440203317351"><a name="p14440203317351"></a><a name="p14440203317351"></a>云服务器风险统计</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p18440833123517"><a name="p18440833123517"></a><a name="p18440833123517"></a>hss:riskyDashboard:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul581475161110"></a><a name="ul581475161110"></a><ul id="ul581475161110"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row744033312355"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1044017332353"><a name="p1044017332353"></a><a name="p1044017332353"></a>查询口令复杂度策略检测报告</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p94401033133513"><a name="p94401033133513"></a><a name="p94401033133513"></a>hss:complexityPolicys:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul178276512112"></a><a name="ul178276512112"></a><ul id="ul178276512112"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row444016335358"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1442133173511"><a name="p1442133173511"></a><a name="p1442133173511"></a>批量操作恶意程序</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p13442033143515"><a name="p13442033143515"></a><a name="p13442033143515"></a>hss:maliciousPrograms:operate</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul384545113119"></a><a name="ul384545113119"></a><ul id="ul384545113119"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row144213313518"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p4442173393519"><a name="p4442173393519"></a><a name="p4442173393519"></a>批量操作开放端口</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p104421833183515"><a name="p104421833183515"></a><a name="p104421833183515"></a>hss:ports:operate</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul986175151114"></a><a name="ul986175151114"></a><ul id="ul986175151114"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row174429333353"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p18442833113515"><a name="p18442833113515"></a><a name="p18442833113515"></a>操作配置检测风险</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1244243343516"><a name="p1244243343516"></a><a name="p1244243343516"></a>hss:configDetects:operate</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul13874251171117"></a><a name="ul13874251171117"></a><ul id="ul13874251171117"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row124421633103516"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p134429333355"><a name="p134429333355"></a><a name="p134429333355"></a>批量操作网站后门</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1442193314352"><a name="p1442193314352"></a><a name="p1442193314352"></a>hss:webshells:operate</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul488718515110"></a><a name="ul488718515110"></a><ul id="ul488718515110"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1644243313359"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p144263393514"><a name="p144263393514"></a><a name="p144263393514"></a>设置常用登录地</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p544212334357"><a name="p544212334357"></a><a name="p544212334357"></a>hss:commonLocations:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul14822134512414"></a><a name="ul14822134512414"></a><ul id="ul14822134512414"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1544263333510"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p4442203311355"><a name="p4442203311355"></a><a name="p4442203311355"></a>查询常用登录地</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p144283314359"><a name="p144283314359"></a><a name="p144283314359"></a>hss:commonLocations:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul1192864510410"></a><a name="ul1192864510410"></a><ul id="ul1192864510410"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row13442033133516"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1944213373515"><a name="p1944213373515"></a><a name="p1944213373515"></a>设置常用登录IP</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p2442143393519"><a name="p2442143393519"></a><a name="p2442143393519"></a>hss:commonIPs:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul594516451341"></a><a name="ul594516451341"></a><ul id="ul594516451341"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row124425337354"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1844383319354"><a name="p1844383319354"></a><a name="p1844383319354"></a>查询常用登录IP</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p24421233203512"><a name="p24421233203512"></a><a name="p24421233203512"></a>hss:commonIPs:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul179644458417"></a><a name="ul179644458417"></a><ul id="ul179644458417"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1144314339358"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1644314332351"><a name="p1644314332351"></a><a name="p1644314332351"></a>设置登录IP白名单</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p7443533163516"><a name="p7443533163516"></a><a name="p7443533163516"></a>hss:whiteIps:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul139895451441"></a><a name="ul139895451441"></a><ul id="ul139895451441"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row5443833143516"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p2044313318357"><a name="p2044313318357"></a><a name="p2044313318357"></a>查询登录IP白名单</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p144431433153511"><a name="p144431433153511"></a><a name="p144431433153511"></a>hss:whiteIps:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul785461148"></a><a name="ul785461148"></a><ul id="ul785461148"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row4443533123510"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p944319331350"><a name="p944319331350"></a><a name="p944319331350"></a>设置自定义弱口令</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p7443433163512"><a name="p7443433163512"></a><a name="p7443433163512"></a>hss:weakPwds:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul32710461147"></a><a name="ul32710461147"></a><ul id="ul32710461147"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row3443933173516"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1443633133516"><a name="p1443633133516"></a><a name="p1443633133516"></a>查询自定义弱口令</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1644333323511"><a name="p1644333323511"></a><a name="p1644333323511"></a>hss:weakPwds:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul144194617412"></a><a name="ul144194617412"></a><ul id="ul144194617412"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row11443633193518"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p20443533173515"><a name="p20443533173515"></a><a name="p20443533173515"></a>设置Web路径</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p12443133383511"><a name="p12443133383511"></a><a name="p12443133383511"></a>hss:webDirs:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><p id="p126252171112"><a name="p126252171112"></a><a name="p126252171112"></a>支持：</p>
<a name="ul172755231118"></a><a name="ul172755231118"></a><ul id="ul172755231118"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row15443123313351"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p444333315353"><a name="p444333315353"></a><a name="p444333315353"></a>查询Web路径</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p15443133173515"><a name="p15443133173515"></a><a name="p15443133173515"></a>hss:webDirs:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul10257551845"></a><a name="ul10257551845"></a><ul id="ul10257551845"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row184432336357"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p54439338352"><a name="p54439338352"></a><a name="p54439338352"></a>查询双因子认证服务器列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p16443103316354"><a name="p16443103316354"></a><a name="p16443103316354"></a>hss:twofactorAuth:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul3272125119413"></a><a name="ul3272125119413"></a><ul id="ul3272125119413"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1344363313510"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p74435331354"><a name="p74435331354"></a><a name="p74435331354"></a>设置双因子认证</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p44437331351"><a name="p44437331351"></a><a name="p44437331351"></a>hss:twofactorAuth:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul2287205119412"></a><a name="ul2287205119412"></a><ul id="ul2287205119412"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row24438333351"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p544343315359"><a name="p544343315359"></a><a name="p544343315359"></a>开启或关闭恶意程序自动隔离查杀</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p244393313352"><a name="p244393313352"></a><a name="p244393313352"></a>hss:automaticKillMp:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul163034511144"></a><a name="ul163034511144"></a><ul id="ul163034511144"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row544353318352"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p744383311357"><a name="p744383311357"></a><a name="p744383311357"></a>查询恶意程序自动隔离查杀</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p5443103312356"><a name="p5443103312356"></a><a name="p5443103312356"></a>hss:automaticKillMp:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul1631845112420"></a><a name="ul1631845112420"></a><ul id="ul1631845112420"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1444393313354"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p94431433123515"><a name="p94431433123515"></a><a name="p94431433123515"></a>订阅安全报告</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p164433334352"><a name="p164433334352"></a><a name="p164433334352"></a>hss:safetyReport:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul1833318511744"></a><a name="ul1833318511744"></a><ul id="ul1833318511744"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row4443143373513"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1644473320359"><a name="p1644473320359"></a><a name="p1644473320359"></a>查询安全报告</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p64441233163512"><a name="p64441233163512"></a><a name="p64441233163512"></a>hss:safetyReport:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul6348551244"></a><a name="ul6348551244"></a><ul id="ul6348551244"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row18444633123516"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p17444143315358"><a name="p17444143315358"></a><a name="p17444143315358"></a>查询包周期配额</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1144417331355"><a name="p1144417331355"></a><a name="p1144417331355"></a>hss:quotas:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul5249511358"></a><a name="ul5249511358"></a><ul id="ul5249511358"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row944453320357"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p0444733193515"><a name="p0444733193515"></a><a name="p0444733193515"></a>购买配额</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p044413313515"><a name="p044413313515"></a><a name="p044413313515"></a>hss:quotas:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul20344711758"></a><a name="ul20344711758"></a><ul id="ul20344711758"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row444443315353"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p19444143343514"><a name="p19444143343514"></a><a name="p19444143343514"></a>查询Agent下载地址</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p5444633173516"><a name="p5444633173516"></a><a name="p5444633173516"></a>hss:installAgent:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul123611617515"></a><a name="ul123611617515"></a><ul id="ul123611617515"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row844403313353"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p54441533133513"><a name="p54441533133513"></a><a name="p54441533133513"></a>卸载Agent</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p104441933133515"><a name="p104441933133515"></a><a name="p104441933133515"></a>hss:agent:uninstall</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul3388911752"></a><a name="ul3388911752"></a><ul id="ul3388911752"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1044433323512"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1444412332355"><a name="p1444412332355"></a><a name="p1444412332355"></a>查询主机安全告警</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p18444183333513"><a name="p18444183333513"></a><a name="p18444183333513"></a>hss:alertConfig:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul19412412510"></a><a name="ul19412412510"></a><ul id="ul19412412510"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1344453314359"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p17444933173510"><a name="p17444933173510"></a><a name="p17444933173510"></a>设置主机安全告警</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1544403363510"><a name="p1544403363510"></a><a name="p1544403363510"></a>hss:alertConfig:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul114291217512"></a><a name="ul114291217512"></a><ul id="ul114291217512"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row444419332355"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p944433316352"><a name="p944433316352"></a><a name="p944433316352"></a>查询网页防篡改防护列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p8444133323518"><a name="p8444133323518"></a><a name="p8444133323518"></a>hss:wtpHosts:list</p>
<p id="p88546448515"><a name="p88546448515"></a><a name="p88546448515"></a>vpc:ports:get</p>
<p id="p248215541513"><a name="p248215541513"></a><a name="p248215541513"></a>vpc:publicIps:list</p>
<p id="p19574215522"><a name="p19574215522"></a><a name="p19574215522"></a>ecs:cloudServers:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul3431109514"></a><a name="ul3431109514"></a><ul id="ul3431109514"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row944513336351"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p4445133323512"><a name="p4445133323512"></a><a name="p4445133323512"></a>开启或关闭网页防篡改</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p15445733123513"><a name="p15445733123513"></a><a name="p15445733123513"></a>hss:wtpProtect:switch</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul166151012511"></a><a name="ul166151012511"></a><ul id="ul166151012511"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1444593303520"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p04455339351"><a name="p04455339351"></a><a name="p04455339351"></a>设置备份服务器</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p144451933143519"><a name="p144451933143519"></a><a name="p144451933143519"></a>hss:wtpBackup:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul18761410652"></a><a name="ul18761410652"></a><ul id="ul18761410652"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1445833173516"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1244514339356"><a name="p1244514339356"></a><a name="p1244514339356"></a>查询备份服务器</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p134454338359"><a name="p134454338359"></a><a name="p134454338359"></a>hss:wtpBackup:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul13907107520"></a><a name="ul13907107520"></a><ul id="ul13907107520"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row244563323515"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1044583383518"><a name="p1044583383518"></a><a name="p1044583383518"></a>设置防护目录</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p94451533113516"><a name="p94451533113516"></a><a name="p94451533113516"></a>hss:wtpDirectorys:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul1210611103519"></a><a name="ul1210611103519"></a><ul id="ul1210611103519"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row8445173313352"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p154451033173515"><a name="p154451033173515"></a><a name="p154451033173515"></a>查询防护目录列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1344520335356"><a name="p1344520335356"></a><a name="p1344520335356"></a>hss:wtpDirectorys:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul712117102512"></a><a name="ul712117102512"></a><ul id="ul712117102512"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1344563313350"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p34451336350"><a name="p34451336350"></a><a name="p34451336350"></a>查询网页防篡改防护记录</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p13445933163511"><a name="p13445933163511"></a><a name="p13445933163511"></a>hss:wtpReports:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul18135110453"></a><a name="ul18135110453"></a><ul id="ul18135110453"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1445203315358"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1445183311357"><a name="p1445183311357"></a><a name="p1445183311357"></a>设置特权进程</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p04451533133518"><a name="p04451533133518"></a><a name="p04451533133518"></a>hss:wtpPrivilegedProcess:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul18151810852"></a><a name="ul18151810852"></a><ul id="ul18151810852"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1244553316355"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p14451533143510"><a name="p14451533143510"></a><a name="p14451533143510"></a>查询特权进程列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p4445103353512"><a name="p4445103353512"></a><a name="p4445103353512"></a>hss:wtpPrivilegedProcesses:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul19693932456"></a><a name="ul19693932456"></a><ul id="ul19693932456"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row244543393516"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p134451933103514"><a name="p134451933103514"></a><a name="p134451933103514"></a>设置防护模式</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p174451133183514"><a name="p174451133183514"></a><a name="p174451133183514"></a>hss:wtpProtectMode:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul18707132955"></a><a name="ul18707132955"></a><ul id="ul18707132955"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row204450337354"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p14451033183514"><a name="p14451033183514"></a><a name="p14451033183514"></a>查询防护模式</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p4445133143518"><a name="p4445133143518"></a><a name="p4445133143518"></a>hss:wtpProtectMode:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul87211632353"></a><a name="ul87211632353"></a><ul id="ul87211632353"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row54452033193511"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p154450332355"><a name="p154450332355"></a><a name="p154450332355"></a>设置防护文件系统</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p244533315354"><a name="p244533315354"></a><a name="p244533315354"></a>hss:wtpFilesystems:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul97361932554"></a><a name="ul97361932554"></a><ul id="ul97361932554"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row8445533103510"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1844519336355"><a name="p1844519336355"></a><a name="p1844519336355"></a>查询防护文件系统列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p64457337351"><a name="p64457337351"></a><a name="p64457337351"></a>hss:wtpFilesystems:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul17524323519"></a><a name="ul17524323519"></a><ul id="ul17524323519"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row16445233153514"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p444553353511"><a name="p444553353511"></a><a name="p444553353511"></a>设置定时关闭防护</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p54451332351"><a name="p54451332351"></a><a name="p54451332351"></a>hss:wtpScheduledProtections:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul4768432755"></a><a name="ul4768432755"></a><ul id="ul4768432755"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1444593383516"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p114463336356"><a name="p114463336356"></a><a name="p114463336356"></a>查询定时关闭防护设置</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p11445133333512"><a name="p11445133333512"></a><a name="p11445133333512"></a>hss:wtpScheduledProtections:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul2074012360510"></a><a name="ul2074012360510"></a><ul id="ul2074012360510"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row15446113318355"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p144615331351"><a name="p144615331351"></a><a name="p144615331351"></a>设置网页防篡改告警</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p20446233183516"><a name="p20446233183516"></a><a name="p20446233183516"></a>hss:wtpAlertConfig:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul1275220362051"></a><a name="ul1275220362051"></a><ul id="ul1275220362051"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row164464336355"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p84461133173515"><a name="p84461133173515"></a><a name="p84461133173515"></a>查询网页防篡改告警</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p10446173323518"><a name="p10446173323518"></a><a name="p10446173323518"></a>hss:wtpAlertConfig:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul17691236856"></a><a name="ul17691236856"></a><ul id="ul17691236856"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row44469330356"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p144469336355"><a name="p144469336355"></a><a name="p144469336355"></a>查询网页防篡改统计信息</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1344643312357"><a name="p1344643312357"></a><a name="p1344643312357"></a>hss:wtpDashboard:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul207855361857"></a><a name="ul207855361857"></a><ul id="ul207855361857"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row282115810214"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p20424165372313"><a name="p20424165372313"></a><a name="p20424165372313"></a>查询策略组信息</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p68212822114"><a name="p68212822114"></a><a name="p68212822114"></a>hss:policy:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul16629172016241"></a><a name="ul16629172016241"></a><ul id="ul16629172016241"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row201609155211"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p12424553182318"><a name="p12424553182318"></a><a name="p12424553182318"></a>设置策略组信息</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1116091514219"><a name="p1116091514219"></a><a name="p1116091514219"></a>hss:policy:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul1172442062419"></a><a name="ul1172442062419"></a><ul id="ul1172442062419"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row15851111772120"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p1142417531238"><a name="p1142417531238"></a><a name="p1142417531238"></a>查询程序运行认证</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p188511417132119"><a name="p188511417132119"></a><a name="p188511417132119"></a>hss:ars:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul207411420182412"></a><a name="ul207411420182412"></a><ul id="ul207411420182412"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row345294119215"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p942410534234"><a name="p942410534234"></a><a name="p942410534234"></a>设置程序运行认证</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1545204112119"><a name="p1545204112119"></a><a name="p1545204112119"></a>hss:ars:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul27574201245"></a><a name="ul27574201245"></a><ul id="ul27574201245"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row8222445210"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p9424155314238"><a name="p9424155314238"></a><a name="p9424155314238"></a>查询入侵检测事件列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p32234462110"><a name="p32234462110"></a><a name="p32234462110"></a>hss:event:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul197781620202414"></a><a name="ul197781620202414"></a><ul id="ul197781620202414"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row77501646182116"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p7424175316238"><a name="p7424175316238"></a><a name="p7424175316238"></a>入侵检测事件操作</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p16750144662120"><a name="p16750144662120"></a><a name="p16750144662120"></a>hss:event:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul7795120172416"></a><a name="ul7795120172416"></a><ul id="ul7795120172416"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row033383714222"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p18424145372318"><a name="p18424145372318"></a><a name="p18424145372318"></a>查询服务器分组信息</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p73338371223"><a name="p73338371223"></a><a name="p73338371223"></a>hss:hostGroup:get</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul3812112014243"></a><a name="ul3812112014243"></a><ul id="ul3812112014243"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1996665314227"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p11424105322319"><a name="p11424105322319"></a><a name="p11424105322319"></a>设置服务器组</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p99661153202212"><a name="p99661153202212"></a><a name="p99661153202212"></a>hss:hostGroup:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul883110208244"></a><a name="ul883110208244"></a><ul id="ul883110208244"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row14326194122319"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p11424145311233"><a name="p11424145311233"></a><a name="p11424145311233"></a>文件完整性校验</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p1326104122317"><a name="p1326104122317"></a><a name="p1326104122317"></a>hss:keyfiles:set</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul14850122082420"></a><a name="ul14850122082420"></a><ul id="ul14850122082420"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row17511313192313"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p3424753102317"><a name="p3424753102317"></a><a name="p3424753102317"></a>查询关键文件变更报告</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p205116133237"><a name="p205116133237"></a><a name="p205116133237"></a>hss:keyfiles:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul78686201243"></a><a name="ul78686201243"></a><ul id="ul78686201243"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1814412235234"><td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.1.4.1.1 "><p id="p242425362310"><a name="p242425362310"></a><a name="p242425362310"></a>查询自动启列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.32%" headers="mcps1.1.4.1.2 "><p id="p121441923122317"><a name="p121441923122317"></a><a name="p121441923122317"></a>hss:launch:list</p>
</td>
<td class="cellrowborder" valign="top" width="50.46000000000001%" headers="mcps1.1.4.1.3 "><a name="ul5886152032414"></a><a name="ul5886152032414"></a><ul id="ul5886152032414"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</td>
</tr>
</tbody>
</table>

