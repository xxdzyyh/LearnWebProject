# BugInsight-Web 解读



## 重要的文件

* package.json 项目第三方依赖管理（类似于swift package.swift）

| 工具                  | 配置文件      | 锁定文件          |
| --------------------- | ------------- | ----------------- |
| npm                   | package.json  | package-lock.json |
| cocoapods             | Podfile       | Podfile.lock      |
| Swift Package Manager | package.swift |                   |



### package.json

* scripts 

  定义脚本的缩写

  ```
  {
    "dev": "webpack-dev-server --inline --progress --config build/webpack.dev.conf.js",
    "start": "npm run dev",
    "unit": "jest --config test/unit/jest.conf.js --coverage",
    "test": "npm run unit",
    "lint": "eslint --ext .js,.vue src test/unit",
    "build": "node build/build.js"
  }
  ```

* dependencies

  release 环境需要的依赖

  ```
  "dependencies": {
    "blueimp-md5": "^2.11.0",
    "default-passive-events": "^1.0.10",
    "echarts": "^4.2.1",
    "element-ui": "^2.9.1",
    "node-sass": "^4.14.1",
    "videojs-vjsdownload": "^1.0.4",
    "vue": "^2.5.2",
    "vue-clipboard2": "^0.3.0",
    "vue-resource": "^1.5.1",
    "vue-router": "^3.0.1",
    "vue-video-player": "^5.0.2"
  }
  ```

* devDependencies

  develop 环境需要的依赖

* engines

  ```
  "engines": {
    "node": ">= 6.0.0",
    "npm": ">= 3.0.0"
  }
  ```

* browserslist

  ```
  "browserslist": [
    "> 1%",
    "last 2 versions",
    "not ie <= 8"
  ]
  ```

  

