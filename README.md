# Git 桌面工作台

一个面向 Windows 的轻量中文 Git 桌面工具，把日常操作集中在清晰的可视化工作流中：

`查看改动 → 暂存文件 → 提交 → 推送 → 创建版本标签`

## 功能

- 打开、初始化或克隆 Git 仓库
- 查看未暂存与已暂存文件，以及代码差异
- 提交、推送、拉取并检查远端更新
- 查看提交历史、分支迭代图和版本标签
- 拖动分隔线调整面板，使用快捷键缩放界面
- 实时显示按钮实际执行的 Git 命令
- 内置适合初学者的 Git 帮助

## 技术栈

Electron、Vue 3、TypeScript、Pinia、simple-git。

## 本地运行

需要安装 Node.js 20+ 和 Git。

```powershell
npm install
npm run dev
```

## 测试与构建

```powershell
npm test
npm run typecheck
npm run package:win
```

Windows 安装包生成在 `release` 目录中。

## 发布新版本

1. 更新 `package.json` 和 `package-lock.json` 中的版本号。
2. 运行 `npm run package:win` 生成安装包。
3. 提交代码并创建同版本 Git 标签，例如 `v0.2.1`。
4. 在 GitHub 仓库的 **Releases** 页面创建 Release，并上传 `release` 中的 `.exe` 安装包。


