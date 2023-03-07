﻿## 如何快速找到需要调用的 API 模型类名 / 方法名？

---

本库提供的请求模型、响应模型和接口方法，三者均保持同名。

例如，创建标签组的请求是 `AppCreateTagRequest`，响应是 `AppCreateTagResponse`，接口是 `ExecuteAppCreateTagAsync()`。知道其中一个，其余两个就可以快速地推断出了。

再有，每个对象的命名与官方文档的接口地址大体保持一致。例如刚刚提到的创建标签组，它的接口地址是 `[POST] /app/create_tag`，将其中的反斜杠去掉、并以大驼峰命名法的方式调整它，就可以得到前文提到的几个对象了。

完整的模型定义可以参考项目目录下的 _src/SKIT.FlurlHttpClient.Baidu.Push/Models_ 目录。
