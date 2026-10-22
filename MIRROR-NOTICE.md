# dsh-purge — 第三方镜像备份（非官方）

本仓库是 **DSH（DeepSeek Harness）插件 `dsh-purge`** 的源码快照镜像，由 ZiLe1433 于 2026-10-22 备份，目的是在原作者停止维护、原仓库有被下架风险时保留可用的源码副本。

## 来源与版本

| 项目 | 值 |
| --- | --- |
| 插件名 | `dsh-purge` |
| 版本 | 1.1.71 |
| 原仓库 | https://github.com/YuJunZhiXue/dsh-purge |
| 安装来源（本地 profile） | `github:YuJunZhiXue/dsh-purge#6c1d638d1bdcc45ede50fc30249c753d58122a51` |
| 上游提交 | `6c1d638d1bdcc45ede50fc30249c753d58122a51` |
| 备份时间 | 2026-10-22 |
| 备份位置 | `%DSH_HOME%/profiles/desktop/node_modules/dsh-purge` |

## 文件说明

- `lib/` — 插件运行时（清洗核心 `core.js`、桌面端桥 `desktop.js`、红队台 `redteam/*`）
- `client.js` — Web 客户端 bundle（由 `scripts/build-client.mjs` 构建）
- `presets/redteam/` — 红队台 agent 预设与 anchor gate
- `skills/redteam/` — 红队技能文档（侦察、隧道、横向、凭证等）
- `docs/` — 截图、免责声明、上游披露与许可说明
- `bin/`、`scripts/` — CLI 与构建脚本
- `cordis.patch.yml` — DSH 插件 bundle 的加载补丁

## 许可

上游采用 MIT License（见 `LICENSE`，Copyright (c) 2026 小杨）。
本镜像原样保留该许可与版权声明，未作修改；如需二开请遵守上游 README 中的署名要求。

## 免责

- 本仓库为**非官方镜像**，与原作者无关，不代表原作者立场。
- 内容按“原样”提供，不承诺兼容未来版本的 DSH。
- 如果原作者恢复维护或提出异议，请优先使用原仓库，并可在 Issues 中告知以便下线本镜像。
