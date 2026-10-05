免验证码登录 Codex 打开即用，纯 JS 处理

原理：解析 ChatGPT Session 数据，构造合规的 Synthetic id_token 与非空 refresh_token，并自动提取 account_id 组装 ~/.codex/auth.json 配置给 Codex CLI

页面提供功能
1. 跳转 https://chatgpt.com/api/auth/session 获取 access token
2. 粘贴 Session JSON 到输入框
3. 生成不同平台的命令
    - windows powershell
    - linux bash
    - macos bash

