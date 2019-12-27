# Windows版本<a name="hss_01_0235"></a>

在主机中安装客户端后，您才能开启企业主机安全服务。通过本节介绍，您将了解如何在Windows操作系统的主机中安装客户端。Linux操作系统的客户端安装请参见[Linux版本](Linux版本.md)。

>![](public_sys-resources/icon-note.gif) **说明：**   
>网页防篡改与主机安全共用同一个客户端，您只需在同一主机安装一次。  

## 安装场景<a name="section16825043312"></a>

企业主机安全服务支持**华为云主机**和**非华为云主机**两种安装方式，请按[表1](#hss_01_0234_table114917164498)进行选择。

**表 1**  安装场景

<a name="hss_01_0234_table114917164498"></a>
<table><thead align="left"><tr id="hss_01_0234_row4150816114916"><th class="cellrowborder" valign="top" width="21.67%" id="mcps1.2.3.1.1"><p id="hss_01_0234_p215031615493"><a name="hss_01_0234_p215031615493"></a><a name="hss_01_0234_p215031615493"></a>服务器类型</p>
</th>
<th class="cellrowborder" valign="top" width="78.33%" id="mcps1.2.3.1.2"><p id="hss_01_0234_p5150216184918"><a name="hss_01_0234_p5150216184918"></a><a name="hss_01_0234_p5150216184918"></a>如何安装Agent</p>
</th>
</tr>
</thead>
<tbody><tr id="hss_01_0234_row19150151664911"><td class="cellrowborder" rowspan="2" valign="top" width="21.67%" headers="mcps1.2.3.1.1 "><p id="hss_01_0234_p966513359117"><a name="hss_01_0234_p966513359117"></a><a name="hss_01_0234_p966513359117"></a>华为云弹性云服务器ECS</p>
<p id="hss_01_0234_p135453716115"><a name="hss_01_0234_p135453716115"></a><a name="hss_01_0234_p135453716115"></a>华为云裸金属服务器BMS</p>
</td>
<td class="cellrowborder" valign="top" width="78.33%" headers="mcps1.2.3.1.2 "><p id="hss_01_0234_p4150181614499"><a name="hss_01_0234_p4150181614499"></a><a name="hss_01_0234_p4150181614499"></a>主机与HSS配额在同一区域，请使用<strong id="hss_01_0234_b16617201129"><a name="hss_01_0234_b16617201129"></a><a name="hss_01_0234_b16617201129"></a>华为云主机</strong>的安装方式。</p>
</td>
</tr>
<tr id="hss_01_0234_row1715013165495"><td class="cellrowborder" valign="top" headers="mcps1.2.3.1.1 "><p id="hss_01_0234_p1716714918537"><a name="hss_01_0234_p1716714918537"></a><a name="hss_01_0234_p1716714918537"></a>主机与HSS配额不在同一区域：</p>
<a name="hss_01_0234_ul1677913318110"></a><a name="hss_01_0234_ul1677913318110"></a><ul id="hss_01_0234_ul1677913318110"><li>HSS配额所在区域：华北-北京一、华东-上海二、华南-广州、华北-北京四。<p id="hss_01_0234_p129001851111015"><a name="hss_01_0234_p129001851111015"></a><a name="hss_01_0234_p129001851111015"></a>请使用<strong id="hss_01_0234_b799315366126"><a name="hss_01_0234_b799315366126"></a><a name="hss_01_0234_b799315366126"></a>非华为云主机</strong>的安装方式将主机接入HSS配额所在区域。</p>
</li></ul>
<a name="hss_01_0234_ul2094613891110"></a><a name="hss_01_0234_ul2094613891110"></a><ul id="hss_01_0234_ul2094613891110"><li>HSS配额所在区域：其他区域。<p id="hss_01_0234_p68299872112"><a name="hss_01_0234_p68299872112"></a><a name="hss_01_0234_p68299872112"></a>请退订配额后重新购买配额。</p>
</li></ul>
<p id="hss_01_0234_p212169114"><a name="hss_01_0234_p212169114"></a><a name="hss_01_0234_p212169114"></a>具体操作请参见<a href="https://support.huaweicloud.com/hss_faq/hss_01_0159.html" target="_blank" rel="noopener noreferrer">如何跨区域使用HSS服务</a>。</p>
</td>
</tr>
<tr id="hss_01_0234_row1715010162495"><td class="cellrowborder" valign="top" width="21.67%" headers="mcps1.2.3.1.1 "><p id="hss_01_0234_p4150716174914"><a name="hss_01_0234_p4150716174914"></a><a name="hss_01_0234_p4150716174914"></a>第三方云主机</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="78.33%" headers="mcps1.2.3.1.2 "><p id="hss_01_0234_p0150616134918"><a name="hss_01_0234_p0150616134918"></a><a name="hss_01_0234_p0150616134918"></a><strong id="hss_01_0234_b17626227101210"><a name="hss_01_0234_b17626227101210"></a><a name="hss_01_0234_b17626227101210"></a>非华为云主机</strong>的安装方式。</p>
<a name="hss_01_0234_ul196058314920"></a><a name="hss_01_0234_ul196058314920"></a><ul id="hss_01_0234_ul196058314920"><li>仅在<span class="parmvalue" id="hss_01_0234_parmvalue1580913141594"><a name="hss_01_0234_parmvalue1580913141594"></a><a name="hss_01_0234_parmvalue1580913141594"></a>“华北-北京一”</span>、<span class="parmvalue" id="hss_01_0234_parmvalue380910148913"><a name="hss_01_0234_parmvalue380910148913"></a><a name="hss_01_0234_parmvalue380910148913"></a>“华东-上海二”</span>、<span class="parmvalue" id="hss_01_0234_parmvalue15813814898"><a name="hss_01_0234_parmvalue15813814898"></a><a name="hss_01_0234_parmvalue15813814898"></a>“华南-广州”</span>、<span class="parmvalue" id="hss_01_0234_parmvalue128132014799"><a name="hss_01_0234_parmvalue128132014799"></a><a name="hss_01_0234_parmvalue128132014799"></a>“华北-北京四”</span>可接入非华为云的主机，请在以上区域内购买防护配额，并使用以上区域内的安装包或安装命令为主机安装客户端。</li><li>在非华为云主机中安装客户端后，在防护列表中，您可以根据主机的IP地址查找该主机。</li></ul>
</td>
</tr>
<tr id="hss_01_0234_row3151181614491"><td class="cellrowborder" valign="top" headers="mcps1.2.3.1.1 "><p id="hss_01_0234_p115112161495"><a name="hss_01_0234_p115112161495"></a><a name="hss_01_0234_p115112161495"></a>线下主机</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-notice.gif) **须知：**   
>-   由于主机的性能差异，非华为云的主机与企业主机安全服务的兼容性可能较差，为使您获得良好的服务体验，建议您使用华为云主机。  
>-   安装客户端时，请暂时清理主机中可能干扰主机安装的应用进程和配置信息，防止客户端安装失败。  

## 前提条件<a name="section145381446145316"></a>

-   待安装客户端的主机已绑定弹性IP。
-   已在本地安装远程管理工具（如：“pcAnywhere“、“UltraVNC“）。

## 操作步骤<a name="section192703820307"></a>

有两种安装方式，以下步骤演示方式一。

-   方式一：下载企业主机安全服务的客户端，上传至待安装客户端的云主机后，在云主机中安装客户端。
-   方式二：登录待安装客户端的云主机，在云主机中登录华为云管理控制台，下载并安装客户端。

1.  [登录管理控制台](https://console.huaweicloud.com)。
2.  在页面上方选择区域后，单击![](figures/icon-servicelist.png)，选择“安全  \>  企业主机安全“。

    **图 1**  企业主机安全<a name="hss_01_0229_fig1271516227232"></a>  
    ![](figures/企业主机安全.png "企业主机安全")

3.  在左侧导航栏中，选择“安装与配置“，进入“安装Agent“界面，下载客户端安装包。

    **图 2**  安装Windows客户端<a name="zh-cn_topic_0167639837_fig98256510550"></a>  
    ![](figures/安装Windows客户端.png "安装Windows客户端")

4.  远程登录待安装客户端的主机。
    -   华为云主机
        -   您可以登录弹性云服务器控制台，在“弹性云服务器“列表中，单击“远程登录“登录主机，详细操作请参见[在云服务器控制台上登录主机](https://support.huaweicloud.com/usermanual-ecs/zh-cn_topic_0027290684.html)。
        -   若您的主机已经绑定了弹性IP，您也可以使用Windows系统的“远程桌面连接“工具，或第三方远程管理工具（例如：“pcAnywhere“、“UltraVNC“）登录主机，并使用管理员账号在主机中安装客户端。

    -   非华为云主机

        请使用Windows系统的“远程桌面连接“工具，或第三方远程管理工具（如：“pcAnywhere“、“UltraVNC“）登录主机，并使用管理员账号在主机中安装客户端。

5.  将客户端安装包上传到待安装客户端的主机中。
6.  使用管理员权限运行客户端安装程序。

    安装客户端时，在主机类型界面，选择主机类型。

    -   华为云主机：请选择“华为云主机”。

        **图 3**  选择主机类型（华为云主机）<a name="zh-cn_topic_0199816002_fig14562154711415"></a>  
        ![](figures/选择主机类型（华为云主机）.png "选择主机类型（华为云主机）")

    -   非华为云主机：请选择“其他云主机”。请从安装Agent界面复制组织ID，如[图5](#zh-cn_topic_0199816002_fig191838428527)所示。

        **图 4**  选择主机类型（非华为云主机）<a name="zh-cn_topic_0199816002_fig661243085110"></a>  
        ![](figures/选择主机类型（非华为云主机）.png "选择主机类型（非华为云主机）")

        **图 5**  获取组织ID（非华为云主机）<a name="zh-cn_topic_0199816002_fig191838428527"></a>  
        ![](figures/获取组织ID（非华为云主机）.png "获取组织ID（非华为云主机）")

7.  安装完成后，在“Windows任务管理器“中查看进程“HostGuard.exe“和“HostWatch.exe“，如[图6](#fig10894450191811)所示。

    若进程不存在，则表示客户端安装失败，请尝试重新安装客户端。

    **图 6**  查看客户端运行状态<a name="fig10894450191811"></a>  
    ![](figures/查看客户端运行状态.png "查看客户端运行状态")


## 相关操作<a name="section982995012508"></a>

-   客户端状态及异常处理的详细操作请参见[客户端状态异常应如何处理？](https://support.huaweicloud.com/hss_faq/hss_01_0036.html)。
-   卸载客户端的详细操作请参见[卸载客户端](https://support.huaweicloud.com/hss_faq/hss_01_0119.html)。

