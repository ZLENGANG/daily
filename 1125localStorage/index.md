## localStorage、sessionStorage的用途
* 用来存储登录后的token
* 用户部分信息的储存，如用户名、头像、简介
* 一些项目通用参数的存储，例如某个id、某个参数params
* 项目持久化存储，如vuex、redux
* 项目整体切换状态大的存储，如主题、语言、icon风格


## 开发中使用暴露的缺点
* 命名过于简单，如user、theme、token
* 不隐秘，未加密

## 解决方案
* 命名规范：项目名+当前环境+版本号+缓存key，如：blkg_dev_680_user，实际使用时应注意封装
* 安全：使用crypto-js进行对数据的加密，需要讨论必要性
