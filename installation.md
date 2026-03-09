# NCF 安装指南

## 前提条件

- Daemonic 解锁器已安装并正常运行
- 魔兽世界客户端

## 文件结构

下载后你会得到以下文件：

```
├── ncf_encrypted.lua       # 核心文件 (加密版)
└── rotations/              # 循环文件夹
    ├── mage_arcane.lua
    ├── mage_frost.lua
    ├── warrior_fury.lua
    └── ...
```

## 安装步骤

1. 将 `ncf_encrypted.lua` 复制到 Daemonic 启动 exe 所在的根目录
2. 将 `rotations/` 文件夹整个复制到 Daemonic 启动 exe 所在的根目录
3. 启动游戏，NCF 会自动加载

最终目录结构：

```
Daemonic/
├── ncf_encrypted.lua
├── rotations/
│   ├── mage_arcane.lua
│   └── ...
└── config/                 # 首次运行后自动生成
    └── ncf_config.dat
```

## 首次使用

1. 进入游戏后 NCF 自动加载
2. 按 **F1** 开启/关闭循环
3. 按 **F2** 切换爆发/划水模式
4. 选中目标后自动建议技能

> **本软件完全免费，如果你是花钱买的，说明你被骗了。**

> 按住 Alt、Shift 或 Ctrl 时循环暂停，松开后恢复。骑乘状态下也会暂停。

## 常见问题

**Q: 没有自动加载？**
- 确认 `ncf_encrypted.lua` 在 Daemonic 启动 exe 所在的根目录下
- 确认 Daemonic 已正常启动
- 重新进入游戏或 `/reload`

**Q: 没有显示技能提示？**
1. 确保循环已开启（状态栏显示「已开启」）
2. 确保有可攻击的目标
3. 确保 `rotations/` 中有对应专精的 `.lua` 文件

**Q: config 文件夹是什么？**
- 首次运行后自动生成，存储你的个人设置
- 不要删除，否则需要重新配置
