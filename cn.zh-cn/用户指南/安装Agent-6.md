# 安装Agent<a name="hss_01_0375"></a>

指导您在console对目标服务器安装Agent，Agent安装后HSS才能对服务器进行正常检测和防护。

## 安装须知<a name="section917743414517"></a>

-   Agent支持的操作系统请参见[支持的操作系统](https://support.huaweicloud.com/productdesc-hss2.0/hss_01_0137.html#section2)。

-   由于主机的性能差异，非华为云的主机与主机安全服务的兼容性可能较差，为使您获得良好的服务体验，建议您使用华为云主机。
-   Windows主机需要配置华为云内网DNS地址后才能下载Agent，DNS详情请参见[华为云的内网DNS](https://support.huaweicloud.com/zh-cn/dns_faq/dns_faq_002.html)。

-   如果您的服务器已安装第三方安全软件，可能会导致主机安全服务Agent无法正常安装，请您关闭或卸载第三方安全软件后再安装Agent。
-   安装Agent的磁盘剩余可用容量须大于300M，否则可能导致Agent安装失败。
-   安装成功后，需要等待5\~10分钟左右才会刷新Agent状态。请前往“资产管理\>主机管理\>云服务器”界面查看。

## 单服务器安装Agent<a name="section15535315577"></a>

1.  [登录管理控制台](https://console.huaweicloud.com/?locale=zh-cn)。
2.  在页面左上角选择“区域“，单击![](figures/zh-cn_image_0000001517317834.png)，选择“安全与合规 \> 主机安全服务”，进入主机安全平台界面。

    **图 1**  进入主机安全<a name="hss_01_0234_fig1855613765114"></a>  
    ![](figures/进入主机安全.png "进入主机安全")

3.  在左侧导航树选择“安装与配置  \>  Agent 管理“，进入Agent管理页面。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果您的服务器已通过企业项目的模式进行管理，您可选择目标“企业项目“后查看或操作目标企业项目内的资产和检测信息。

    **图 2**  进入Agent管理<a name="hss_01_0374_fig43639934816"></a>  
    ![](figures/进入Agent管理.png "进入Agent管理")

4.  选择“Agent不在线（X）“，查看Agent未安装或离线的服务器列表，详情请参见[表1](#table1926618704616)。

    **表 1**  Agent不在线列表参数说明

    <a name="table1926618704616"></a>
    <table><thead align="left"><tr id="row16266127154611"><th class="cellrowborder" valign="top" width="14.66%" id="mcps1.2.3.1.1"><p id="p9266375468"><a name="p9266375468"></a><a name="p9266375468"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="85.34%" id="mcps1.2.3.1.2"><p id="p22662074462"><a name="p22662074462"></a><a name="p22662074462"></a>参数说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1226617104612"><td class="cellrowborder" valign="top" width="14.66%" headers="mcps1.2.3.1.1 "><p id="p15266147134619"><a name="p15266147134619"></a><a name="p15266147134619"></a>服务器名称/ID</p>
    </td>
    <td class="cellrowborder" valign="top" width="85.34%" headers="mcps1.2.3.1.2 "><p id="p6266167144612"><a name="p6266167144612"></a><a name="p6266167144612"></a>服务器的名称和ID。</p>
    </td>
    </tr>
    <tr id="row12661472469"><td class="cellrowborder" valign="top" width="14.66%" headers="mcps1.2.3.1.1 "><p id="p92662074464"><a name="p92662074464"></a><a name="p92662074464"></a>IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="85.34%" headers="mcps1.2.3.1.2 "><p id="p67691716205414"><a name="p67691716205414"></a><a name="p67691716205414"></a>目标服务器所属的公网IP或私网IP。</p>
    </td>
    </tr>
    <tr id="row112663754616"><td class="cellrowborder" valign="top" width="14.66%" headers="mcps1.2.3.1.1 "><p id="p326612711468"><a name="p326612711468"></a><a name="p326612711468"></a>操作系统</p>
    </td>
    <td class="cellrowborder" valign="top" width="85.34%" headers="mcps1.2.3.1.2 "><p id="p1266137164620"><a name="p1266137164620"></a><a name="p1266137164620"></a>目标服务器的操作系统。</p>
    <a name="ul7230182265511"></a><a name="ul7230182265511"></a><ul id="ul7230182265511"><li>linux</li><li>windows</li></ul>
    </td>
    </tr>
    <tr id="row5266673467"><td class="cellrowborder" valign="top" width="14.66%" headers="mcps1.2.3.1.1 "><p id="p32666794619"><a name="p32666794619"></a><a name="p32666794619"></a>Agent状态</p>
    </td>
    <td class="cellrowborder" valign="top" width="85.34%" headers="mcps1.2.3.1.2 "><p id="p426667194615"><a name="p426667194615"></a><a name="p426667194615"></a>目标服务器的Agent状态。</p>
    <a name="ul6395135214554"></a><a name="ul6395135214554"></a><ul id="ul6395135214554"><li>离线</li><li>未安装</li><li>安装失败</li></ul>
    </td>
    </tr>
    <tr id="row9213131511111"><td class="cellrowborder" valign="top" width="14.66%" headers="mcps1.2.3.1.1 "><p id="p1429412312595"><a name="p1429412312595"></a><a name="p1429412312595"></a>Agent版本</p>
    </td>
    <td class="cellrowborder" valign="top" width="85.34%" headers="mcps1.2.3.1.2 "><p id="p8295123175919"><a name="p8295123175919"></a><a name="p8295123175919"></a>目标服务器当前安装的Agent版本。</p>
    </td>
    </tr>
    <tr id="row10871181720112"><td class="cellrowborder" valign="top" width="14.66%" headers="mcps1.2.3.1.1 "><p id="p157841125135918"><a name="p157841125135918"></a><a name="p157841125135918"></a>Agent升级状态</p>
    </td>
    <td class="cellrowborder" valign="top" width="85.34%" headers="mcps1.2.3.1.2 "><p id="p15784132505914"><a name="p15784132505914"></a><a name="p15784132505914"></a>目标服务器在Agent升级过程中的状态。</p>
    </td>
    </tr>
    </tbody>
    </table>

5.  单击目标服务器“操作“列的“离线原因“，查看目标服务器Agent离线原因。
6.  单击目标服务器“操作“列的“安装Agent“，选择不同架构以及不同系统的链接进行下载安装，linux系统安装详情请参见[安装Linux版本Agent](安装Linux版本Agent.md)，windows系统安装详情请参见[安装Windows版本Agent](安装Windows版本Agent.md)。

## 批量安装Agent（服务器账号、密码不同）<a name="section15707112131411"></a>

您可对不同账号密码的多台服务器进行批量安装。

**约束限制**

-   Agent支持的操作系统请参见[支持的操作系统](https://support.huaweicloud.com/productdesc-hss2.0/hss_01_0137.html#section2)。
-   目前仅支持华为云上Linux系统的服务器进行不同账号密码的Agent批量安装。
-   批量安装Agent的服务器在同一安全组或能连接的安全组。

**前提条件**

-   批量安装的所有服务器需要支持ssh登录。
-   批量安装的所有服务器需要提供正确的登录账号、端口、密码。
-   批量安装的主机“服务器状态“必须为“运行中“。

**操作步骤**

1.  [登录管理控制台](https://console.huaweicloud.com/?locale=zh-cn)。
2.  在页面左上角选择“区域“，单击![](figures/zh-cn_image_0000001517477402.png)，选择“安全与合规 \> 主机安全服务”，进入主机安全服务界面。

    **图 3**  进入主机安全服务<a name="fig103496184718"></a>  
    ![](figures/进入主机安全服务-46.png "进入主机安全服务-46")

3.  在左侧导航树选择“安装与配置  \>  Agent 管理“，进入Agent管理页面。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果您的服务器已通过企业项目的模式进行管理，您可选择目标“企业项目“后查看或操作目标企业项目内的资产和检测信息。

    **图 4**  进入Agent管理<a name="hss_01_0374_fig43639934816_1"></a>  
    ![](figures/进入Agent管理.png "进入Agent管理")

4.  单击“Agent安装指南“，复制“批量安装“的命令。

    **图 5**  复制批量安装命令<a name="fig19982162414342"></a>  
    ![](figures/复制批量安装命令.png "复制批量安装命令")

5.  远程登录待安装Agent的华为云主机。

    您可以登录弹性云服务器控制台，在“弹性云服务器“列表中，单击“远程登录“登录主机，详细操作请参见[在云服务器控制台上登录主机](https://support.huaweicloud.com/usermanual-ecs/ecs_03_0136.html)。

    >![](public_sys-resources/icon-notice.gif) **须知：** 
    >登录服务器后先执行以下命令检查服务器是否具备expect命令，若不具备需配置yum源。
    >/bin/expect -v

6.  执行以下命令进入tmp目录。

    cd /tmp/

7.  按照以下命令格式执行命令，创建文件linux-host-list.txt并将需要批量安装的节点私有ip添加至创建的文件中。

    命令格式：echo "IP地址 端口 root rootPassword" \>\> linux-host-list.txt

    或echo "IP地址 端口 user userPassword rootPassword" \>\> linux-host-list.txt

    示例：echo "127.8.10.8 22 root rootPassword" \>\> linux-host-list.txt

    或echo "127.8.10.9 22 user userPassword rootPassword" \>\> linux-host-list.txt

    若存在多个不同IP，则不同IP的命令之间用换行符隔开。

    示例：echo "127.8.10.1 22 root rootPassword" \>\> linux-host-list.txt

    echo "127.8.10.8 22 user userPassword rootPassword" \>\> linux-host-list.txt

    echo "127.8.10.3 22 root rootPassword" \>\> linux-host-list.txt

8.  键入回车保存IP，执行命令cat linux-host-list.txt查询是否添加完成。
9.  粘贴复制的安装命令，以root权限执行，在主机中安装Agent。

    若界面回显如下信息，则表示Agent安装成功。

    remote\_install finished. \[OK\]

10. 安装成功后可在“安装与配置  \>  Agent管理  \>  Agent在线“页面查看目标服务器的“Agent状态“为“在线“，表示Agent服务运行正常。

