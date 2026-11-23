# Warm-Lead Conversion Playbook (from the Partner R pilot retrospective)

> Correctover commercial playbook v1 — 2026-11-21



## 一、Partner R 为什么愿意付费（四因复盘）

### 我们做对的（可复制）
1. **先免费交付可验真货，收货款不卖期货**
   - a crosswalk validation with six live test cases, pinned to a specific commit
   - independent profile issue + real test vectors + integration review, item by item
   - 付费时对方已见过全部交付物形态——信任攒出来的，不是谈出来的
2. **我们抓到过他们生态里的真问题**
   - a signature-verification gap in one of our own verifier tools自己扫出来当场补——证明眼睛真能看见别人看不见的
   - 对方「对 $2,500 开放+December窗口」= 采购方验货后的议价语气

### 对方的结构（不可复制但要找同类）
3. **「独立」是它业务结构的刚需**：它做 agent 集成验证，它的客户迟早问「谁证明你验证过」——vendor 自证无解，我们是唯一给可离线复验签名收据的第三方
4. **交易结构零摩擦**：$2,500 试点预算（不过采购委员会）｜December实验窗口=先试后买、风险在对方侧我们主动给台阶｜全程邮件异步零会议

## 二、可复制 SOP（暖线索复耕标准流程）

```
S1 选择：有过 ≥1 次真实互动的线索（回信/社区互动/用过我们的 verifier）
S2 免费件：实跑一件对方「本周就能用上」的验证资产
   - 形态候选：crosswalk 对其系统实跑 / corpus 向量组 / 一页可复现 PoC
   - 硬门槛：pin commit + 可离线复验 + 附赠不邀功
S3 留痕：资产公开可查（repo/issue），让对方被外部看到受益
S4 报价：小额试点锚 + 试后买结构（「先窗口后付款」）
   - Pricing discipline: pilot-anchor pricing with deliverable list + acceptance criteria; quoted orders never silently re-priced.
S5 节奏：零会议、全异步、零催——交付物自己会说话
S6 关闭判定：窗口到期无书面动作 → 3-strike 关闭，不续命
```

## 三、反模式（禁止）
- ❌ 上来就报价（Partner R 是四轮免费交付后才谈钱）
- ❌ 卖「我们很专业」（卖「你已收到的实跑结果」）
- ❌ 催单（Partner R December窗口前不主动催，备好实验输入材料即可）
- ❌ 会议邀约（对方没要求过任何会）
- ❌ 把「独立」说成特色形容词（说成对方业务结构的必需品）

## 四、批量应用
- 候选名单（有过互动的暖线索）：Partner R（模板客户，December窗口推进）、Steven Zhao、Konrad Gruszka（CCS 读者）、agentproto/Justin Kintzele（corpus 捐赠意向）、Vanta（已有线）、TRM Labs（已有线）
- 每个候选 S2 免费件由本 agent 按 S2 门槛定制，备草稿走三道关卡

---
*留存：2026-11-21 18:18 主人令「按这个流程去找客户」*

---
*Correctover — AI Agent action-layer independent audit. Evidence-first, offline re-verifiable.*

## Why It Worked — Validated Success Factors (2026-11)

Case evidence: two parallel USD 2,500 engagements (a Bounded Review and an integration-verification pilot) advanced through this same playbook. Post-mortem of both:

**Common root cause: deliver verifiable goods first. Trust is earned by artifacts, not negotiated.**

1. **Free artifact first, actually executed.** Crosswalk ran against six real cases, pinned to a specific commit, plus a standalone profile issue and real test vectors — by the time money was discussed, the buyer had already seen every deliverable shape.
2. **Found a real problem in their ecosystem, fixed it on the spot.** (A verifier signature-check gap in their stack, self-scanned, patched same day.) Proof that we see what others don't.
3. **Hit a structural need, not an adjective.** Integration-verification vendors eventually face the question "who verified *your* verification?" — vendor self-attestation has no answer. An independent third party with offline-verifiable signed receipts is the only resolution. Sell the structural gap, never "we're independent" as decoration.
4. **Zero-friction deal shape.** Pilot price below procurement-committee threshold; try-then-buy window keeps the risk on our side; fully async, zero meetings.

**Compounding channel note:** one buyer held both a paper co-author seat and the payment decision — every thread the paper advanced added trust to the commercial line automatically.

**Copyable formula:** free executed artifact (pinned, re-verifiable) → catch & fix a real problem on the spot → hit the structural need → small anchor + try-then-buy + async → let deliverables speak; never chase.

**Downside guards:** 3-strike close discipline; price anchoring by track (pilot USD 2,500 / new-client default USD 5,000); explicit walk-away criteria.
