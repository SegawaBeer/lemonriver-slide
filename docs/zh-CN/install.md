# 安装说明

[English](../en/install.md) · 简体中文 · [回到首页](../../README.zh-CN.md)

## Mac 安装包（推荐）

不用装 Node.js，也不用开终端。目前只支持 Apple 芯片的 Mac（M1 及以后），系统需要 macOS 11 或更新。

1. 打开[最新版下载页](https://github.com/SegawaBeer/lemonriver-slide/releases/latest)，在页面下方「Assets」里点 `LemonRiver-<版本>-arm64.dmg` 下载。
2. 双击下载的文件，在弹出的窗口里把 LemonRiver 拖进「应用程序」。
3. 打开「应用程序」文件夹，双击 LemonRiver。**不要直接在安装盘的窗口里打开**，先拖进「应用程序」。
4. 第一次打开会被系统拦下（因为安装包没有经过苹果公证）：
   1. 在提示框里点「完成」。
   2. 打开「系统设置 → 隐私与安全性」，往下翻到「安全性」一栏，点「仍要打开」。
   3. 输入开机密码确认。之后再打开就不会拦了。
5. 第一次打开要等十几秒准备工作区，然后浏览器会自动打开 LemonRiver 的使用指南。

装好以后：

- 你的幻灯片都在「个人文件夹 → LemonRiver」里，让 Agent 在这个文件夹里工作（见[使用指南](guide.md)）。
- 程序坞和桌面上的柠檬就是入口，点一下就在浏览器里打开。
- 有新版本时程序里会提示，点「立即更新」就行，不用重新下载安装包。

## 用命令行建工作区

已经装了 Node.js（20.19 以上或 22.12 以上）的话，可以自己建一个工作区，Windows、Linux 也能用：

```bash
npx @lemonriver/cli init my-slide --use-pnpm
cd my-slide
pnpm dev
```

init 会顺手把依赖装好（npm、pnpm、yarn、bun 都支持，把 `--use-pnpm` 换成 `--use-npm` 等即可）。打开终端里显示的地址，就能在浏览器里用了。

## 常见问题

- **提示「请先把 LemonRiver 拖到「应用程序」文件夹，再从那里打开」**：说明是直接在安装盘里打开的。把它拖进「应用程序」，再从那里打开。
- **系统设置里找不到「仍要打开」**：先双击打开一次 LemonRiver，让系统拦一次，按钮才会出现。
- **浏览器里打不开页面**：再点一次程序坞上的柠檬。还不行的话，在 [Issues](https://github.com/SegawaBeer/lemonriver-slide/issues) 里告诉我们你看到的提示。
