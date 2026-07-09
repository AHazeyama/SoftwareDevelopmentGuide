> [!CAUTION]
> This guide is continuously updated.
<p align="left">
	<img src="assets/Title_dark.png#gh-dark-mode-only" alt="banner dark">
	<img src="assets/Title_light.png#gh-light-mode-only" alt="banner light">
</p>


# Overview
本リポジトリは、私がソフトウェア開発で採用している開発標準・手順・テンプレートをまとめたガイドです。  
特定の言語やフレームワークに依存せず、開発プロセス全体を標準化するために、 要件定義から設計、実装、テスト、ドキュメント作成、リリースまでを体系的に整理。  
個人開発・受託開発の双方で再利用できることを目的としています。  
## 対象
・個人開発者  
・小規模開発チーム  
・受託開発エンジニア  
## 要件定義 
業務内容やシステム化の目的を整理し、必要な機能・制約・対応範囲を明確化するためのガイド。  
ヒアリングシートや業務フロー、機能一覧など、開発の土台となる成果物を作成します。  
[📄要件定義](docs/01_RequirementDefinition.md)  
## 基本設計
システム全体の構成や画面、データ構造、機能の関連性を整理する工程。  
実装前にシステム全体の設計方針を明確にし、開発・保守しやすい構成を目指します。  
[📄基本設計](docs/02_BasicDesign.md)  
## 詳細設計 (コーディング規約)
クラス設計、関数設計、命名規則、ディレクトリ構成など、実装時のルールを定義。  
可読性・保守性・再利用性を重視したコーディング標準をまとめています。  
[📄詳細設計](docs/03_DetailDesign.md)  
## UI設計
操作性・視認性・一貫性を重視したユーザーインターフェース設計のガイド。  
画面レイアウト、配色、ボタン配置、メッセージ表示など、ユーザーが迷わず操作できる設計を目指します。  
[📄UI設計](docs/04_UIDesign.md)  
## ドキュメント作成
ソースコードや設計情報を保守しやすい形で文書化するためのガイド。  
Doxygenを用いたAPIリファレンスの生成や、MarkdownによるREADME・設計書の作成方法など、継続的なドキュメント管理についてまとめています。  
[📄ドキュメント作成](docs/05_Documentation.md)  
## 開発環境毎のテンプレート
言語・開発環境ごとの標準構成や初期設定テンプレート。  
新規プロジェクトを短時間で立ち上げ、同じ品質で開発を開始できることを目的としています。  
### C#  
　　Visual StudioによるWPFアプリケーション開発テンプレートです。  
　　[📄C# [WPF / VisualStudio]](templates/exrm_WPF_VS2026.md)  
### Python  
　　Python開発用テンプレートです。  
　　[📄Python [PySide6 / VisualStudio]](templates/renm_ps6_Vim.md)  
　　<!-- &emsp; &emsp; [📄Python [FastAPI / Vim]](docs/05_Documentation.md)  -->
## Git運用
GitおよびGitHubを利用したソースコード管理方法。  
ブランチ運用、コミットルール、リリース管理など、継続的な開発を支える運用手順を定義します。  
[📄Git運用](docs/07_GitOperation.md)  
## Docker構築
Dockerを利用した開発環境の構築手順。
環境差異を最小限に抑え、再現性の高い開発環境を構築することを目的としています。  
[📄Docker構築](docs/08_Docker.md)  
## リリース手順
アプリケーションのビルドから配布までの手順。
動作確認、成果物作成、GitHub Releasesへの公開など、安定したリリースを行うための標準手順を定義します。  
[📄リリース手順](docs/09_Release.md)    
## 開発チェックリスト
開発工程におけるチェックリスト。　　
各項目完了時にレビューを行いチェックリストに記載します。  
[📄開発チェックリスト](docs/Development_Checklist.md)  
## Future Plans
- FastAPI Template
- Flask Template
- PySide6 Template