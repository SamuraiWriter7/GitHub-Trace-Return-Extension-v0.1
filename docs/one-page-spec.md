# GitHub Trace Return Extension v0.1
## One-Page Specification

## What this is

**GitHub Trace Return Extension v0.1** は、AI時代の公開貢献フローに対して、  
**痕跡の可視化・寄与推定・限定的還元**を追加するための、  
**公開リポジトリ限定・明示同意型の拡張仕様案**である。

この仕様は、GitHub上ですでに存在する以下のような部品と整合することを前提とする。

- リポジトリ設定
- メタデータ管理
- 依存関係グラフ
- 使用量レポート
- GitHub Sponsors
- クレジット型の内部還元レール

本仕様の目的は、AI時代において強化されつつある  
**吸収・改善・集約の回路**に対し、  
**開示・還元・還流の回路**を接続することである。

---

## Core Question

> 吸収が制度化されたなら、還元はどう接続されるべきか。

---

## Core Model

現在のAI支援開発環境は、構造的に次の回路を強めやすい。

```text id="51522"
public trace → improvement → platform value concentration

本仕様は、そこに次の返還層を追加する。

public trace → improvement → platform value → trace report → limited return

これは完全な因果証明の仕組みではない。
あくまで、透明な寄与推定にもとづく限定的な還元層である。

Yin / Yang Structure

本仕様は、AI文明の制度設計を陰陽構造として捉える。

陰 = 吸収 / 改善 / 集約
陽 = 開示 / 還元 / 還流

GitHub的なAI基盤が陰を強化するほど、
社会的正当性と長期的安定性のためには、陽の構造が必要になる。

Scope

本仕様の初期対象は、公開リポジトリのみとする。

Included
公開リポジトリ単位の opt-in
痕跡可視化
寄与メトリクス
月次レポート
限定的還元
Excluded
private repository の詳細追跡
完全な著作権裁定
厳密なモデル重み由来証明
全派生物への完全分配
遡及的な全面救済
Design Principles
1. Public-first

まずは公開領域から始める。
非公開領域を無理に巻き込まない。

2. Explicit opt-in

参加は明示同意制とし、デフォルト参加にはしない。

3. Transparent estimation

完全証明ではなく、説明可能な推定を採用する。

4. Limited return before perfect fairness

完全公平を待つのではなく、限定的還元を先に始める。

5. Anti-gaming by design

スパム、複製、フォーク水増しを防ぐ。

6. Reuse existing primitives

新たな巨大基盤を一から作るのではなく、既存のGitHub機能を部品として使う。

Minimal Repository Metadata

参加リポジトリは、以下のような設定ファイルを持つ。

推奨パス

.github/trace-return.yml

最小例

trace_return:
  enabled: true
  version: "0.1"
  scope: public_repository_only
  attribution_mode: interaction_estimate
  monthly_report: true
  return_rail: github_sponsors

anti_gaming:
  fork_deduplication: true
  score_cap: true
  spam_filter: basic

maintainer:
  sponsors_handle: example-maintainer
Contribution Estimation

本仕様は、寄与を「絶対真理」としてではなく、
説明可能なスコアリング層として扱う。

Main signal groups
A. Structural signal
依存関係上の中心性
再利用されやすさ
ドキュメント整備
参照頻度
B. Maintenance signal
PR受理実績
issue整理の質
継続的更新
リリース持続性
C. Interaction signal
public discussion の密度
サンプルやテンプレートの有用性
教育的価値
パターン明瞭性
D. Quality signal
重複の少なさ
スパム性の低さ
リポジトリの一貫性
異常挙動の少なさ
Example Score Model
trace_score =
  structural_signal * 0.35
+ maintenance_signal * 0.25
+ interaction_signal * 0.25
+ quality_signal * 0.15

これは一例であり、固定値ではない。
重要なのは、不可視の抽出より、可視の推定のほうが健全であるという点である。

Monthly Trace Ledger

各参加リポジトリには、月次で痕跡レポートを返すことを想定する。

Example fields
month: "2026-05"
repository: "example-org/example-repo"
trace_return_enabled: true

estimated_trace_score: 78.4
signal_breakdown:
  structural_signal: 31.2
  maintenance_signal: 18.6
  interaction_signal: 20.1
  quality_signal: 8.5

return_recommendation:
  rail: github_sponsors
  suggested_return_tier: medium

anti_gaming_review:
  passed: true
  notes: "No major duplication anomalies detected."

この台帳は、すべての下流価値に対する所有権証明ではない。
これは、痕跡の可視化と還元判断のための軽量台帳である。

Return Rails

本仕様では、還元レールを段階的に定義する。

Phase A: GitHub Sponsors

もっとも現実的な第一段階。
既存の支援導線をそのまま使える。

Phase B: Copilot Credits

Copilot利用クレジットとして還元する。
プラットフォーム内部で循環しやすい。

Phase C: Actions Credits

CI/CD実行コスト軽減として還元する。
OSS保守者への実利が大きい。

Phase D: Hybrid

Sponsors、Copilot Credits、Actions Credits を併用する。

Governance
Participation requirements
公開リポジトリであること
maintainer の明示同意があること
設定ファイルが存在すること
レポート対象が説明可能であること
Exclusion triggers
明白なスパム
自動複製による水増し
フォーク乱造
低品質大量生成
身元の不整合
Governance requirements
スコアリング変更のバージョン管理
説明可能性
異議申立て余地
ポリシー更新の文書化
Anti-Gaming Baseline

還元制度は、対策なしではノイズ吸引機になる。
そのため、最低限以下を備える。

fork deduplication
score cap
quality threshold
anomaly detection
repository continuity check
maintainer consistency check
Why this matters

この仕様は、AI改善そのものを止めるためのものではない。
また、公開知の循環を否定するものでもない。

本仕様が問うのはただ一つである。

公開痕跡がプラットフォーム価値を生むなら、
そこに何らかの可視的な還元経路が存在すべきではないか。

この問いに対し、
本仕様は 制度として最小限に動く答え を与える。

One-Sentence Summary

Trace Return Extension v0.1 は、AI時代の公開貢献フローに、
痕跡の可視化・寄与推定・限定的還元を接続するための、公開先行・明示同意型の拡張仕様である。

Status
Draft Proposal
README-aligned One-Page Spec
Version: v0.1
