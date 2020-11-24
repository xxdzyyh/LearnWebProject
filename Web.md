# Web

* HTML 定义了网页的内容

* CSS    描述了网页的布局

* JavaScript  网页的行为




| Web     | iOS                             | 描述           |      |
| ------- | ------------------------------- | -------------- | ---- |
| npm     | Cocoapods/Swift Package Manager | 第三方依赖管理 |      |
| webpack | Xcode                           | 打包工具       |      |
|         |                                 |                |      |
|         |                                 |                |      |
|         |                                 |                |      |
|         |                                 |                |      |
|         |                                 |                |      |
|         |                                 |                |      |
|         |                                 |                |      |

### webpack

webpack 是一个打包工具，相当于实现了iOS 代码到 IPA 这一步。 默认将项目代码编译为类浏览器环境里可用。

webpack 也有target的概念，可以为不同的环境（dev,release）创建多个target

webpack 的 source map 就类似于 iOS 的符号表。source map 的配置就类似于符号表的配置。



```
// 注意整个配置中我们使用 Node 内置的 path 模块，并在它前面加上 __dirname这个全局变量。
// 可以防止不同操作系统之间的文件路径问题，并且可以使相对路径按照预期工作。
const path = require('path');



```

