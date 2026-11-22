# DraftStamp · 写作十分钟邮局

把“我不知道怎么开始”变成一张可以马上动笔的小任务卡。DraftStamp 面向卡在报告、论文或个人写作起步的人：写一句卡点，离线得到三张可改写任务卡，挑一张专注十分钟，完成后盖一枚邮票；每三次挑战还能集成一页写作护照。

> 这是一个轻量、单页、无需安装的离线小工具。没有账号、联网 AI、待办看板或第三方依赖。

## 立即体验

1. 下载或解压项目文件夹。
2. 双击打开 `index.html`（也可以拖进现代浏览器）。
3. 写一句卡点，选一张任务卡，开始 10 分钟挑战。
4. 完成后下载挑战邮票 PNG；完成三次挑战后，还可下载写作护照卡。

不需要 Node.js、服务器、构建步骤或网络连接。主要界面、计时、记录和 PNG 导出都在浏览器本地完成。

## 写作护照

每完成一次挑战就收一枚类别邮戳，任意三次组成一页；重复类别也能集章。护照不设连续天数，停几天再回来，进度仍在。集满后可下载护照 PNG，内容只汇总三类挑战的次数和专注时长。旧版本已有的邮戳历史会保留，但不会混入新护照。

## 隐私说明

- 输入的卡点仅在当前页面内存中用于本地判断任务方向，不会上传；开始计时后会清空该输入框。
- 草稿和可编辑任务卡不会写入浏览器存储；刷新或关闭页面会清空它们。
- `localStorage` 只保存挑战记录和护照统计等元数据，不含正文；最近挑战记录保留最多 30 条，完成护照统计最多 5,000 页。
- 挑战 PNG 只含类别、时长和“已完成”；护照 PNG 只含类别次数和专注时长，不含输入原文、任务卡文本或草稿。
- 侧栏的“清空全部”会同时删除本机挑战记录、护照进度和已完成护照。
- 页面没有网络请求、分析追踪、登录或广告代码。

## 项目结构

```text
DraftStamp/
├── .gitignore   # 忽略系统杂项与本地 QA 工作目录
├── index.html   # 完整应用；CSS、JavaScript 和图形均内嵌，可离线打开
├── LICENSE      # MIT 许可证
└── README.md    # 中英双语使用与项目说明
```

## 开发

本项目没有打包或安装步骤。修改后直接重新打开 `index.html` 即可预览。

## 许可证

本项目采用 MIT 许可证，具体条款见 [LICENSE](LICENSE)。

## English

DraftStamp is a tiny, offline-first writing starter for people stuck at the beginning of a report, essay, or personal draft. Describe the block in one sentence, get three editable task cards generated locally, choose one, write for ten minutes, and collect a stamp. Three challenges make a shareable writing-passport page.

### Quick start

Open `index.html` in a modern browser. No install, build step, server, account, network connection, or third-party dependency is required.

### Writing passport

Every completed challenge adds one category stamp; any three challenges fill a page, including repeated categories. There is no streak or deadline. Downloaded passport PNGs contain only per-category challenge counts and total focus time. Existing challenge history remains, but older stamps do not count toward the first passport page.

### Privacy by design

The blocker text is used only in the current page's memory to select a local prompt category. It is cleared when a challenge starts. Draft text and editable cards are never written to browser storage and disappear on refresh or close. `localStorage` keeps only challenge and passport metadata, not writing text. Challenge PNGs contain category, duration, and completion status; passport PNGs contain category counts and focus time. The app makes no network requests and includes no analytics or tracking.

### License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
