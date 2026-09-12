# 当前项目上下文

更新：2026-09-12。仅维护当前事实；长期规则见根 `SKILL.md` 和 `AGENTS.md`。本页预算 80 行 / 8 KiB，旧检查点迁入专题，不追加长日报。

- 默认目录 `E:\PenguinPravite\T8-penguin-canvas`；branch `codex/release-v3.0.8-volcengine-assets-ux`，common dir `.git`。v3.1.6 正式源码与 Tag 固定为 `a747224846aa311c0e7c6a3f0ac4988881b58e36`；发布后证据提交可推进当前分支与 `main`，但不得移动 Tag。实际开工仍以 git/worktree 门为准。
- package 版本为 `3.1.6`；[v3.1.6 GitHub Release](https://github.com/T8mars/T8-penguin-canvas/releases/tag/v3.1.6) 已于 `2026-09-12T04:39:06Z` 发布为非草稿、非预发布 Latest，Windows 与 macOS arm64 六个安装/自动更新资产已附加。
- 本任务正式发布已完成；固定源码、Windows 正式包、GitHub 推送/Tag/Latest、自动更新资产和额度允许的同源 Mac 包均已完成。外部证据仍按 `owner-approved-post-release-v3.1.6` 后补，不视为通过。

## 当前检查点

| 事项 | 当前事实与下一步 |
| --- | --- |
| v3.1.6 发布 | Windows 唯一一次生产编译/加密链和系统 7-Zip 复用同次 `win-unpacked` 的 NSIS 恢复完成，7 文件 app.asar、双运行时、provenance/sealed recovery、上传及完整回下载通过；[macOS workflow](https://github.com/T8mars/T8-penguin-canvas/actions/runs/34673590415) 同源成功，本机独立回下载通过。六资产大小与 SHA-256 见 `feature release`。Tag 固定，不随本页证据提交移动。 |
| 文档轻量化 | 已完成：根手册62行，原文逐字节归档；默认三份上下文约18KiB，features/roadmap按需读。8组校验通过，1353份源码/配置/原测试/技能散列未变，详见[校验记录](../local-private/context-maintenance/verification.json)。后续遵守手册开头预算。 |
| 生成历史 | 当前支持范围已随 v3.1.6 发布；19个完整客户端场景/25项、React UI 13项、限定回归56/56通过，通过进程正常退出/强制0/残留0。完整状态与剩余范围见[验收清单](generation-history-acceptance-status.md)及[证据索引](generation-history-acceptance-20260912.md)。 |
| 历史修复最终限定检查 | 专题清单与 features 回执已同步为 19/25+React UI 13、限定回归56/56；本轮按暂停点复核后未重跑。支持范围已接受；用户旧库、安装升级、断电、真实Provider、外部设备与其他未适配输入仍不计通过。 |
| 工坊 Suno V6 | 三版本已随 v3.1.6 发布且有出音证据；wild请求 `chirp-hawk-wild` 实际返回 `chirp-hawk`，身份需渠道确认。保留旧模型/默认与独立平价协议，不再自动付费重试。用 `feature sunoWorkshopV620260912` 查完整记录。 |
| 平价小屋 Suno V6 | 三项动作、34项目录、双语UI和4份无密钥工作流已随 v3.1.6 发布。真实API三动作各有成功案例；失败的纯测试音模型案例明确记录且未冒认。详见[专题与证据](seedance-nz-suno-v6-actions.md)。 |
| Creator 技能市场 | 首期基础能力已随 v3.1.6 发布；真实模型作品、质量盲评、新手试点、生态治理和完整整体验收仍未完成。用 `feature creatorSkillMarket20260910` 查询。 |
| 外部验收 | F8–F10、真实设备与用户环境仍按原约束未完成。临时夹具不替代外部证据。 |

## 按需取上下文

```powershell
node scripts/read-project-context.cjs find history
node scripts/read-project-context.cjs feature generationHistoryRecovery20260910 status
node scripts/read-project-context.cjs feature sunoWorkshopV620260912
node scripts/read-project-context.cjs roadmap 生成历史
node scripts/read-project-context.cjs find 打包
```

工具只读取项目文档；默认输出有限页，显示总行数与后续页命令。需要详细规则时继续翻页，禁止将截断页面当全文已读。完整 features 仍是原路径原结构，无需改现有消费者。
