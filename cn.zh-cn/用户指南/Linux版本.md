# Linux版本<a name="hss_01_0234"></a>

安装Agent后，您才能开启企业主机安全服务。通过本节介绍，您将了解如何在Linux操作系统的主机中安装Agent。Windows操作系统的Agent安装请参见[Windows版本](Windows版本.md)。

>![](public_sys-resources/icon-note.gif) **说明：** 
>网页防篡改与主机安全共用同一个Agent，您只需在同一主机安装一次。

## 前提条件<a name="section18581100219"></a>

-   待安装Agent所在的线下主机必须绑定弹性IP。
-   待安装Agent所在的线上主机需要与网段相通，要求您的服务器安全组出方向的设置允许访问**100.125.0.0/16**网段的**443**端口。
-   已在本地安装远程管理工具（如：“Xftp“、“SecureFX“、“WinSCP“）。
-   请关闭Selinux防火墙，防止Agent安装失败，安装成功后再打开。

## 约束与限制<a name="section79811406183"></a>

-   **华为云主机**

    主机与HSS必须在**同一区域**，并使用配额所在区域的安装命令或安装包为主机安装Agent，否则会导致HSS Agen**安装失败**。若主机与HSS配额不在同一区域，请退订重新购买主机所在区域的配额。

-   **非华为云主机**
    -   当前仅“华北-北京一“、“华东-上海二“、“华南-广州“、“华北-北京四“可接入非华为云的主机，请在以上区域内购买防护配额，并使用以上区域内的安装包或安装命令为主机安装Agent。
    -   非华为云主机需要能通过**公网IP**访问华为云，才能接入HSS。安装Agent后，在防护列表中，您可以根据主机的IP地址查找该主机。

        >![](public_sys-resources/icon-notice.gif) **须知：** 
        >-   由于主机的性能差异，非华为云的主机与企业主机安全服务的兼容性可能较差，为使您获得良好的服务体验，建议您使用华为云主机。
        >-   安装Agent时，请暂时清理主机中可能干扰主机安装的应用进程和配置信息（例，McAfee软件、360安全卫士、腾讯管家等第三方安全防护软件），防止Agent安装失败。



## 系统影响<a name="section33281913112120"></a>

安装HSS Agent 对主机没有任何影响。HSS Agent用于执行检测任务，全量扫描主机；实时监测主机的安全状态，并将收集的主机信息上报给云端防护中心。未安装Agent插件的主机将不受HSS保护，控制台页面也不会显示该主机资产的任何系统漏洞、基线风险、入侵事件和安全报告等数据。

## 默认安装路径<a name="section1587918461017"></a>

在Linux操作系统的主机中安装Agent时，安装过程中不提供安装路径的选择，默认安装在以下路径中：

“/usr/local/hostguard/“

## 使用安装命令安装<a name="section1831315205214"></a>

登录待安装Agent的云主机，使用安装命令在线安装Agent。安装成功后，Agent不会立即生效，需要等待3\~5分钟左右控制台才会刷新。

1.  [登录管理控制台](https://console.huaweicloud.com)。
2.  在页面左上角选择“区域“，单击![](figures/icon-servicelist.png)，选择“安全与合规  \>  企业主机安全“，进入企业主机安全页面。

    **图 1**  企业主机安全<a name="hss_01_0229_fig65591238182410"></a>  
    ![](figures/企业主机安全.png "企业主机安全")

3.  在左侧导航栏中，选择“安装与配置“，进入“安装Agent“界面，复制安装Agent的命令。

    **图 2**  复制安装Agent的命令<a name="fig2320121019118"></a>  
    ![](figures/复制安装Agent的命令.png "复制安装Agent的命令")

4.  远程登录待安装Agent的主机。
    -   华为云主机
        -   您可以登录弹性云服务器控制台，在“弹性云服务器“列表中，单击“远程登录“登录主机，详细操作请参见[在云服务器控制台上登录主机](https://support.huaweicloud.com/usermanual-ecs/ecs_03_0136.html)。
        -   若您的主机已经绑定了弹性IP，您也可以使用远程管理工具（例如：“Xftp“、“SecureFX“、“WinSCP“）登录主机，并使用root帐号在主机中安装Agent。

    -   非华为云主机

        请使用远程管理工具（例如：“Xftp“、“SecureFX“、“WinSCP“）登录主机，并使用root帐号在主机中安装Agent。

5.  粘贴复制的安装命令，并按“Enter“，在主机中安装Agent。

    若界面回显信息与如下信息类似，则表示Agent安装成功。

    ```
    Preparing...                  ########################## [100%]
    1:hostguard                   ########################## [100%]
    Hostguard is running.
    Hostguard installed.
    ```

6.  使用**service hostguard** **status**命令，查看Agent的运行状态。

    若界面回显如下信息，则表示Agent服务运行正常。

    ```
    Hostguard is running
    ```

    安装成功后，Agent不会立即生效，需要等待3\~5分钟左右控制台才会刷新。


## 使用安装包安装（仅华为云主机支持）<a name="section2429194215320"></a>

下载企业主机安全服务的Agent软件，上传至待安装Agent的云主机后，在云主机中使用安装命令安装Agent。

1.  [登录管理控制台](https://console.huaweicloud.com)。
2.  在左侧导航栏中，选择“安装与配置“，进入“安装Agent“界面，下载Agent安装包。

    **图 3**  下载Agent安装包<a name="fig88946474"></a>  
    ![](figures/下载Agent安装包.png "下载Agent安装包")

3.  在弹出的对话框中，根据待安装Agent的云服务器操作系统版本，下载所需安装的Agent。
4.  使用文件传输工具（例如：“Xftp“、“SecureFX“、“WinSCP“），将下载的Agent安装包上传至云主机。
5.  远程登录待安装Agent的主机。
    -   您可以登录弹性云服务器控制台，在“弹性云服务器“列表中，单击“远程登录“登录主机，详细操作请参见[在云服务器控制台上登录主机](https://support.huaweicloud.com/usermanual-ecs/ecs_03_0136.html)。
    -   若您的主机已经绑定了弹性IP，您也可以使用远程管理工具（例如：“Xftp“、“SecureFX“、“WinSCP“）登录主机，并使用root帐号在主机中安装Agent。

6.  使用**cd** _安装包所在目录_命令，进入安装包所在目录。
7.  使用如下命令，在云主机中安装Agent。
    -   安装“.rpm“格式的安装包，请执行命令：**rpm** **-ivh** _安装包名称_。

        >![](public_sys-resources/icon-note.gif) **说明：** 
        >强制安装请执行命令：**rpm** **-ivh --force** _安装包名称_

    -   安装“.deb“格式的安装包，请执行命令：**dpkg** **-i** _安装包名称_。

        若界面回显信息与如下信息类似，则表示Agent安装成功。

        ```
        Preparing...                  ########################## [100%]
        1:hostguard                   ########################## [100%]
        Hostguard is running.
        Hostguard installed.
        ```

8.  使用**service hostguard** **status**命令，查看Agent的运行状态。

    若界面回显如下信息，则表示Agent服务运行正常。

    ```
    Hostguard is running
    ```

    安装成功后，Agent不会立即生效，需要等待3\~5分钟左右控制台才会刷新。


## 相关操作<a name="section982995012508"></a>

-   Agent状态及异常处理的详细操作请参见[Agent状态异常应如何处理？](https://support.huaweicloud.com/hss_faq/hss_01_0036.html)
-   Agent安装失败，请参见[Agent安装失败应如何处理？](https://support.huaweicloud.com/hss_faq/hss_01_0069.html)
-   卸载Agent的详细操作请参见[如何卸载Agent？](https://support.huaweicloud.com/hss_faq/hss_01_0119.html)

