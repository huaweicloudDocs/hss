# 支持云审计的HSS操作列表<a name="hss_01_0071"></a>

企业主机安全通过云审计服务（Cloud Trace Service，CTS）为用户提供云服务资源的操作记录，记录内容包括用户从管理控制台或者开放API发起的云服务资源操作请求以及每次请求的结果，供用户查询、审计和回溯使用。

云审计服务支持的HSS操作列表如[表1](#table24308247181417)所示。

**表 1**  云审计服务支持的HSS操作列表

<a name="table24308247181417"></a>
<table><thead align="left"><tr id="row23938145181417"><th class="cellrowborder" valign="top" width="43%" id="mcps1.2.4.1.1"><p id="p66527987181455"><a name="p66527987181455"></a><a name="p66527987181455"></a>操作名称</p>
</th>
<th class="cellrowborder" valign="top" width="24%" id="mcps1.2.4.1.2"><p id="p20057853181455"><a name="p20057853181455"></a><a name="p20057853181455"></a>资源类型</p>
</th>
<th class="cellrowborder" valign="top" width="33%" id="mcps1.2.4.1.3"><p id="p14073416181455"><a name="p14073416181455"></a><a name="p14073416181455"></a>事件名称</p>
</th>
</tr>
</thead>
<tbody><tr id="row58092716181417"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p60998591181455"><a name="p60998591181455"></a><a name="p60998591181455"></a>开启主机安全防护</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p41938876181455"><a name="p41938876181455"></a><a name="p41938876181455"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p41605785181455"><a name="p41605785181455"></a><a name="p41605785181455"></a>openHssProtect</p>
</td>
</tr>
<tr id="row66834545181417"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p50833866201253"><a name="p50833866201253"></a><a name="p50833866201253"></a>关闭主机安全防护</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p58720953181455"><a name="p58720953181455"></a><a name="p58720953181455"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p58776730181455"><a name="p58776730181455"></a><a name="p58776730181455"></a>closeHssProtect</p>
</td>
</tr>
<tr id="row29947516181417"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p38551357181455"><a name="p38551357181455"></a><a name="p38551357181455"></a>手动检测</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p35652233181455"><a name="p35652233181455"></a><a name="p35652233181455"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p2149794181455"><a name="p2149794181455"></a><a name="p2149794181455"></a>manualDetection</p>
</td>
</tr>
<tr id="row10571659181417"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p23696365181455"><a name="p23696365181455"></a><a name="p23696365181455"></a>解除封禁IP</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p40357412181455"><a name="p40357412181455"></a><a name="p40357412181455"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p47724931181455"><a name="p47724931181455"></a><a name="p47724931181455"></a>unblockIp</p>
</td>
</tr>
<tr id="row64234896111241"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p35644097111241"><a name="p35644097111241"></a><a name="p35644097111241"></a>设置常用登录地</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1490746111241"><a name="p1490746111241"></a><a name="p1490746111241"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p53641636111241"><a name="p53641636111241"></a><a name="p53641636111241"></a>setCommonLocation</p>
</td>
</tr>
<tr id="row43273696111250"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p15508516111250"><a name="p15508516111250"></a><a name="p15508516111250"></a>设置登录IP白名单</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p48230284111250"><a name="p48230284111250"></a><a name="p48230284111250"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p14338945111250"><a name="p14338945111250"></a><a name="p14338945111250"></a>setWhiteIpList</p>
</td>
</tr>
<tr id="row6201522111247"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p32561289111247"><a name="p32561289111247"></a><a name="p32561289111247"></a>启用或停用登录IP白名单</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p20218781111247"><a name="p20218781111247"></a><a name="p20218781111247"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p27108565111247"><a name="p27108565111247"></a><a name="p27108565111247"></a>switchWhiteIpList</p>
</td>
</tr>
<tr id="row60043060111244"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p31649681111244"><a name="p31649681111244"></a><a name="p31649681111244"></a>设置自定义弱口令</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p13487350111244"><a name="p13487350111244"></a><a name="p13487350111244"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p18733580111244"><a name="p18733580111244"></a><a name="p18733580111244"></a>setWeakPwd</p>
</td>
</tr>
<tr id="row3259079811356"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p2260895911356"><a name="p2260895911356"></a><a name="p2260895911356"></a>设置告警信息</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1938642211356"><a name="p1938642211356"></a><a name="p1938642211356"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p2679631211356"><a name="p2679631211356"></a><a name="p2679631211356"></a>setAlarm</p>
</td>
</tr>
<tr id="row23617716388"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p1236210793812"><a name="p1236210793812"></a><a name="p1236210793812"></a>开启自动识别Web路径</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p113623703817"><a name="p113623703817"></a><a name="p113623703817"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p136210713814"><a name="p136210713814"></a><a name="p136210713814"></a>openAutoIdentify</p>
</td>
</tr>
<tr id="row73841201142"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p612428771142"><a name="p612428771142"></a><a name="p612428771142"></a>关闭自动识别Web路径</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p617260271142"><a name="p617260271142"></a><a name="p617260271142"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p337522651142"><a name="p337522651142"></a><a name="p337522651142"></a>closeAutoIdentify</p>
</td>
</tr>
<tr id="row17476121020530"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p8841712145314"><a name="p8841712145314"></a><a name="p8841712145314"></a>手动添加Web路径</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p884171245318"><a name="p884171245318"></a><a name="p884171245318"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p2084161275312"><a name="p2084161275312"></a><a name="p2084161275312"></a>setWebDir</p>
</td>
</tr>
<tr id="row1976411501226"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p137611052122210"><a name="p137611052122210"></a><a name="p137611052122210"></a>忽略端口</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p15761175212210"><a name="p15761175212210"></a><a name="p15761175212210"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p19761165272219"><a name="p19761165272219"></a><a name="p19761165272219"></a>ignorePort</p>
</td>
</tr>
<tr id="row671811472317"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p18718191414237"><a name="p18718191414237"></a><a name="p18718191414237"></a>取消忽略端口</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p97186146233"><a name="p97186146233"></a><a name="p97186146233"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p01574318260"><a name="p01574318260"></a><a name="p01574318260"></a>noIgnorePort</p>
</td>
</tr>
<tr id="row728573717234"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p628519376236"><a name="p628519376236"></a><a name="p628519376236"></a>忽略恶意程序</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p15285737182320"><a name="p15285737182320"></a><a name="p15285737182320"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p6785183718358"><a name="p6785183718358"></a><a name="p6785183718358"></a>ignoreMalwareProgram</p>
</td>
</tr>
<tr id="row1155894272312"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p14558842182320"><a name="p14558842182320"></a><a name="p14558842182320"></a>取消忽略恶意程序</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p14558164214236"><a name="p14558164214236"></a><a name="p14558164214236"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p1558942142316"><a name="p1558942142316"></a><a name="p1558942142316"></a>notIgnoreMalwareProgram</p>
</td>
</tr>
<tr id="row87991434185313"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p11314123919536"><a name="p11314123919536"></a><a name="p11314123919536"></a>隔离查杀恶意程序</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p15314103914534"><a name="p15314103914534"></a><a name="p15314103914534"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p43148395535"><a name="p43148395535"></a><a name="p43148395535"></a>isolationKillMalwareProgram</p>
</td>
</tr>
<tr id="row4721103717536"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p231463913539"><a name="p231463913539"></a><a name="p231463913539"></a>取消隔离恶意程序</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p4314103975311"><a name="p4314103975311"></a><a name="p4314103975311"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p1431453919534"><a name="p1431453919534"></a><a name="p1431453919534"></a>notIsolationMalwareProgram</p>
</td>
</tr>
<tr id="row345045619517"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p1048019114616"><a name="p1048019114616"></a><a name="p1048019114616"></a>忽略疑似恶意程序</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p8480511567"><a name="p8480511567"></a><a name="p8480511567"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p1048113117618"><a name="p1048113117618"></a><a name="p1048113117618"></a>ignoreSuspectMP</p>
</td>
</tr>
<tr id="row15932115612"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p1848121119612"><a name="p1848121119612"></a><a name="p1848121119612"></a>取消忽略疑似恶意程序</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p2048115111160"><a name="p2048115111160"></a><a name="p2048115111160"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p1148131120613"><a name="p1148131120613"></a><a name="p1148131120613"></a>notIgnoreSuspectMP</p>
</td>
</tr>
<tr id="row18513184167"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p148115114615"><a name="p148115114615"></a><a name="p148115114615"></a>隔离查杀疑似恶意程序</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1148141117618"><a name="p1148141117618"></a><a name="p1148141117618"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p194811311769"><a name="p194811311769"></a><a name="p194811311769"></a>isolationKillSuspectMP</p>
</td>
</tr>
<tr id="row172951496616"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p184814111769"><a name="p184814111769"></a><a name="p184814111769"></a>取消隔离疑似恶意程序</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p3481131115617"><a name="p3481131115617"></a><a name="p3481131115617"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p24812011169"><a name="p24812011169"></a><a name="p24812011169"></a>notIsolationKillSuspectMP</p>
</td>
</tr>
<tr id="row98251614619"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p134813113614"><a name="p134813113614"></a><a name="p134813113614"></a>忽略配置风险</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1748112111363"><a name="p1748112111363"></a><a name="p1748112111363"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p54811111768"><a name="p54811111768"></a><a name="p54811111768"></a>ignoreConfigRisky</p>
</td>
</tr>
<tr id="row181166592056"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p848211117616"><a name="p848211117616"></a><a name="p848211117616"></a>取消忽略配置风险</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p134822011266"><a name="p134822011266"></a><a name="p134822011266"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p144829111368"><a name="p144829111368"></a><a name="p144829111368"></a>notIgnoreConfigRisky</p>
</td>
</tr>
<tr id="row1373864712315"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p12738174714234"><a name="p12738174714234"></a><a name="p12738174714234"></a>忽略软件漏洞</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1273864792318"><a name="p1273864792318"></a><a name="p1273864792318"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p18738647102316"><a name="p18738647102316"></a><a name="p18738647102316"></a>ignoreVul</p>
</td>
</tr>
<tr id="row10105164552312"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p131051145142314"><a name="p131051145142314"></a><a name="p131051145142314"></a>取消忽略软件漏洞</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1410574522314"><a name="p1410574522314"></a><a name="p1410574522314"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p51051445112311"><a name="p51051445112311"></a><a name="p51051445112311"></a>notIgnoreVul</p>
</td>
</tr>
<tr id="row57086514520"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p511416455320"><a name="p511416455320"></a><a name="p511416455320"></a>开启防火墙</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1711414415317"><a name="p1711414415317"></a><a name="p1711414415317"></a>HSS</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p194159613455"><a name="p194159613455"></a><a name="p194159613455"></a>turnonFirewall</p>
</td>
</tr>
<tr id="row1564615154516"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p611410411531"><a name="p611410411531"></a><a name="p611410411531"></a>网页防篡改开启防护</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p91149455315"><a name="p91149455315"></a><a name="p91149455315"></a>HSS</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p84154611457"><a name="p84154611457"></a><a name="p84154611457"></a>openWtp</p>
</td>
</tr>
<tr id="row19561820513"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p911416455314"><a name="p911416455314"></a><a name="p911416455314"></a>网页防篡改关闭防护</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p171143419537"><a name="p171143419537"></a><a name="p171143419537"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p1741556164517"><a name="p1741556164517"></a><a name="p1741556164517"></a>stopWtp</p>
</td>
</tr>
<tr id="row13975202011519"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p2011415410539"><a name="p2011415410539"></a><a name="p2011415410539"></a>网页防篡改添加防护目录</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p3114944533"><a name="p3114944533"></a><a name="p3114944533"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p134151367459"><a name="p134151367459"></a><a name="p134151367459"></a>addWtpDir</p>
</td>
</tr>
<tr id="row1338052305114"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p1611418410535"><a name="p1611418410535"></a><a name="p1611418410535"></a>网页防篡改删除防护目录</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1611474145315"><a name="p1611474145315"></a><a name="p1611474145315"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p341546174518"><a name="p341546174518"></a><a name="p341546174518"></a>deleteWtpDir</p>
</td>
</tr>
<tr id="row128372665112"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p101148455316"><a name="p101148455316"></a><a name="p101148455316"></a>网页防篡改修改防护目录</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1211454185315"><a name="p1211454185315"></a><a name="p1211454185315"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p24155664519"><a name="p24155664519"></a><a name="p24155664519"></a>modifyWtpDir</p>
</td>
</tr>
<tr id="row928616429512"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p101145405316"><a name="p101145405316"></a><a name="p101145405316"></a>网页防篡改暂停防护目录</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p11149465310"><a name="p11149465310"></a><a name="p11149465310"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p7415146164511"><a name="p7415146164511"></a><a name="p7415146164511"></a>suspendWtpDir</p>
</td>
</tr>
<tr id="row2096054414514"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p141141415539"><a name="p141141415539"></a><a name="p141141415539"></a>网页防篡改恢复防护目录</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p51141043535"><a name="p51141043535"></a><a name="p51141043535"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p4415106154510"><a name="p4415106154510"></a><a name="p4415106154510"></a>resumeWtpDir</p>
</td>
</tr>
<tr id="row17786010135120"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p211416455314"><a name="p211416455314"></a><a name="p211416455314"></a>网页防篡改设置备份服务器</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p2011415420539"><a name="p2011415420539"></a><a name="p2011415420539"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p14415260452"><a name="p14415260452"></a><a name="p14415260452"></a>setWtpBackupHost</p>
</td>
</tr>
<tr id="row3514511510"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p201147417536"><a name="p201147417536"></a><a name="p201147417536"></a>网页防篡改设置远端备份</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1334454644510"><a name="p1334454644510"></a><a name="p1334454644510"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p94154615454"><a name="p94154615454"></a><a name="p94154615454"></a>setWtpRemoteBackup</p>
</td>
</tr>
<tr id="row204888275459"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p149001035104512"><a name="p149001035104512"></a><a name="p149001035104512"></a>网页防篡改添加特权进程</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p18488527114516"><a name="p18488527114516"></a><a name="p18488527114516"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p15727114613453"><a name="p15727114613453"></a><a name="p15727114613453"></a>addWtpPrivilegedProcess</p>
</td>
</tr>
<tr id="row206323256459"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p1790093518457"><a name="p1790093518457"></a><a name="p1790093518457"></a>网页防篡改删除特权进程</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p16322251452"><a name="p16322251452"></a><a name="p16322251452"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p10727184644518"><a name="p10727184644518"></a><a name="p10727184644518"></a>deleteWtpPrivilegedProcess</p>
</td>
</tr>
<tr id="row194242234518"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p290043554520"><a name="p290043554520"></a><a name="p290043554520"></a>网页防篡改修改特权进程</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p94252284515"><a name="p94252284515"></a><a name="p94252284515"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p11727184617457"><a name="p11727184617457"></a><a name="p11727184617457"></a>modifyWtpPrivilegedProcess</p>
</td>
</tr>
<tr id="row7834885111"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p611484165313"><a name="p611484165313"></a><a name="p611484165313"></a>开启双因子认证</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p18828148144516"><a name="p18828148144516"></a><a name="p18828148144516"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p341510620453"><a name="p341510620453"></a><a name="p341510620453"></a>turnOnTwoFactor</p>
</td>
</tr>
<tr id="row598765315519"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p5114184155310"><a name="p5114184155310"></a><a name="p5114184155310"></a>关闭双因子认证</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p16984185017459"><a name="p16984185017459"></a><a name="p16984185017459"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p7415116194515"><a name="p7415116194515"></a><a name="p7415116194515"></a>turnOffTwoFactor</p>
</td>
</tr>
<tr id="row98311056175110"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p111146415536"><a name="p111146415536"></a><a name="p111146415536"></a>修改双因子认证主题</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p567118520454"><a name="p567118520454"></a><a name="p567118520454"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p12415196194511"><a name="p12415196194511"></a><a name="p12415196194511"></a>modifyTwoFactorTopic</p>
</td>
</tr>
<tr id="row1334912261464"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p8690553490"><a name="p8690553490"></a><a name="p8690553490"></a>忽略网站后门</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1269075144920"><a name="p1269075144920"></a><a name="p1269075144920"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p5690457492"><a name="p5690457492"></a><a name="p5690457492"></a>ignoreWebShell</p>
</td>
</tr>
<tr id="row1480217308474"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p1069015524911"><a name="p1069015524911"></a><a name="p1069015524911"></a>取消忽略网站后门</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1169010512491"><a name="p1169010512491"></a><a name="p1169010512491"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p36901253495"><a name="p36901253495"></a><a name="p36901253495"></a>notIgnoreWebShell</p>
</td>
</tr>
<tr id="row1933082974716"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p16690253492"><a name="p16690253492"></a><a name="p16690253492"></a>卸载客户端</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p166911657494"><a name="p166911657494"></a><a name="p166911657494"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p186916514499"><a name="p186916514499"></a><a name="p186916514499"></a>unInstall</p>
</td>
</tr>
<tr id="row915517161475"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p2691358495"><a name="p2691358495"></a><a name="p2691358495"></a>网页防篡改设置保护模式</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p196913512491"><a name="p196913512491"></a><a name="p196913512491"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p46911654498"><a name="p46911654498"></a><a name="p46911654498"></a>setProtectMode</p>
</td>
</tr>
<tr id="row44181548114720"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p66911456499"><a name="p66911456499"></a><a name="p66911456499"></a>网页防篡改添加被保护文件系统</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p86911952491"><a name="p86911952491"></a><a name="p86911952491"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p16911659491"><a name="p16911659491"></a><a name="p16911659491"></a>addFileSystem</p>
</td>
</tr>
<tr id="row1260422724710"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p669111514496"><a name="p669111514496"></a><a name="p669111514496"></a>网页防篡改删除被保护文件系统</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p9691125154911"><a name="p9691125154911"></a><a name="p9691125154911"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p76911357490"><a name="p76911357490"></a><a name="p76911357490"></a>delFileSystem</p>
</td>
</tr>
<tr id="row1553143415481"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p1969116516498"><a name="p1969116516498"></a><a name="p1969116516498"></a>网页防篡改修改被保护文件系统</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p16692115154916"><a name="p16692115154916"></a><a name="p16692115154916"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p1069212519492"><a name="p1069212519492"></a><a name="p1069212519492"></a>modifyFileSystem</p>
</td>
</tr>
<tr id="row127881452174815"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p9692195164917"><a name="p9692195164917"></a><a name="p9692195164917"></a>网页防篡改暂停被保护文件系统</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1569213513492"><a name="p1569213513492"></a><a name="p1569213513492"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p1969217574910"><a name="p1969217574910"></a><a name="p1969217574910"></a>suspendFileSystem</p>
</td>
</tr>
<tr id="row15212145118480"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p66923512499"><a name="p66923512499"></a><a name="p66923512499"></a>网页防篡改恢复被保护文件系统</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p166926520494"><a name="p166926520494"></a><a name="p166926520494"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p186921534915"><a name="p186921534915"></a><a name="p186921534915"></a>resumeFileSystem</p>
</td>
</tr>
<tr id="row326212455487"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p1969215519492"><a name="p1969215519492"></a><a name="p1969215519492"></a>网页防篡改开启定时停止防护功能</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1369215174913"><a name="p1369215174913"></a><a name="p1369215174913"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p869218512494"><a name="p869218512494"></a><a name="p869218512494"></a>turnonTimedStopProtect</p>
</td>
</tr>
<tr id="row18422104916481"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p4692559492"><a name="p4692559492"></a><a name="p4692559492"></a>网页防篡改关闭定时停止防护功能</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1692165124920"><a name="p1692165124920"></a><a name="p1692165124920"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p1269216584919"><a name="p1269216584919"></a><a name="p1269216584919"></a>turnoffTimedStopProtect</p>
</td>
</tr>
<tr id="row161759470484"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p1069217510498"><a name="p1069217510498"></a><a name="p1069217510498"></a>网页防篡改设置定时停止防护执行周期</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p10693135144917"><a name="p10693135144917"></a><a name="p10693135144917"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p16933554915"><a name="p16933554915"></a><a name="p16933554915"></a>setTimedStopDate</p>
</td>
</tr>
<tr id="row18667143934815"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p9693053496"><a name="p9693053496"></a><a name="p9693053496"></a>网页防篡改添加停止防护时间段</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p96931584915"><a name="p96931584915"></a><a name="p96931584915"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p156939584916"><a name="p156939584916"></a><a name="p156939584916"></a>addTimerRange</p>
</td>
</tr>
<tr id="row144041743124812"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p1969315554917"><a name="p1969315554917"></a><a name="p1969315554917"></a>网页防篡改修改停止防护时间段</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p169317554919"><a name="p169317554919"></a><a name="p169317554919"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p166930515497"><a name="p166930515497"></a><a name="p166930515497"></a>modifyTimerRange</p>
</td>
</tr>
<tr id="row11539184112485"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p869316574918"><a name="p869316574918"></a><a name="p869316574918"></a>网页防篡改删除停止防护时间段</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p86937511493"><a name="p86937511493"></a><a name="p86937511493"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p16931651496"><a name="p16931651496"></a><a name="p16931651496"></a>delTimerRange</p>
</td>
</tr>
<tr id="row92014388483"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p1693195174916"><a name="p1693195174916"></a><a name="p1693195174916"></a>设置网页防篡改告警</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p969320515497"><a name="p969320515497"></a><a name="p969320515497"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p1669317554917"><a name="p1669317554917"></a><a name="p1669317554917"></a>setWtpAlertConfig</p>
</td>
</tr>
<tr id="row5452143619485"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p17693757492"><a name="p17693757492"></a><a name="p17693757492"></a>开启动态网页防篡改</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p66931751492"><a name="p66931751492"></a><a name="p66931751492"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p669315114913"><a name="p669315114913"></a><a name="p669315114913"></a>turnonRasp</p>
</td>
</tr>
<tr id="row164471532154815"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p869345124915"><a name="p869345124915"></a><a name="p869345124915"></a>关闭动态网页防篡改</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p269320584917"><a name="p269320584917"></a><a name="p269320584917"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p116937594917"><a name="p116937594917"></a><a name="p116937594917"></a>turnoffRasp</p>
</td>
</tr>
<tr id="row1736214145472"><td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.1 "><p id="p66948534916"><a name="p66948534916"></a><a name="p66948534916"></a>订阅安全报告</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p269411594918"><a name="p269411594918"></a><a name="p269411594918"></a>hss</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.3 "><p id="p1369414512498"><a name="p1369414512498"></a><a name="p1369414512498"></a>subSafetyReport</p>
</td>
</tr>
</tbody>
</table>

