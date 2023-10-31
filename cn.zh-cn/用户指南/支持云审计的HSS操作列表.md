# 支持云审计的HSS操作列表<a name="hss_01_0071"></a>

主机安全服务通过云审计服务（Cloud Trace Service，CTS）为用户提供云服务资源的操作记录，记录内容包括用户从管理控制台或者开放API发起的云服务资源操作请求以及每次请求的结果，供用户查询、审计和回溯使用。

云审计服务支持的HSS操作列表如[表1](#table24308247181417)所示。

**表 1**  云审计服务支持的HSS操作列表

<a name="table24308247181417"></a>
<table><thead align="left"><tr id="row23938145181417"><th class="cellrowborder" valign="top" width="31.75%" id="mcps1.2.4.1.1"><p id="p66527987181455"><a name="p66527987181455"></a><a name="p66527987181455"></a>操作名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.28%" id="mcps1.2.4.1.2"><p id="p20057853181455"><a name="p20057853181455"></a><a name="p20057853181455"></a>资源类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.97%" id="mcps1.2.4.1.3"><p id="p14073416181455"><a name="p14073416181455"></a><a name="p14073416181455"></a>事件名称</p>
</th>
</tr>
</thead>
<tbody><tr id="row58092716181417"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p070415313576"><a name="p070415313576"></a><a name="p070415313576"></a>取消忽略端口</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p41938876181455"><a name="p41938876181455"></a><a name="p41938876181455"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p20215184875717"><a name="p20215184875717"></a><a name="p20215184875717"></a>notIgnorePortStatus</p>
</td>
</tr>
<tr id="row66834545181417"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1670413316579"><a name="p1670413316579"></a><a name="p1670413316579"></a>忽略端口</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p58720953181455"><a name="p58720953181455"></a><a name="p58720953181455"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p11215748145710"><a name="p11215748145710"></a><a name="p11215748145710"></a>ignorePortStatus</p>
</td>
</tr>
<tr id="row29947516181417"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p2704231195716"><a name="p2704231195716"></a><a name="p2704231195716"></a>取消忽略配置检测项</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p35652233181455"><a name="p35652233181455"></a><a name="p35652233181455"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p62151948105716"><a name="p62151948105716"></a><a name="p62151948105716"></a>notIgnoreCheckRuleStat</p>
</td>
</tr>
<tr id="row10571659181417"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p12704183135715"><a name="p12704183135715"></a><a name="p12704183135715"></a>忽略配置检测项</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p40357412181455"><a name="p40357412181455"></a><a name="p40357412181455"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p5215134875710"><a name="p5215134875710"></a><a name="p5215134875710"></a>ignoreCheckRuleStat</p>
</td>
</tr>
<tr id="row64234896111241"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p370415315579"><a name="p370415315579"></a><a name="p370415315579"></a>重新进行基线检测</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p1490746111241"><a name="p1490746111241"></a><a name="p1490746111241"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p2021594816571"><a name="p2021594816571"></a><a name="p2021594816571"></a>runBaselineDetect</p>
</td>
</tr>
<tr id="row43273696111250"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p117041031175717"><a name="p117041031175717"></a><a name="p117041031175717"></a>解绑配额</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p48230284111250"><a name="p48230284111250"></a><a name="p48230284111250"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p162151348195712"><a name="p162151348195712"></a><a name="p162151348195712"></a>cancelHostsQuota</p>
</td>
</tr>
<tr id="row6201522111247"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p197043318577"><a name="p197043318577"></a><a name="p197043318577"></a>关闭容器防护</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p20218781111247"><a name="p20218781111247"></a><a name="p20218781111247"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p32151648145719"><a name="p32151648145719"></a><a name="p32151648145719"></a>closeContainerProtectStatus</p>
</td>
</tr>
<tr id="row1976411501226"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1970412319572"><a name="p1970412319572"></a><a name="p1970412319572"></a>开启容器防护</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p15761175212210"><a name="p15761175212210"></a><a name="p15761175212210"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p221534819578"><a name="p221534819578"></a><a name="p221534819578"></a>openContainerProtectStatus</p>
</td>
</tr>
<tr id="row671811472317"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p0704731135720"><a name="p0704731135720"></a><a name="p0704731135720"></a>解除已拦截IP</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p97186146233"><a name="p97186146233"></a><a name="p97186146233"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p3215174817577"><a name="p3215174817577"></a><a name="p3215174817577"></a>changeBlockedIp</p>
</td>
</tr>
<tr id="row98251614619"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p14704931165712"><a name="p14704931165712"></a><a name="p14704931165712"></a>处理事件状态</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p1748112111363"><a name="p1748112111363"></a><a name="p1748112111363"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p821510482570"><a name="p821510482570"></a><a name="p821510482570"></a>changeEvent</p>
</td>
</tr>
<tr id="row181166592056"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p070463114576"><a name="p070463114576"></a><a name="p070463114576"></a>恢复已隔离文件</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p134822011266"><a name="p134822011266"></a><a name="p134822011266"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p11215174815571"><a name="p11215174815571"></a><a name="p11215174815571"></a>changeIsolatedFile</p>
</td>
</tr>
<tr id="row13799115464120"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p5704531115711"><a name="p5704531115711"></a><a name="p5704531115711"></a>删除告警白名单</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p147991554134120"><a name="p147991554134120"></a><a name="p147991554134120"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p421574885715"><a name="p421574885715"></a><a name="p421574885715"></a>removeAlarmWhiteList</p>
</td>
</tr>
<tr id="row3617125113417"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p37041631185719"><a name="p37041631185719"></a><a name="p37041631185719"></a>添加登录白名单</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p861715513418"><a name="p861715513418"></a><a name="p861715513418"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p20215104845715"><a name="p20215104845715"></a><a name="p20215104845715"></a>addLoginWhiteList</p>
</td>
</tr>
<tr id="row1973614482413"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p177041231155711"><a name="p177041231155711"></a><a name="p177041231155711"></a>删除登录白名单</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p373744864119"><a name="p373744864119"></a><a name="p373744864119"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p421564812574"><a name="p421564812574"></a><a name="p421564812574"></a>removeLoginWhiteList</p>
</td>
</tr>
<tr id="row1373864712315"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p11704193165714"><a name="p11704193165714"></a><a name="p11704193165714"></a>新增服务器组</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p1273864792318"><a name="p1273864792318"></a><a name="p1273864792318"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p122151448125710"><a name="p122151448125710"></a><a name="p122151448125710"></a>addHostsGroup</p>
</td>
</tr>
<tr id="row10105164552312"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1570493195716"><a name="p1570493195716"></a><a name="p1570493195716"></a>分配到服务器组</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p1410574522314"><a name="p1410574522314"></a><a name="p1410574522314"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p162151148135712"><a name="p162151148135712"></a><a name="p162151148135712"></a>associateHostsGroup</p>
</td>
</tr>
<tr id="row57086514520"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1704153118577"><a name="p1704153118577"></a><a name="p1704153118577"></a>修改服务器组</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p10313355112411"><a name="p10313355112411"></a><a name="p10313355112411"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p1721564813578"><a name="p1721564813578"></a><a name="p1721564813578"></a>changeHostsGroup</p>
</td>
</tr>
<tr id="row1564615154516"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p12704131125719"><a name="p12704131125719"></a><a name="p12704131125719"></a>删除服务器组</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p17314145552416"><a name="p17314145552416"></a><a name="p17314145552416"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p721574817575"><a name="p721574817575"></a><a name="p721574817575"></a>deleteHostsGroup</p>
</td>
</tr>
<tr id="row19561820513"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p16704183119571"><a name="p16704183119571"></a><a name="p16704183119571"></a>关闭主机防护</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p171143419537"><a name="p171143419537"></a><a name="p171143419537"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p11215104805714"><a name="p11215104805714"></a><a name="p11215104805714"></a>closeHostsProtectStatus</p>
</td>
</tr>
<tr id="row13975202011519"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1570417317575"><a name="p1570417317575"></a><a name="p1570417317575"></a>开启主机防护</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p3114944533"><a name="p3114944533"></a><a name="p3114944533"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p421544885719"><a name="p421544885719"></a><a name="p421544885719"></a>openHostsProtectStatus</p>
</td>
</tr>
<tr id="row1338052305114"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p13704113118571"><a name="p13704113118571"></a><a name="p13704113118571"></a>卸载agent</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p1611474145315"><a name="p1611474145315"></a><a name="p1611474145315"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p13215174812578"><a name="p13215174812578"></a><a name="p13215174812578"></a>uninstallAgents</p>
</td>
</tr>
<tr id="row128372665112"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p97051731145715"><a name="p97051731145715"></a><a name="p97051731145715"></a>运行镜像扫描</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p1211454185315"><a name="p1211454185315"></a><a name="p1211454185315"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p1821534818572"><a name="p1821534818572"></a><a name="p1821534818572"></a>runImageScan</p>
</td>
</tr>
<tr id="row928616429512"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p670516317571"><a name="p670516317571"></a><a name="p670516317571"></a>从SWR服务同步镜像列表</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p11149465310"><a name="p11149465310"></a><a name="p11149465310"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p17215184875713"><a name="p17215184875713"></a><a name="p17215184875713"></a>runImageSynchronizeTask</p>
</td>
</tr>
<tr id="row2096054414514"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p14705143110579"><a name="p14705143110579"></a><a name="p14705143110579"></a>更新并扫描SWR镜像</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p51141043535"><a name="p51141043535"></a><a name="p51141043535"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p142155483573"><a name="p142155483573"></a><a name="p142155483573"></a>runSwrImageScan</p>
</td>
</tr>
<tr id="row17786010135120"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1477717813588"><a name="p1477717813588"></a><a name="p1477717813588"></a>重新体检</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p2011415420539"><a name="p2011415420539"></a><a name="p2011415420539"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p10622171215599"><a name="p10622171215599"></a><a name="p10622171215599"></a>resetRiskScore</p>
</td>
</tr>
<tr id="row3514511510"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p107771884582"><a name="p107771884582"></a><a name="p107771884582"></a>添加策略组</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p1334454644510"><a name="p1334454644510"></a><a name="p1334454644510"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p136228121591"><a name="p136228121591"></a><a name="p136228121591"></a>addPolicyGroup</p>
</td>
</tr>
<tr id="row204888275459"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p11777283587"><a name="p11777283587"></a><a name="p11777283587"></a>删除策略组</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p18488527114516"><a name="p18488527114516"></a><a name="p18488527114516"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p12622012195918"><a name="p12622012195918"></a><a name="p12622012195918"></a>deletePolicyGroup</p>
</td>
</tr>
<tr id="row206323256459"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p37771188589"><a name="p37771188589"></a><a name="p37771188589"></a>部署策略组</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p16322251452"><a name="p16322251452"></a><a name="p16322251452"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p10623101218595"><a name="p10623101218595"></a><a name="p10623101218595"></a>deployPolicyGroup</p>
</td>
</tr>
<tr id="row194242234518"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1277713818585"><a name="p1277713818585"></a><a name="p1277713818585"></a>修改策略内容</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p94252284515"><a name="p94252284515"></a><a name="p94252284515"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p86237123595"><a name="p86237123595"></a><a name="p86237123595"></a>modifyPolicyDetail</p>
</td>
</tr>
<tr id="row7834885111"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p87777885818"><a name="p87777885818"></a><a name="p87777885818"></a>修改策略组</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p18828148144516"><a name="p18828148144516"></a><a name="p18828148144516"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p76231012175911"><a name="p76231012175911"></a><a name="p76231012175911"></a>modifyPolicyGroup</p>
</td>
</tr>
<tr id="row598765315519"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p37773805819"><a name="p37773805819"></a><a name="p37773805819"></a>关闭自动隔离查杀</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p16984185017459"><a name="p16984185017459"></a><a name="p16984185017459"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p6623171285915"><a name="p6623171285915"></a><a name="p6623171285915"></a>closeAutoKillVirusStatus</p>
</td>
</tr>
<tr id="row98311056175110"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1177711885818"><a name="p1177711885818"></a><a name="p1177711885818"></a>开启自动隔离查杀</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p567118520454"><a name="p567118520454"></a><a name="p567118520454"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p562312122595"><a name="p562312122595"></a><a name="p562312122595"></a>openAutoKillVirusStatus</p>
</td>
</tr>
<tr id="row1334912261464"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p57771818583"><a name="p57771818583"></a><a name="p57771818583"></a>设置常用登录IP</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p1269075144920"><a name="p1269075144920"></a><a name="p1269075144920"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p13623111295914"><a name="p13623111295914"></a><a name="p13623111295914"></a>modifyLoginCommonIp</p>
</td>
</tr>
<tr id="row1480217308474"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p877715819582"><a name="p877715819582"></a><a name="p877715819582"></a>设置常用登录地</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p1169010512491"><a name="p1169010512491"></a><a name="p1169010512491"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p162318125592"><a name="p162318125592"></a><a name="p162318125592"></a>modifyLoginCommonLocation</p>
</td>
</tr>
<tr id="row1933082974716"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p377714816584"><a name="p377714816584"></a><a name="p377714816584"></a>设置SSH登录白名单</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p166911657494"><a name="p166911657494"></a><a name="p166911657494"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p1362310123592"><a name="p1362310123592"></a><a name="p1362310123592"></a>modifyLoginWhiteIp</p>
</td>
</tr>
<tr id="row915517161475"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1577719814588"><a name="p1577719814588"></a><a name="p1577719814588"></a>修复漏洞</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p196913512491"><a name="p196913512491"></a><a name="p196913512491"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p362361218597"><a name="p362361218597"></a><a name="p362361218597"></a>changeVulStatus</p>
</td>
</tr>
<tr id="row44181548114720"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p147775812588"><a name="p147775812588"></a><a name="p147775812588"></a>添加防护目录</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p86911952491"><a name="p86911952491"></a><a name="p86911952491"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p11623171219592"><a name="p11623171219592"></a><a name="p11623171219592"></a>addHostProtectDirInfo</p>
</td>
</tr>
<tr id="row1260422724710"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p07771186584"><a name="p07771186584"></a><a name="p07771186584"></a>添加特权进程</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p9691125154911"><a name="p9691125154911"></a><a name="p9691125154911"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p166231712175917"><a name="p166231712175917"></a><a name="p166231712175917"></a>addPrivilegedProcessInfo</p>
</td>
</tr>
<tr id="row1553143415481"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1277714810581"><a name="p1277714810581"></a><a name="p1277714810581"></a>添加定时关闭防护配置</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p16692115154916"><a name="p16692115154916"></a><a name="p16692115154916"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p1362314126592"><a name="p1362314126592"></a><a name="p1362314126592"></a>addTimingOffConfigInfo</p>
</td>
</tr>
<tr id="row127881452174815"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p13777188580"><a name="p13777188580"></a><a name="p13777188580"></a>删除远端备份服务器</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p1569213513492"><a name="p1569213513492"></a><a name="p1569213513492"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p3623212145913"><a name="p3623212145913"></a><a name="p3623212145913"></a>deleteBackupHostInfo</p>
</td>
</tr>
<tr id="row15212145118480"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p07771281587"><a name="p07771281587"></a><a name="p07771281587"></a>删除防护目录</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p166926520494"><a name="p166926520494"></a><a name="p166926520494"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p662301216598"><a name="p662301216598"></a><a name="p662301216598"></a>deleteHostProtectDirInfo</p>
</td>
</tr>
<tr id="row326212455487"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p87778855819"><a name="p87778855819"></a><a name="p87778855819"></a>删除特权进程</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p1369215174913"><a name="p1369215174913"></a><a name="p1369215174913"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p362311126591"><a name="p362311126591"></a><a name="p362311126591"></a>deletePrivilegedProcessInfo</p>
</td>
</tr>
<tr id="row18422104916481"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p117778819587"><a name="p117778819587"></a><a name="p117778819587"></a>删除定时关闭防护配置</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p1692165124920"><a name="p1692165124920"></a><a name="p1692165124920"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p13623812195918"><a name="p13623812195918"></a><a name="p13623812195918"></a>deleteTimingOffConfigInfo</p>
</td>
</tr>
<tr id="row161759470484"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p17777987584"><a name="p17777987584"></a><a name="p17777987584"></a>设置定时关闭防护周期</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p10693135144917"><a name="p10693135144917"></a><a name="p10693135144917"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p16234126594"><a name="p16234126594"></a><a name="p16234126594"></a>setDateOffConfigInfo</p>
</td>
</tr>
<tr id="row18667143934815"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1677718825816"><a name="p1677718825816"></a><a name="p1677718825816"></a>修改防护目录开启状态</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p96931584915"><a name="p96931584915"></a><a name="p96931584915"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p462312125591"><a name="p462312125591"></a><a name="p462312125591"></a>setProtectDirSwitchInfo</p>
</td>
</tr>
<tr id="row144041743124812"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p147782835817"><a name="p147782835817"></a><a name="p147782835817"></a>修改动态网页防篡改状态</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p169317554919"><a name="p169317554919"></a><a name="p169317554919"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p26231112115913"><a name="p26231112115913"></a><a name="p26231112115913"></a>setRaspSwitch</p>
</td>
</tr>
<tr id="row11539184112485"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1877888145816"><a name="p1877888145816"></a><a name="p1877888145816"></a>设置远端备份服务器</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p86937511493"><a name="p86937511493"></a><a name="p86937511493"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p4623612175915"><a name="p4623612175915"></a><a name="p4623612175915"></a>setRemoteBackupInfo</p>
</td>
</tr>
<tr id="row92014388483"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p15778682589"><a name="p15778682589"></a><a name="p15778682589"></a>修改定时关闭防护状态</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p969320515497"><a name="p969320515497"></a><a name="p969320515497"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p10623161213599"><a name="p10623161213599"></a><a name="p10623161213599"></a>setTimingOffSwitchInfo</p>
</td>
</tr>
<tr id="row5452143619485"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1577814835818"><a name="p1577814835818"></a><a name="p1577814835818"></a>关闭网页防篡改防护</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p66931751492"><a name="p66931751492"></a><a name="p66931751492"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p16231612135915"><a name="p16231612135915"></a><a name="p16231612135915"></a>closeWtpProtectionStatusInfo</p>
</td>
</tr>
<tr id="row164471532154815"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p15778138145817"><a name="p15778138145817"></a><a name="p15778138145817"></a>开启网页防篡改防护</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p269320584917"><a name="p269320584917"></a><a name="p269320584917"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p26234123594"><a name="p26234123594"></a><a name="p26234123594"></a>openWtpProtectionStatusInfo</p>
</td>
</tr>
<tr id="row1736214145472"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p2778138105820"><a name="p2778138105820"></a><a name="p2778138105820"></a>修改远端备份服务器</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p269411594918"><a name="p269411594918"></a><a name="p269411594918"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p66231612185910"><a name="p66231612185910"></a><a name="p66231612185910"></a>updateBackupHostInfo</p>
</td>
</tr>
<tr id="row123182345415"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p577888175816"><a name="p577888175816"></a><a name="p577888175816"></a>修改防护目录</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p07594545420"><a name="p07594545420"></a><a name="p07594545420"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p19623121295911"><a name="p19623121295911"></a><a name="p19623121295911"></a>updateHostProtectDirInfo</p>
</td>
</tr>
<tr id="row8210930135418"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p197783845813"><a name="p197783845813"></a><a name="p197783845813"></a>修改特权进程</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p37684518546"><a name="p37684518546"></a><a name="p37684518546"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p262315123594"><a name="p262315123594"></a><a name="p262315123594"></a>updatePrivilegedProcessInfo</p>
</td>
</tr>
<tr id="row1788617294547"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p1577816819585"><a name="p1577816819585"></a><a name="p1577816819585"></a>修改Tomcat bin目录</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p3626516558"><a name="p3626516558"></a><a name="p3626516558"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p1623912175916"><a name="p1623912175916"></a><a name="p1623912175916"></a>updateRaspPathInfo</p>
</td>
</tr>
<tr id="row1155332705420"><td class="cellrowborder" valign="top" width="31.75%" headers="mcps1.2.4.1.1 "><p id="p13778286585"><a name="p13778286585"></a><a name="p13778286585"></a>修改定时关闭防护时间段</p>
</td>
<td class="cellrowborder" valign="top" width="19.28%" headers="mcps1.2.4.1.2 "><p id="p196213514557"><a name="p196213514557"></a><a name="p196213514557"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="48.97%" headers="mcps1.2.4.1.3 "><p id="p062317126596"><a name="p062317126596"></a><a name="p062317126596"></a>updateTimingOffConfigInfo</p>
</td>
</tr>
</tbody>
</table>

