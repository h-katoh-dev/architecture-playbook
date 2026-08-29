# Architecture Playbook

A public, practical knowledge base for learning and improving system architecture decision-making.

**日本語:** このリポジトリは、システムアーキテクチャの判断力を実践的に身につけるための公開ナレッジベースです。

## Purpose / 目的

This repository focuses on **why an architecture should be chosen**, not simply which technology to use.

このリポジトリでは、単に「どの技術を使うか」ではなく、**「なぜそのアーキテクチャを選ぶのか」**を重視します。

The goal is to develop the ability to:

- identify system responsibilities and boundaries
- generate multiple architecture options
- compare trade-offs
- reason about security, reliability, scalability, maintainability, and operations
- explain architectural decisions clearly
- review an existing architecture and identify risks

目標は、次の能力を身につけることです。

- システムの責務と境界を整理する
- 複数のアーキテクチャ案を考える
- メリット・デメリットやトレードオフを比較する
- セキュリティ、信頼性、スケーラビリティ、保守性、運用性を考える
- アーキテクチャ上の判断理由を説明する
- 既存アーキテクチャをレビューし、リスクを発見する

## Learning Loop / 学習ループ

```text
Requirement / 要件
    ↓
Responsibilities & boundaries / 責務・境界
    ↓
Architecture options / 構成案
    ↓
Trade-off analysis / トレードオフ分析
    ↓
Decision / 判断
    ↓
Review / feedback / レビュー・フィードバック
    ↓
Architecture Decision Record (ADR)
```

## Repository Structure / ディレクトリ構成

- `principles/` — fundamental architecture principles / アーキテクチャの基本原則
- `patterns/` — architecture patterns and when to use them / アーキテクチャパターンと適用条件
- `exercises/` — architecture design exercises / 設計演習
- `case-studies/` — realistic system design case studies / 実践的なケーススタディ
- `architecture-reviews/` — review checklists and review exercises / レビュー観点・レビュー演習
- `adr/` — documented architecture decisions and trade-offs / 設計判断とトレードオフの記録

## Public Repository Policy / 公開リポジトリのルール

This repository is intentionally public.

Do not commit:

- confidential or proprietary information
- customer or employer-specific information
- personal information
- credentials, secrets, tokens, or private URLs
- unreleased project details

Real-world experiences may be generalized and anonymized so that the underlying architectural lessons remain useful without exposing confidential information.

このリポジトリは意図的に公開しています。以下の情報はコミットしません。

- 機密情報・ proprietary information
- 顧客や勤務先を特定できる情報
- 個人情報
- 認証情報、秘密情報、トークン、非公開URL
- 未公開の案件情報

実案件の経験を扱う場合は、機密情報を含まないよう一般化・匿名化し、アーキテクチャ上の学びだけを残します。

## Relationship to dev-standard / dev-standardとの関係

`architecture-playbook` focuses on **architecture decisions and their reasoning**.

`dev-standard` focuses on **implementation standards and development rules**.

The two repositories may reference each other, but they serve different purposes.

`architecture-playbook` は**アーキテクチャの判断と、その判断理由**を扱います。

`dev-standard` は**実装標準と開発ルール**を扱います。

両リポジトリは相互に参照できますが、役割は明確に分けます。
