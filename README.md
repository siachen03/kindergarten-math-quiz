# 小班数学选择题 Beta

一个面向幼儿园小班/中班早期练习的数学选择题网页。页面可以直接部署为静态网站，适合在 iPad、平板浏览器或电脑浏览器中使用。

<img width="2310" height="2418" alt="ScreenShot_2026-07-02_155641_133" src="https://github.com/user-attachments/assets/35116352-b12a-4d85-bbd5-8aed80280dc9" />
<img width="2466" height="2356" alt="ScreenShot_2026-07-02_172647_992" src="https://github.com/user-attachments/assets/0d1a1b21-92b6-40f2-ab83-2d880ec73075" />
<img width="2084" height="2310" alt="ScreenShot_2026-07-02_155728_010" src="https://github.com/user-attachments/assets/7ba3cb46-2e66-438c-a1b3-6ac0e1fdde0b" />
<img width="2058" height="2366" alt="ScreenShot_2026-07-02_155748_344" src="https://github.com/user-attachments/assets/798821e8-0c86-40f5-9512-eedf6f4e53e6" />
<img width="2064" height="2344" alt="ScreenShot_2026-07-02_155841_431" src="https://github.com/user-attachments/assets/4df5c87a-ce92-40dd-8bb8-95b38c2e4486" />


## 在线部署

这个项目是纯静态网页，不需要后端服务。

- Netlify: 将项目目录拖到 Netlify Drop 即可发布。
- GitHub Pages: 仓库开启 Pages 后，选择根目录发布即可。
- 本地预览: 直接打开 `index.html`。

## 内容特点

- 覆盖数一数、找数字、数量配对、多少比较、长短高矮、规律、分类、排序、补缺数字、加减法、图形、空间位置等题型。
- 按简单、一般、困难分级。
- 内置中文女声题目播报和选项播报。
- 适配平板触控，按钮较大，适合儿童点选。
- 无需登录、无需联网 API，部署后可直接访问。

## 语音说明

语音文件已内嵌在 `audio/` 目录中，使用 Kokoro `zf_xiaoxiao` 中文女声生成。

- TTS 模型: Kokoro / Kokoro-82M
- 本地生成工具: sherpa-onnx `kokoro-multi-lang-v1_0`
- 语音清单: `audio_manifest.json`

参考来源:

- Kokoro: https://huggingface.co/hexgrad/Kokoro-82M
- sherpa-onnx TTS: https://k2-fsa.github.io/sherpa/onnx/tts/

## 当前状态

这是 Beta 版本。已经可以发布和体验，但仍建议根据真实使用反馈继续迭代。

后续可优化方向:

- 默认一轮题量从 150 题改为 10-15 题小组练习。
- 对小班用户弱化 `> < =` 符号题，优先使用“哪个更大/哪个更小”的问法。
- 答对后增加解释朗读，例如“十小于十八，所以选小于号”。
- 为家长或老师增加练习记录导出。

## 文件结构

```text
.
├── index.html
├── audio/
├── audio_manifest.json
├── docs/
│   └── preview.png
└── README.md
```

## 许可

项目代码采用 MIT License。语音模型及相关工具请遵守其上游许可说明。
