# 项目目录结构说明

```javascript
-
- api // 模拟数据目录
-   \- [filename].json
- app // 生产环境目录
  |- api
  |    \- [filename].json
  |- resources
  |     |- js
  |     |   |- vendor-[hash].js
  |     |   |- index-[hash].js
  |     |   |- ...
  |     |   \- [id]-[hash].js
  |     |- css
  |     |   |- vendor-[hash].css
  |     |   |- index-[hash].css
  |     |   |- ...
  |     |   \- [id]-[hash].css
  |     \- images
  |         |- ...
  |         |- [filename]-[hash].svg
  |         \- [filename]-[hash].png
  |- index.html     // 登录后首页（单页应用主体）
  \- favicon.ico
- src // 开发环境目录
  |- components // 展示组件目录
  |     |- Icon
  |     |- Button
  |     |- ...
  |     \- Index
  |         |- js
  |         |   \- Index.js
  |         |- less
  |         |   \- index.less
  |         \- images
  |             |- ...
  |             |- [filename].svg
  |             \- [filename].png
  |- containers // 容器组件目录
  |     |- ...
  |     |- App.js
  |     \- Index.js
  |- reducers // Redux（规则）定义目录 - 负责接收、处理 action，返回新的 state
  |     |- ...
  |     \- index.js // 根 Reducer
  |- actions // Redux（动作）定义目录 - 定义 action 及需要携带的数据
  |     \- ...
  |- sagas  // 业务逻辑代码目录 - 负责协调异步操作的目录
  |     |- ...
  |     \- index.js // 根 Sagas
  |- store  // 数据存储目录
  |     |- initialState.js
  |     \- configureStore.js // 应用程序 Store 配置文件
  |- utils  // 实用工具
  |     |- FL.js
  |     |- interceptor.js
  |     |- localStorage.js
  |     \- auth.js
  |- index.js // 应用程序根（混合展示组件、容器组件、Store、API）
  |- index.ejs // HTML 文件模板
  \- favicon.ico
```
