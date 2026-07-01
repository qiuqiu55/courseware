# 中考英语自学系统

一个为中学生设计的英语词汇自学系统，包含72个单元，每个单元30个词，共2160词。

## 功能特点

- 🎯 **智能复习系统**：错词自动收集，连续答对2次移出复习池
- 📊 **进度追踪**：每个单元独立记录学习进度
- 🏠 **总主页**：一目了然查看所有单元进度
- 📖 **四轮循环**：词义识别 → 拼写掌握 → 词形变化 → 综合运用
- 🔊 **真人发音**：支持TTS语音发音（浏览器原生）

## 使用方法

1. 双击打开 `zhongkao-vocab-index.html`（总主页）
2. 点击任意单元卡片进入学习
3. 完成学习后点击左上角"🏠 返回主页"

## 目录结构

```
courseware/
├── zhongkao-vocab-index.html    # 总主页
├── zhongkao-vocab-unit1/       # 单元1
│   ├── index.html               # 单元课件
│   ├── manifest.json           # 单元元数据
│   └── assets/
│       └── vocabulary-data.js  # 词汇数据
├── zhongkao-vocab-unit2/       # 单元2
├── ...
└── zhongkao-vocab-unit72/      # 单元72
```

## 技术栈

- 纯HTML5 + CSS3 + JavaScript（无框架依赖）
- localStorage 存储学习进度
- Free Dictionary API 获取音标和例句

## 适用人群

- 初中学生（中考备考）
- 英语教师（课堂辅助工具）
- 自学者（系统性扩充词汇量）

## 许可证

MIT License
