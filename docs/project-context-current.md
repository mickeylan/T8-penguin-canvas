# 当前项目上下文

更新：2026-09-12。仅维护当前事实；长期规则见根 `SKILL.md` 和 `AGENTS.md`。本页预算 80 行 / 8 KiB，旧检查点迁入专题，不追加长日报。

- 默认目录 `E:\PenguinPravite\T8-penguin-canvas`；最近核对 branch `codex/release-v3.0.8-volcengine-assets-ux`、HEAD `a9ce7a770c8730c20934b2216bc5700b5586f724`、common dir `.git`。实际开工仍以 git/worktree 门为准。
- package 版本已同步为 `3.1.6`；v3.1.5 Tag 固定源码为 `d3d16054f049bfa01aa64e1432c5d382cc806f59`。2026-09-12 已联网核对 origin/main 与当前 HEAD 同为 `a9ce7a770c8730c20934b2216bc5700b5586f724`，v3.1.6 Tag/Release 尚不存在。
- 本任务授权：更新根 SKILL/features/版本事实，执行唯一一次 Windows Electron 正式构建，推送固定源码与 v3.1.6 Tag，发布 GitHub Latest 和自动更新资产；外部证据后补但不视为通过。Mac 仅在 GitHub Actions 额度足够时发布，其余必须完成。

## 当前检查点

| 事项 | 当前事实与下一步 |
| --- | --- |
| 文档轻量化 | 已完成：根手册62行，原文逐字节归档；默认三份上下文约18KiB，features/roadmap按需读。8组校验通过，1353份源码/配置/原测试/技能散列未变，详见[校验记录](../local-private/context-maintenance/verification.json)。后续遵守手册开头预算。 |
| 生成历史 | 19个完整客户端场景/25项、React UI 13项、限定回归56/56通过；通过进程正常退出/强制0/残留0。此为已有报告事实，本次未重跑。完整状态与剩余范围见[验收清单](generation-history-acceptance-status.md)及[证据索引](generation-history-acceptance-20260912.md)。 |
| 历史修复最终限定检查 | 专题清单与 features 回执已同步为 19/25+React UI 13、限定回归56/56；本轮按暂停点复核后未重跑。支持范围已接受；用户旧库、安装升级、断电、真实Provider、外部设备与其他未适配输入仍不计通过。 |
| 工坊 Suno V6 | 三版本已实现且有出音证据；wild请求 `chirp-hawk-wild` 实际返回 `chirp-hawk`，身份需渠道确认。保留旧模型/默认与独立平价协议，不再自动付费重试。用 `feature sunoWorkshopV620260912` 查完整记录。 |
| 平价小屋 Suno V6 | `suno-create-model` / `suno-upload-cover` / `suno-upload-extend` 已按动作白名单接入，34项目录、双语UI和4份无密钥工作流已同步。真实API三动作均有一次成功案例：Cover/Extend各2段MP3+2张JPEG并完整校验，Create Model返回36位UUID；失败的纯测试音模型案例明确记录且未冒认。详见[专题与证据](seedance-nz-suno-v6-actions.md)。 |
| Creator 技能市场 | 既有未发布工作保留；用 `feature creatorSkillMarket20260910` 查询，不在本轮扩大开发。 |
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
