# Element

> eleme components

## 开发规范

- 目录名即为组件名，使用 `build` 命令将遵循 UMD 规范打包。
- 该仓库内的组件均为可复用的最低级“零件”，即不依赖其它组件。
- 尽量通过 `props` 接收外部数据，但这并不代表禁止使用 `$broadcast` 和 `$dispatch`。
- 尽量指定 `props` 的类型并提供默认值。
- 默认 `props` 传参为单向，即禁止在子组件内部直接修改父组件的状态。
- 组件内部样式不应当依赖外部（如 reset），虽然这样会增加代码量，但可以确保组件的独立与安全。
- 可能会出现同一个组件需要不同的样式，对于简单的样式变更，可以抽象并提供配置参数。对于稍复杂的改动（如更改 DOM 结构），则推荐创建新的组件。
- 必须编写使用文档。

## 免责声明

Element 是一套面向业务的移动端组件，基于 Vue + webpack 开发。  
目前由我一个人维护，版本和 API 都非常不稳定。（虽然已经在线上跑了 2333）  
总之，欢迎一起来改善，毕竟我还是图样……
