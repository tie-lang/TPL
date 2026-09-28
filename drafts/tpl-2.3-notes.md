# TPL 2.2 → 2.3 Revision Notes / TPL 2.2 → 2.3 修订说明

Status: **DRAFT for review** — `drafts/tpl-2.3-draft.txt`. The canonical `tpl.txt`
and the frozen `2.2` copy are untouched until this draft is approved; adoption
follows the dual-write policy (update `tpl.txt`, add a byte-identical `2.3`
copy).

状态：**草稿待审** —— `drafts/tpl-2.3-draft.txt`。权威文本 `tpl.txt` 与冻结副本
`2.2` 在草稿获批前不动；换版按双写纪律执行（更新 `tpl.txt`，新增逐字节一致的
`2.3` 副本）。

## Decisions locked in / 已定决策

1. **Termination regime / 终止体制**: the copyright and database rights grants
   are irrevocable except for a **material breach** (§11.2); the patent grant
   is irrevocable except for patent retaliation (§3.3) or a material breach.
   Reinstatement is **automatic** on cure (§11.5, Apache-style), replacing the
   sole-discretion clause.
   版权与数据库权利许可仅在**材料违约**（§11.2）时终止；专利许可仅在专利报复
   （§3.3）或材料违约时终止。复权改为**治愈即自动**（§11.5，对齐 Apache），替换
   原来的"许可人酌情"条款。

2. **Renumbering allowed but avoided / 允许重排但未动**: the 15-section
   skeleton and clause numbers are preserved so that existing references,
   templates and links remain valid; new clauses were appended within sections
   (2.8, 2.9, 6.5, 15.8).
   保留 15 节骨架与全部原节号，新条款在节内追加（2.8、2.9、6.5、15.8），既有
   引用、模板与链接不失效。

3. **Compression / 压缩**: net size 46,437 → 44,483 bytes despite ~3.5 KB of
   new clauses (legacy text compressed ~15%: preamble, §8, §9, §10, §4 lists).
   尽管新增约 3.5 KB 条款，全文净减约 2 KB（序言、§8、§9、§10、§4 各列表压缩
   约 15%）。

4. **Notice pinned / 通知钉死版本**: the appendix notice states the exact
   version ("TPL-2.3") and forbids "current version" wording; §14.3 covers
   prior-version continuation.
   附录通知写明精确版本（"TPL-2.3"），禁止"当前版本"措辞；旧版本作品继续受其
   发布时版本约束（§14.3）。

## Hard defects fixed / 硬伤修复

- Dangling "Section 5.7" cross-references in §11.4 and §15.5 → now cite
  existing sections. / §11.4 与 §15.5 中两处悬空的 "Section 5.7" 引用已修正。
- Appendix placeholder `<uniform resource locator...>` removed; real URLs
  (canonical GitHub text + https://tpl.franj2.top/). / 附录占位符删除，替换为
  真实链接。
- Version-pinning ambiguity removed. / 版本锁定歧义移除。

## New clauses / 新增条款

- **§2.8 Database Rights** — sui generis database rights granted on the same
  footing as copyright. / 数据库特殊权利（sui generis）与版权同等待遇授权。
- **§2.9 Moral Rights (Licensor waiver)** — licensor waives moral rights to
  the extent permitted, attribution obligations unaffected. / 许可人精神权利
  豁免（CC4 式），§4 署名义务不受影响。
- **§6.5 Linking and Interfaces** — static/dynamic linking, API/protocol
  communication, plugin loading, execution under a runtime/interpreter, and
  declaring or implementing compatible interfaces do not by themselves create
  a Derivative Work; independent portions are User Works. / 链接边界条款：
  静态/动态链接、API/协议通信、插件加载、运行时/解释器执行、声明或实现兼容
  接口，均不本身构成 Derivative Work，独立部分为 User Work。
- **§6.4(e)/(f) AI extensions** — embeddings/vector/retrieval indexes are not
  Licensed Material (verbatim-substantial redistribution still subject to §4);
  benchmarks/evaluations are permitted and their results are User Works. /
  AI 扩展：嵌入/向量/检索索引不属于授权材料（逐字实质部分再分发仍受 §4）；
  基准与评测允许开展，结果为 User Work。
- **§15.8 Official Translations** — only Licensor-designated translations are
  official; English text prevails. / 官方翻译条款：仅许可人指定者为官方，英文
  文本优先。
- **§8 savings clause** — voluntary warranty/indemnity by a distributor is at
  its own responsibility. / §8 增加分发者自愿担保责任自负条款。

## Wording generalization / 措辞全面去软件化

- "Source Code" → **"Source Form"** (§1.4 now defines it generically with
  examples for programs, fonts/graphics, documents, datasets, models, hardware
  designs; multi-form works are resolved by Licensor identification or the
  preferred-form test). / "Source Code" 改为 **"Source Form"**，定义覆盖各类
  作品形态。
- "Object Code" → **"Object Form"** (§1.5: any non-Source-Form, including
  rendered, exported, generated, and mechanically transformed forms). /
  "Object Code" 改为 **"Object Form"**。
- "Licensed Material Source Code" → "Licensed Material in Source Form"
  throughout (§6.1–6.4, §11.2, §15.2). / 全文对应改写。
- §4.10(a) "proprietary software" → "proprietary or licensed exclusively to
  You". / 去除残余软件措辞。
- §2.1 verbs generalized (use, run, execute, display, perform, utilize). /
  §2.1 行为动词泛化。
- User Work examples now include documents, fonts, datasets, models alongside
  programs. / User Work 示例补充非软件形态。

## Not done / 未纳入

- **SPDX**: not applied for at this time (per decision). / SPDX 暂不申请（按
  决策）。
- Section renumbering: not used. / 未做章节重排。

## Review checklist / 审阅清单

1. §3.1 patent scope wording (Apache-style necessity + acquisition carve-out)
   — confirm intent. / 专利授权范围措辞请确认。
2. §11.5 automatic reinstatement window (60 days, first breach only) —
   confirm. / 自动复权窗口（60 天、仅首次）请确认。
3. §12.2 three Designation granularities (law only / law+exclusive forum /
   law+non-exclusive forum) — confirm. / 管辖指定的三档粒度请确认。
4. §6.4(e) embeddings carve-out wording — confirm. / 嵌入向量条款措辞请确认。
5. Preamble compression — confirm the shorter principles list. / 序言压缩后
   的原则清单请确认。
