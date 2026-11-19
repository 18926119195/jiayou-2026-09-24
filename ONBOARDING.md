# 加油 · 9 月 24 日实验归档入库指南

[一分钟定位](#一分钟定位) · [沿聊天时间线看灵感](#沿聊天时间线看灵感) · [从代码反查来由](#从代码反查来由) · [走读与维护记录](#走读与维护记录)

## 一分钟定位

这个公开仓库是 2026 年 9 月 24 日的 Cursor 归档，包含 12 个聊天窗口、11 个终端快照、6,048 份变更文件笔记。它把当时的实验决策与文件位置连起来。代码和完整运行产物在 [源工程 `chenggong-jiachi-master` 的参考提交](https://github.com/18926119195/chenggong-jiachi-master/tree/9da50bc1f5731a2c988a1bd906f8e427044033b8)，本库只保存导出记录与预览。两库都有同名的 12 个窗口文件，其中 11 个 Git blob 完全一致。本指南的消息位置以本库为准。归档基线为 [`main` 的 `d4fe893`](https://github.com/18926119195/jiayou-2026-09-24/commit/d4fe893a282d227de13124eb5560e74cc0ec5d61)。

## 沿聊天时间线看灵感

**如何读状态。** 已实现表示在所列版本找到与灵感相符的代码路径。部分实现表示已有其中一段。未实现表示已查的入口尚无对应实现。证据不足时标待确认。归档与设计文稿按资料本身的状态描述。

表中为主人在各窗口提出问题的时间，均为 9 月 24 日北京时间。状态用「归档」指本库，用「源工程」指另一个提交；聊天中的推测按当时证据理解。

| ID／时间 | 仓库主人的问题与决定 | 状态 | 代码与材料证据 |
| --- | --- | --- | --- |
| <a name="idea-i01"></a>I01 · 10:15 | 先查 CoT 实验中每个目录的用途，再区分文件改动与对照是否有污染。[原始对话](chats/2e343cf4-45b8-4018-9c87-69a7d02001d9.md) | 已落地（归档） | [当天索引](TODAY-INDEX.md) 登记了会话、脚本预览、实验产物及终端输出。[源工程的对照报告](https://github.com/18926119195/chenggong-jiachi-master/blob/9da50bc1f5731a2c988a1bd906f8e427044033b8/cot对比实验/提高缓存命中率的实验/COMPARISON-REPORT.md) 是两题实验，不能用来代表全量。 |
| <a name="idea-i02"></a>I02 · 12:41 | 核对缓存指标是否从响应的真实 usage 字段提取，能否区分命中和未命中。[原始对话](chats/46dde017-d602-47e5-8d6c-23b8162c134d.md) | 已落地（报告） | [9 月 23 日余下题目批次预览](file-notes/问题一__runs__2026-09-23-cache-test-rerun-remainder__token-cost-report.json.md) 分列命中、未命中和输出 token。 |
| <a name="idea-i03"></a>I03 · 14:56 | 同一道题的步骤可能触发多次调用，询问备份和运行目录应如何辨认。[原始对话](chats/d88c8485-40c1-48c7-9da1-12111254d869.md) | 部分落地 | [跨批次比较脚本预览](file-notes/问题一__runs__2026-09-24-cache-test-rerun__compare-prev-vs-current.cjs.md) 对齐两次 Z1-Q2 的请求及响应，并记录预热条件差异。当前证据覆盖这个对照例，其他备份仍需逐个确认归属。 |
| <a name="idea-i04"></a>I04 · 15:51–15:54 | 首次将全部去重名词作为前缀，再用较短分批请求，观察命中率是否提升。[原始对话](chats/9d2b2485-15b3-4ae1-af87-3f91f663593c.md) | 部分落地（单题实验） | [Z3-Q2 预热脚本](file-notes/test-cache-warmup-z3q2.js.md) 与 [对应结果预览](file-notes/cache-warmup-test-z3q2.json.md) 记录由长到短的实验。这个预览无法确认全量生产链采用同一策略。 |
| <a name="idea-i05"></a>I05 · 16:35 | 按文件核算 API 成本，需要说明缓存命中和输出用量如何计价。[原始对话](chats/d1fa02de-606c-472e-b761-31748b84d5ce.md) | 待确认（该窗口口径） | 归档中有 [缓存率脚本预览](file-notes/问题一__runs__2026-09-24-cache-test-rerun__cache-rate.cjs.md) 和 I02 的成本报告。I02 对应 13 题旧批次，本窗口核算的是另一个目录，不能把两处数字当成同一份账。 |
| <a name="idea-i06"></a>I06 · 16:39–16:47 | 从答案提取机器编号，再回看推理中的同编号可能落在一个还是多个位置。[原始对话](chats/281b9f6a-4320-41cd-8289-a6ed381c81d0.md) | 部分落地 | [追踪脚本预览](file-notes/cot对比实验__提高缓存命中率的实验__llm-configs__trace_mapper.ps1.md) 提供对照入口，能看到向原文追踪的设计。对话追问的多处映射应按实际题目与文件核验。 |
| <a name="idea-i07"></a>I07 · 19:02 | 在保留旧产物的情况下，复刻同一流程并重跑 15 题。[原始对话](chats/f157b225-f56d-48c5-a066-7c9dedda1a65.md) | 已落地（源工程） | [复跑说明预览](file-notes/问题一__runs__2026-09-24-cache-test-rerun__README.txt.md) 和 [源工程批次目录](https://github.com/18926119195/chenggong-jiachi-master/tree/9da50bc1f5731a2c988a1bd906f8e427044033b8/问题一/runs/2026-09-24-cache-test-rerun) 留有逐题快照、日志、最终输出。旧批次的成本归档仍单独存在。 |
| <a name="idea-i08"></a>I08 · 20:02 | 将当天各窗口和变更文件做成 Markdown 导航，取名「加油」。同 I07 会话第 91 条消息。 | 已落地（归档） | [主索引](TODAY-INDEX.md)、[仓库说明](README.md) 与当前 Git 提交对应。 |

## 从代码反查来由

| 先看到的文件 | 应查的会话 |
| --- | --- |
| [逐题快照运行器](https://github.com/18926119195/chenggong-jiachi-master/blob/9da50bc1f5731a2c988a1bd906f8e427044033b8/run-test15-with-snapshot.js) · [逐题布局预览](file-notes/9.24最终版本__README.md.md) | [I03](#idea-i03)、[I07](#idea-i07)。先确定阶段、题号和运行目录，再阅读快照编号。 |
| [预热脚本预览](file-notes/test-cache-warmup-z3q2.js.md) · [跨批次比较预览](file-notes/问题一__runs__2026-09-24-cache-test-rerun__compare-prev-vs-current.cjs.md) | [I02](#idea-i02)、[I04](#idea-i04)–[I05](#idea-i05)。预热单题、13 题余量批次和 15 题全量批次各自有口径。 |
| [索引与归档布局](TODAY-INDEX.md) | [I01](#idea-i01)、[I08](#idea-i08)。索引在本库，工程脚本在源工程。 |

## 走读与维护记录

第一次读，从 [I07](#idea-i07) 的第一条主人消息进入，依次看复跑说明和 [I03](#idea-i03) 的 Z1-Q2 比较，再打开源工程批次下的 `final/`。只跟一题即可看到为什么同题会有多批快照、重跑前备份和不同成本统计。

本次离线核对了总索引中的 361 个表格链接。需要补一个线索时，在对应 I 编号写清会话消息、源仓库提交、批次和相对路径。分享公开摘要时用获准的脱敏预览。

**指南如何更新。** 以仓库和版本划定范围，从聊天提取原始目标，再用代码与产物校正对当时决策的理解。新证据出现时，回到原编号修订记录。这种读法借鉴了钱学森的系统工程和工程控制论。 [《组织管理的技术——系统工程》](https://doi.org/10.13255/j.cnki.jusst.2011.06.020) · [《工程控制论》](https://openlibrary.org/books/OL49218199M/Engineering_cybernetics)
