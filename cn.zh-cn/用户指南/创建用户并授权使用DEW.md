# 创建用户并授权使用DEW<a name="dew_01_0135"></a>

本章节通过简单的用户组授权方法，将DEW的策略授予用户组，并将用户添加至用户组中，从而使用户拥有对应的DEW权限，操作流程如[图1](#fig392404973213)所示。

**图 1**  给用户授权DEW权限流程<a name="fig392404973213"></a>  
![](figures/给用户授权DEW权限流程.png "给用户授权DEW权限流程")

1.  <a name="li8135822590"></a>创建用户组并授权。

    在IAM控制台创建用户组，并授予数据加密服务的管理员权限“KMS Administrator“。

2.  创建用户。

    在IAM控制台创建用户，并将其加入[1](#li8135822590)中创建的用户组。

3.  用户登录并验证权限。

    新创建的用户登录控制台，验证数据加密服务的管理员权限。


## 前提条件<a name="section5211203911259"></a>

给用户组授权之前，请您了解用户组可以添加的DEW系统策略，并结合实际需求进行选择，DEW系统策略如[表1](#table1574195286)所示。若您需要对除DEW之外的其它服务授权，IAM支持服务的所有策略请参见[权限策略](https://support.huaweicloud.com/usermanual-permissions/zh-cn_topic_0063498930.html)。

**表 1**  DEW系统策略

<a name="table1574195286"></a>
<table><thead align="left"><tr id="zh-cn_topic_0169425412_row1346222921318"><th class="cellrowborder" valign="top" width="27.69276927692769%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0169425412_p246217292138"><a name="zh-cn_topic_0169425412_p246217292138"></a><a name="zh-cn_topic_0169425412_p246217292138"></a>策略名称</p>
</th>
<th class="cellrowborder" valign="top" width="35.32353235323533%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0169425412_p146292918139"><a name="zh-cn_topic_0169425412_p146292918139"></a><a name="zh-cn_topic_0169425412_p146292918139"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="16.711671167116712%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0169425412_p3459112418415"><a name="zh-cn_topic_0169425412_p3459112418415"></a><a name="zh-cn_topic_0169425412_p3459112418415"></a>策略类别</p>
</th>
<th class="cellrowborder" valign="top" width="20.27202720272027%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0169425412_p446218291138"><a name="zh-cn_topic_0169425412_p446218291138"></a><a name="zh-cn_topic_0169425412_p446218291138"></a>依赖关系</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0169425412_row1462142915137"><td class="cellrowborder" valign="top" width="27.69276927692769%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0169425412_p25241140125910"><a name="zh-cn_topic_0169425412_p25241140125910"></a><a name="zh-cn_topic_0169425412_p25241140125910"></a>KMS Administrator</p>
</td>
<td class="cellrowborder" valign="top" width="35.32353235323533%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0169425412_p0462172991319"><a name="zh-cn_topic_0169425412_p0462172991319"></a><a name="zh-cn_topic_0169425412_p0462172991319"></a>数据加密服务的管理员权限。</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0169425412_p134591224104113"><a name="zh-cn_topic_0169425412_p134591224104113"></a><a name="zh-cn_topic_0169425412_p134591224104113"></a>RBAC策略</p>
</td>
<td class="cellrowborder" valign="top" width="20.27202720272027%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0169425412_p446222915139"><a name="zh-cn_topic_0169425412_p446222915139"></a><a name="zh-cn_topic_0169425412_p446222915139"></a>无。</p>
</td>
</tr>
<tr id="zh-cn_topic_0169425412_row4708123532810"><td class="cellrowborder" valign="top" width="27.69276927692769%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0169425412_p07090356289"><a name="zh-cn_topic_0169425412_p07090356289"></a><a name="zh-cn_topic_0169425412_p07090356289"></a>KMS CMK Admin</p>
</td>
<td class="cellrowborder" valign="top" width="35.32353235323533%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0169425412_p12709103592818"><a name="zh-cn_topic_0169425412_p12709103592818"></a><a name="zh-cn_topic_0169425412_p12709103592818"></a>数据加密服务加密密钥所有权限。</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0169425412_p1170963517284"><a name="zh-cn_topic_0169425412_p1170963517284"></a><a name="zh-cn_topic_0169425412_p1170963517284"></a>细粒度策略</p>
</td>
<td class="cellrowborder" valign="top" width="20.27202720272027%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0169425412_p1470993562816"><a name="zh-cn_topic_0169425412_p1470993562816"></a><a name="zh-cn_topic_0169425412_p1470993562816"></a>无。</p>
</td>
</tr>
<tr id="zh-cn_topic_0169425412_row13720637112819"><td class="cellrowborder" valign="top" width="27.69276927692769%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0169425412_p17720123792815"><a name="zh-cn_topic_0169425412_p17720123792815"></a><a name="zh-cn_topic_0169425412_p17720123792815"></a>DEW Keypair Admin</p>
</td>
<td class="cellrowborder" valign="top" width="35.32353235323533%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0169425412_p1872023712815"><a name="zh-cn_topic_0169425412_p1872023712815"></a><a name="zh-cn_topic_0169425412_p1872023712815"></a>数据加密服务密钥对所有权限。</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0169425412_p772133712819"><a name="zh-cn_topic_0169425412_p772133712819"></a><a name="zh-cn_topic_0169425412_p772133712819"></a>细粒度策略</p>
</td>
<td class="cellrowborder" valign="top" width="20.27202720272027%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0169425412_p2072153711280"><a name="zh-cn_topic_0169425412_p2072153711280"></a><a name="zh-cn_topic_0169425412_p2072153711280"></a>无。</p>
</td>
</tr>
<tr id="zh-cn_topic_0169425412_row43641644115114"><td class="cellrowborder" valign="top" width="27.69276927692769%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0169425412_p4365104445120"><a name="zh-cn_topic_0169425412_p4365104445120"></a><a name="zh-cn_topic_0169425412_p4365104445120"></a>DEW Keypair Viewer</p>
</td>
<td class="cellrowborder" valign="top" width="35.32353235323533%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0169425412_p19365194475114"><a name="zh-cn_topic_0169425412_p19365194475114"></a><a name="zh-cn_topic_0169425412_p19365194475114"></a>数据加密服务密钥对查看权限。</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0169425412_p6776131716526"><a name="zh-cn_topic_0169425412_p6776131716526"></a><a name="zh-cn_topic_0169425412_p6776131716526"></a>细粒度策略</p>
</td>
<td class="cellrowborder" valign="top" width="20.27202720272027%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0169425412_p877621719521"><a name="zh-cn_topic_0169425412_p877621719521"></a><a name="zh-cn_topic_0169425412_p877621719521"></a>无。</p>
</td>
</tr>
</tbody>
</table>

## 步骤1：创建用户组并授权<a name="section3220739152517"></a>

用户组是用户的集合，IAM通过用户组功能实现用户的授权。您在IAM中创建的用户，需要加入特定用户组后，用户才具备用户组所拥有的权限。关于创建用户组并给用户组授权的方法，可以参考如下操作。

1.  使用注册的华为云账号登录华为云，登录时请选择“账号登录“。

    **图 2**  账号登录<a name="zh-cn_topic_0154973652_fig184406496424"></a>  
    ![](figures/账号登录-1.png "账号登录-1")

2.  进入华为云控制台，控制台页面中单击右上角的用户名，选择“统一身份认证“。

    **图 3**  服务选择<a name="fig192441010165114"></a>  
    ![](figures/服务选择.png "服务选择")

3.  在统一身份认证服务的左侧导航空格中，单击“用户组  \>  创建用户组“。

    **图 4**  创建用户组<a name="fig135481549125111"></a>  
    ![](figures/创建用户组.png "创建用户组")

4.  在“创建用户组“界面，输入“用户组名称“，以“data“为例，单击“确定“。

    用户组创建完成，界面自动返回用户组列表，列表中显示新建的用户组。

5.  单击新建用户组“data“右侧的“权限配置“。

    **图 5**  权限配置<a name="fig918317195211"></a>  
    ![](figures/权限配置.png "权限配置")

6.  在“用户组权限“页签中，单击列表左上方的“配置权限“。

    **图 6**  配置权限<a name="fig124391145132312"></a>  
    ![](figures/配置权限.png "配置权限")

7.  IAM提供“策略视图“和“项目视图“两种权限配置方式，两种方式产生的授权效果相同，请根据您的需求选择合适的方式。

    DEW为项目级服务，请确认用户需要使用DEW资源的项目，在对应项目中设置权限。设置完成后用户仅能访问授权项目中的DEW资源，无法访问其他项目中的DEW资源。

    -   策略视图：您可以为一个策略同时配置多个项目。
        1.  在右侧滑窗中，选中“策略视图“；在搜索框中搜索“KMS“，选择“KMS CMK Admin“为例；在已勾选策略的“项目\[作用范围\]“下拉框中，选择需要给该策略授权的项目（可选择多个项目）。DEW的系统策略说明，请参见：[DEW系统策略](https://support.huaweicloud.com/productdesc-dew/dew_01_0018.html#section0)。

            **图 7**  选择项目<a name="fig1137115416494"></a>  
            ![](figures/选择项目.png "选择项目")

        2.  单击“确定“，完成用户组授权。

    -   项目视图：您可以为一个项目同时配置多个策略。
        1.  在右侧滑窗中，单击“项目视图“；选择需要授权的“项目\[作用范围\]“，单击右侧的“选择策略“。

            **图 8**  选择项目视图<a name="fig174066518293"></a>  
            ![](figures/选择项目视图.png "选择项目视图")

        2.  在“选择策略“弹窗中，搜索“KMS“，选择“KMS CMK Admin“为例；DEW的系统策略说明，请参见：[DEW系统策略](https://support.huaweicloud.com/productdesc-dew/dew_01_0018.html#section0)。

            **图 9**  选择策略<a name="fig55971385018"></a>  
            ![](figures/选择策略.png "选择策略")

        3.  单击“确定“，完成用户组授权。



## 步骤2：创建IAM用户<a name="section1222415393250"></a>

IAM用户与企业中的实际员工或是应用程序相对应，有唯一的安全凭证，可以通过加入一个或多个用户组来获得用户组的权限。关于IAM用户的创建方式请参见如下步骤。

1.  在统一身份认证服务，左侧导航中，单击“用户  \>  创建用户“。
2.  在“创建用户“界面中填写“用户信息“。如需一次创建多个用户，可以单击“添加用户“进行批量创建，每次最多可创建10个用户。

    **图 10**  用户信息<a name="fig233618408535"></a>  
    ![](figures/用户信息.png "用户信息")

    -   用户名：用户登录华为云的用户名，以“James“为例。
    -   邮箱：IAM用户绑定的邮箱，仅“访问方式“选择“首次登录时设置“时必填，选择其他访问方式时选填。
    -   手机号（选填）：IAM用户绑定的手机号。
    -   描述（可选）：对用户的描述信息。

3.  在“创建用户“页面选择“访问方式“，完成后单击“下一步“。

    **图 11**  访问方式<a name="fig558915354115"></a>  
    ![](figures/访问方式.png "访问方式")

    -   编程访问：创建用户完成后即可下载本次创建的所有用户的[访问密钥](https://support.huaweicloud.com/usermanual-ca/zh-cn_topic_0046606340.html)。
    -   华为云管理控制台访问：用户可以使用账号密码登录到华为云管理控制台。
        -   控制台登录密码设置方式：当一次创建多个用户时，密码设置方式可选择“首次登录时设置“和“自定义“，不支持“自动生成“密码；当仅创建一个用户时，以上方式均可选择。
        -   登录保护：为了您的账号安全，建议选择“开启登录保护“。后续如需开启或关闭登录保护，请参见：[登录保护](https://support.huaweicloud.com/usermanual-iam/zh-cn_topic_0079477316.html)。

4.  （可选）将用户加入到用户组，完成后单击“下一步“。
    -   选择新创建的用户组“data“。将用户加入用户组，用户将具备用户组的权限，这一过程即给该用户授权。其中“admin“为系统缺省提供的用户组，具有管理人员以及所有云服务资源的操作权限。
    -   如需创建新的用户组，可单击“创建用户组“，填写用户组名称和描述（可选），创建成功后即可将用户加入到新创建的用户组中。

5.  IAM用户创建成功，用户列表中显示新创建的IAM用户。如果在访问方式中勾选了“编程访问“，可在此页面下载访问密钥，后续也可以在“我的凭证“中[管理访问密钥](https://support.huaweicloud.com/usermanual-ca/zh-cn_topic_0046606340.html)。

    **图 12**  创建成功<a name="fig12238144920189"></a>  
    ![](figures/创建成功.png "创建成功")


## 步骤3：用户登录并验证权限<a name="section12483530738"></a>

用户创建完成后，可以使用新用户的用户名及身份凭证登录华为云验证权限，即“KMS CMK Admin“权限。更多用户登录方法请参见[用户登录华为云方法](https://support.huaweicloud.com/qs-iam/iam_01_0031.html#section2)。

1.  在华为云登录页面，单击右下角的“IAM用户登录“。

    **图 13**  IAM用户登录<a name="fig8273258155316"></a>  
    ![](figures/IAM用户登录-2.png "IAM用户登录-2")

2.  在“IAM用户登录“页面，输入账号名、用户名及用户密码，使用新创建的用户登录。

    -   账号名为该IAM用户所属华为云账号的名称。
    -   用户名和密码为账号在IAM创建用户时输入的用户名和密码。

    如果登录失败，您可以联系您的账号主体，确认用户名及密码是否正确，或是重置用户名及密码，重置方法请参见：[忘记IAM用户密码](https://support.huaweicloud.com/iam_faq/iam_01_0314.html#section1)。

3.  登录成功后，进入华为云控制台，请先切换至授权区域“华东-上海二“。

    **图 14**  区域选择<a name="fig1888720620543"></a>  
    ![](figures/区域选择.png "区域选择")

4.  在“服务列表“中选择数据加密服务，进入DEW主界面，选择密钥对管理，若提示权限不足，表示“KMS CMK Admin“已生效。
5.  在“服务列表“中选择除数据加密服务外的任一服务，若提示权限不足，表示“KMS CMK Admin“已生效。

