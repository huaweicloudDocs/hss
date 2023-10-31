# HSS自定义策略<a name="hss_01_0005"></a>

如果系统预置的HSS权限，不满足您的授权要求，可以创建自定义策略。自定义策略中可以添加的授权项（Action）请参见[HSS授权项说明](HSS授权项说明.md)_。_

目前华为云支持以下两种方式创建自定义策略：

-   可视化视图创建自定义策略：无需了解策略语法，按可视化视图导航栏选择云服务、操作、资源、条件等策略内容，可自动生成策略。
-   JSON视图创建自定义策略：可以在选择策略模板后，根据具体需求编辑策略内容；也可以直接在编辑框内编写JSON格式的策略内容。

具体创建步骤请参见：[创建自定义策略](https://support.huaweicloud.com/usermanual-iam/iam_01_0605.html)。本章为您介绍常用的HSS自定义策略样例。

## HSS自定义策略样例<a name="section8786220155718"></a>

-   示例1：授权用户查询主机防护列表

    ```
    {
            "Version": "1.1",
            "Statement": [
                    {
                            "Effect": "Allow",
                            "Action": [
                                    "hss:hosts:list"
                                                           ]
                    }
            ]
    }
    ```

-   示例2：拒绝用户卸载Agent

    拒绝策略需要同时配合其他策略使用，否则没有实际作用。用户被授予的策略中，一个授权项的作用如果同时存在Allow和Deny，则遵循Deny优先。

    如果您给用户授予“HSS Administrator“的系统策略，但不希望用户拥有“HSS Administrator“中定义的卸载Agent的权限（hss:agent:uninstall），您可以创建一条相同Action的自定义策略，并将自定义策略的Effect设置为“Deny“，然后同时将“HSS Administrator“和拒绝策略授予用户，根据Deny优先原则用户可以对HSS执行除了卸载Agent的所有操作。以下策略样例表示：拒绝用户卸载Agent。

    ```
    {
            "Version": "1.1",
            "Statement": [
                    {
                            "Effect": "Deny",
                            "Action": [
                                    "hss:agent:uninstall"                                
                            ]
                    },
            ]
    }
    ```

-   多个授权项策略

    一个自定义策略中可以包含多个授权项，且除了可以包含本服务的授权项外，还可以包含其他服务的授权项，可以包含的其他服务必须跟本服务同属性，即都是项目级服务。多个授权语句策略描述如下：

    ```
    {
            "Version": "1.1",
            "Statement": [
                    {
                            "Effect": "Allow",
                            "Action": [
                                    "hss:hosts:list"
                            ]
                    },
                   {
                            "Effect": "Allow",
                            "Action": [
                                    "hss:hosts:switchVersion",
                                    "hss:hosts:manualDetect",
                                    "hss:manualDetectStatus:get"
                            ]
                    }
            ]
    }
    ```

