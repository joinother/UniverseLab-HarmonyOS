# UniverseLab-HarmonyOS · 星体实验室

鸿蒙原生宇宙沙盒实验平台：用 **ArkTS/ArkUI** 构建交互界面，用 **OpenSPH** 的 C++ SPH 求解器计算岩质碰撞，用独立的 C++ 多体引力模型计算行星轨道，通过 `XComponent` / OpenGL ES 显示。

包名 `com.opensph.lab`，当前源码版本 **0.57.0**。

## 目录

| 路径 | 内容 |
|---|---|
| `OpenSPH-HarmonyOS-Native/` | 完整 DevEco 工程（ArkTS + C++）。**从这里开始读**：[工程 README](OpenSPH-HarmonyOS-Native/README.md) |
| `docs/screenshots/` | 版本里程碑截图（0.45–0.47） |
| `docs/experiments/` | 实验产出记录（JSON） |
| `CHECKPOINT.md` | 本轮工作检查点 |

## 项目来源

本仓库从 [`joinother/OpenSPH-HarmonyOS`](https://github.com/joinother/OpenSPH-HarmonyOS) 的
`checkpoint/arkui-0.17.0-2026-09-06` 分支拆分而来（55 个提交，2026-09-06 → 2026-09-09），
与原仓库共享第一作者与开发脉络，但作为独立项目演进。

- 原仓库保留：**OpenSPH 原版 wxWidgets UI 的鸿蒙移植**（适配层 + 补丁，不含上游源码）
- 本仓库保留：**基于 OpenSPH 内核重写的 ArkUI 宇宙沙盒**

历史完整截图（36 个版本、193 张）保留在原仓库备份标签
`backup/before-split-20261028/simulator` 中。

## 上游依赖

SPH 求解基于 [OpenSPH](https://github.com/pavelsevecek/OpenSPH)（基线 v0.4.1）。
与上游的关系、补丁方式见原仓库的 `UPSTREAM.md`。

## 构建

用 DevEco Studio 打开 `OpenSPH-HarmonyOS-Native/`，构建配置与依赖说明见该目录的 `README.md` 与 `docs/`。
