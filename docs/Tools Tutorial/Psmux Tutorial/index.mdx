---
title: "Psmux 初学者教程"
description: "面向初学者的 Psmux 上手指南：安装、会话、窗口、面板与常用配置"
sidebarTitle: "Psmux Tutorial"
---

# Psmux 初学者教程

> 本文面向第一次接触 `psmux` 的使用者，目标是让其在 15-30 分钟内完成从安装到日常使用的闭环。

## 1. Psmux 是什么

`psmux` 可以理解为“终端里的工作台管理器”：

- 普通终端像单人书桌：一次只能专注一个任务窗口。
- `psmux` 像带分区的工作台：同一屏里可以并排观察编辑器、日志、测试、监控，并可随时离开再回来。

它是 Windows 原生的终端复用器，兼容 tmux 命令语言，常见别名有：

- `psmux`
- `pmux`
- `tmux`

这三个命令在 psmux 中等价。

## 2. 三个核心概念（必须先建立）

初学者最容易混淆的是层级关系。可用“办公楼类比”快速记忆：

- `Session`（会话）= 一层楼。
- `Window`（窗口）= 楼层中的一个房间。
- `Pane`（面板）= 房间里的工位。

层级关系可写成：

$$
\text{Session} \supset \text{Window} \supset \text{Pane}
$$

这条关系是后续所有命令理解的“母规则”。

## 3. 安装与验证（Windows）

推荐使用 `winget`：

```powershell
winget install psmux
```

安装后验证：

```powershell
psmux --help
tmux --help
```

如果两条都能输出帮助信息，说明别名也已可用。

## 4. 5 分钟上手闭环（建议照打）

### 第一步：创建命名会话

```powershell
psmux new-session -s work
```

### 第二步：切分面板

- `Ctrl+b` 后按 `%`：左右分屏。
- `Ctrl+b` 后按 `"`：上下分屏。

> 注意：Prefix 是“先后按键”，不是同时按。默认 Prefix 为 `Ctrl+b`。

### 第三步：在不同 Pane 跑不同任务

例如：

- Pane A：编辑代码。
- Pane B：`npm test --watch`。
- Pane C：`tail -f` 日志。

### 第四步：临时离开会话

- `Ctrl+b` 后按 `d`（detach）。

此时任务仍在后台运行，不会因为关闭当前终端窗口而结束。

### 第五步：稍后恢复

```powershell
psmux ls
psmux attach -t work
```

到这里，最关键的“创建-分屏-分离-恢复”闭环已完成。

## 5. 初学者高频操作清单

### 会话管理

```powershell
psmux ls
psmux new-session -s dev
psmux attach -t dev
psmux kill-session -t dev
```

### 窗口管理（Prefix 后）

- `c`：新建窗口。
- `n` / `p`：下一个 / 上一个窗口。
- `,`：重命名窗口。
- `0-9`：按编号跳转。

### 面板管理（Prefix 后）

- `Arrow`：在面板间移动焦点。
- `x`：关闭当前面板。
- `z`：当前面板最大化/还原。
- `q`：显示面板编号并快速跳转。

## 6. 第一个配置文件（让体验更顺手）

`psmux` 启动时会按顺序读取配置文件（例如 `~/.psmux.conf`、`~/.tmux.conf`）。

建议新建 `~/.psmux.conf`：

```tmux
# 把前缀改成 Ctrl+a（可选）
set -g prefix C-a

# 鼠标支持
set -g mouse on

# 滚动历史行数
set -g history-limit 5000

# 窗口编号从 1 开始（便于记忆）
set -g base-index 1
```

如果需要临时指定配置文件：

```powershell
psmux -f ~/.config/psmux/custom.conf
```

## 7. 常见误区与“新手不知道自己不知道”

### 误区 1：关闭终端 = 任务结束

不一定。只要任务在 `psmux` 的会话里运行，detach 后仍可继续。

### 误区 2：`Ctrl+b` 没反应

常见原因：

- 把 Prefix 误当成“组合键同时按”。
- 终端被其他快捷键占用。
- 已将 `prefix` 改为其他键但忘记。

### 误区 3：只会建 Pane，不会管理 Session

真正的生产力增益来自“会话持久化”。可把效率粗略理解为：

$$
\text{有效开发时间占比}=\frac{\text{连续专注时间}}{\text{连续专注时间}+\text{上下文重建时间}}
$$

`psmux` 通过减少“上下文重建时间”提升长期效率。

## 8. 推荐的日常工作流模板

一个可复用的结构：

- Session：`project-a`。
- Window 1：`editor`（代码与 REPL）。
- Window 2：`test`（单测/集成测试）。
- Window 3：`logs`（应用日志、系统指标）。

每天只需 `attach` 回来即可继续昨天的上下文。

## 9. 下一步学习路径

- 学会复制模式（`Prefix + [`）与缓冲粘贴（`Prefix + ]`）。
- 学会自定义键绑定（`bind-key`）。
- 在团队中约定统一命名规则：`session/window` 命名即文档。

---

## 参考资料

- 官方仓库：<https://github.com/psmux/psmux>
- 官方安装与用法：<https://github.com/psmux/psmux#installation>
- 官方快捷键文档：<https://github.com/psmux/psmux/blob/master/docs/keybindings.md>
- 官方配置文档：<https://github.com/psmux/psmux/blob/master/docs/configuration.md>
- 
