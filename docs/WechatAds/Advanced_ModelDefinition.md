﻿## 如何快速找到需要调用的 API 模型类名 / 方法名？

---

本库提供的请求模型、响应模型和接口方法，三者均保持同名。

例如，预估覆盖人数的请求是 `EstimationGetRequest`，响应是 `EstimationGetResponse`，接口是 `ExecuteEstimationGetAsync()`。知道其中一个，其余两个就可以快速地推断出了。

再有，每个对象的命名与官方文档的接口地址大体保持一致。例如刚刚提到的预估覆盖人数，它的接口地址是 `[POST] /estimation/get`，将其中的反斜杠去掉、并以大驼峰命名法的方式调整它，就可以得到前文提到的几个对象了。

完整的模型定义可以参考项目目录下的 _src/SKIT.FlurlHttpClient.Wechat.Ads/Models_ 目录。

---

### 找不到所需要的接口或字段？

本库会定期随微信官方更新接口或模型，但也会偶有疏漏。如果你在使用中遇到了因接口或模型定义而产生的问题，欢迎提出 Issue。

如果你的项目来不及等待 Issue 被处理，你可以自行扩展相关 API。

---

### 微信广告平台 API 支持情况：

<details>

<summary>[展开查看]</summary>

|     |    微信 API    | 备注 |
| :-: | :------------: | :--: |
|  √  |  广告帐号模块  |      |
|  √  |  资质管理模块  |      |
|  √  | 服务商权限模块 |      |
|  √  |  资金账户模块  |      |
|  √  |  推广计划模块  |      |
|  √  |   广告组模块   |      |
|  √  |  广告创意模块  |      |
|  √  |    广告模块    |      |
|  √  |    报表模块    |      |
|  √  |  异步任务模块  |      |
|  √  |  图片管理模块  |      |
|  √  |  客户人群管理  |      |
|  √  |    其他模块    |      |

</details>
