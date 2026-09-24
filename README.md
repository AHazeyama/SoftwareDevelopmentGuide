> [!CAUTION]  
> This guide is continuously updated.  
> 現在作成途中です。随時更新いたします。
<p align="left">  
	<img src="assets/Title_dark.png#gh-dark-mode-only" alt="banner dark">  
	<img src="assets/Title_light.png#gh-light-mode-only" alt="banner light">  
</p>  

<!--  
<img src="assets/Title_light.png">  
-->  
  
### このガイドは特定の開発手法に依存せず、ウォーターフォール、アジャイル、小規模開発など、さまざまな開発形態で利用できることを目的としています。  
# Overview  
本リポジトリは、私が **個人的な** ソフトウェア開発で採用している設計思想・開発標準・手順をまとめたガイドです。  
特定の言語やフレームワークに依存せず、開発プロセス全体を標準化し、品質を安定させるために、 要件定義から設計、実装、テスト、ドキュメント作成、リリースまでを体系的に整理し、個人開発・受託開発の双方で再利用できることを目的としています。  
## 対象  
・個人開発者  
・小規模開発チーム  
・受託開発エンジニア  
## 要件定義   
業務内容やシステム化の目的を整理し、必要な機能・制約・対応範囲を明確化するためのガイド。  
ヒアリングシートや業務フロー、機能一覧など、開発の土台となる成果物を作成します。  
[<img src="./assets/env/M_file.png" height="14"> 要件定義](https://github.com/AHazeyama/SoftwareDevelopmentGuide/blob/main/docs/01_RequirementDefinition.md)  
## 基本設計  
システム全体の構成や画面、データ構造、機能の関連性を整理する工程。  
実装前にシステム全体の設計方針を明確にし、開発・保守しやすい構成を目指します。  
[<img src="./assets/env/M_file.png" height="14"> 基本設計](https://github.com/AHazeyama/SoftwareDevelopmentGuide/blob/main/docs/02_BasicDesign.md)  
## 詳細設計 (コーディング規約)  
クラス設計、関数設計、命名規則、ディレクトリ構成など、実装時のルールを定義。  
可読性・保守性・再利用性を重視したコーディング標準をまとめています。  
<!-- [🗋 詳細設計](docs/03_DetailDesign.md)  -->  
> [!NOTE]  
> <img src="./assets/env/M_file.png" height="14"> 詳細設計　**Scheduled for creation**  
## UI設計  
操作性・視認性・一貫性を重視したユーザーインターフェース設計のガイド。  
画面レイアウト、配色、ボタン配置、メッセージ表示など、ユーザーが迷わず操作できる設計を目指します。  
<!-- [<img src="./assets/env/M_file.png" height="14"> UI設計](docs/04_UIDesign.md)  -->  
> [!NOTE]  
> <img src="./assets/env/M_file.png" height="14"> UI設計　**Scheduled for creation**  
## ドキュメント作成  
ソースコードや設計情報を保守しやすい形で文書化するためのガイド。  
Doxygenを用いたAPIリファレンスの生成や、MarkdownによるREADME・設計書の作成方法など、継続的なドキュメント管理についてまとめています。  
<!-- [<img src="./assets/env/M_file.png" height="14"> ドキュメント作成](docs/05_Documentation.md)  -->  
> [!NOTE]  
> <img src="./assets/env/M_file.png" height="14"> ドキュメント作成　**Scheduled for creation**  
## Tutorial  
言語・開発環境ごとの標準構成や初期設定手順。  
新規プロジェクトを短時間で立ち上げ、同じ品質で開発を開始できることを目的としています。  
### 　DeskTop & Web  
&emsp; &emsp; &emsp; [<img src="./assets/env/M_tech-documents.png" height="18"> C# / WPF](https://github.com/AHazeyama/SoftwareDevelopmentGuide/blob/main/templates/exrm_WPF_VS2026.md)　　　　　# VisualStudioによるWPFアプリケーション開発手順  
&emsp; &emsp; &emsp; [<img src="./assets/env/M_tech-documents.png" height="18"> Python / PySide6](https://github.com/AHazeyama/SoftwareDevelopmentGuide/blob/main/templates/renm_ps6_Vim.md)　　# Terminal & Editor による開発手順  
### 　Mobile  
&emsp; &emsp; &emsp; [<img src="./assets/env/M_tech-documents.png" height="18"> Dart / Flutter](https://github.com/AHazeyama/public/blob/main/tmct_flt/tmct_flt_AndroidStudio.md)　　　　# AndroidStudioによるAPK開発手順  
## Git運用  
GitおよびGitHubを利用したソースコード管理方法。  
ブランチ運用、コミットルール、リリース管理など、継続的な開発を支える運用手順を定義します。  
<!-- [🗋 Git運用](docs/07_GitOperation.md)  -->  
> [!NOTE]  
> <img src="./assets/env/M_file.png" height="14"> Git運用　**Scheduled for creation**  
## Docker構築  
Dockerを利用した開発環境の構築手順。  
環境差異を最小限に抑え、再現性の高い開発環境を構築することを目的としています。  
<!-- [<img src="./assets/env/M_file.png" height="18"> Docker構築](docs/08_Docker.md)  -->  
> [!NOTE]  
> <img src="./assets/env/M_file.png" height="14"> Docker構築　**Scheduled for creation**  
## リリース手順  
アプリケーションのビルドから配布までの手順。  
動作確認、成果物作成、GitHub Releasesへの公開など、安定したリリースを行うための標準手順を定義します。  
<!-- [<img src="./assets/env/M_file.png" height="14"> リリース手順](docs/09_Release.md)  -->  
> [!NOTE]  
> <img src="./assets/env/M_file.png" height="14"> リリース手順　**Scheduled for creation**  
## 開発チェックリスト  
開発工程におけるチェックリスト。　　  
各項目完了時にレビューを行いチェックリストに記載します。  
<!-- [<img src="./assets/env/M_file.png" height="14"> 開発チェックリスト](docs/Development_Checklist.md)  -->  
> [!NOTE]  
> <img src="./assets/env/M_file.png" height="14"> 開発チェックリスト　**Scheduled for creation**  
## Future Plans  
- FastAPI Template  
- Flask Template  
- Tkinter Template  