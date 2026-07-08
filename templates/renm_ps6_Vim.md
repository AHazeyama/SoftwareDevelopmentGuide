# renm_PySide6_Vim
## OverView
目的 : PySide6を使用したアプリケーション開発  
内容 : ファイル/ディレクトリ名一括変換ツール[renm_ps6]  
|Item|Content|
|:--|:--|
|OS|![](./assets/logo_Windows11.png) / ![](./assets/logo_Ubuntu.png)|
|IDE|![](./assets/logo_Vim.png) ( Plugin, LSP追加 )|
|言語|![](./assets/logo_Python.png)|
|Framework|![](./assets/logo_PySide6.png)|

※ 記号例
```
⬇️:マウスクリック、"･･･":テキスト、a/b:選択(a or b)、｢･･･｣:ウィンドウ/メニュー/フォーム、
[･･･]:ボタン、<･･･>:Key、⇒:次動作、#･･･:コメント  
```
<br>

# ファイル/フォルダーの排他的削除ツール [exrm]作成手順
## 開発環境構築
### 仮想環境生成
　　![](assets/shell_P.png)
※｢.NET 10.0SDK｣をインストール (手順省略)  
　　Installer [Download](https://dotnet.microsoft.com/ja-jp/download/dotnet/10.0)  
※｢VisualStudioInstaller｣で、ワークロード｢.NETデスクトップ開発｣をインストール (手順省略)  
　　Source code [GitHub](https://github.com/AHazeyama/public/tree/main/exrm_wpf)

## VisualStudio起動
　[新しいプロジェクトの作成] ⬇️  
　｢新しいプロジェクトの作成｣  
　　｢テンプレートの検索｣で"WPF"を検索  
　　[WPF アプリケーション] ⬇️  
　　[次へ] ⬇️  
　｢新しいプロジェクトを構成します｣  
　　｢プロジェクト名｣に "exrm_wpf" 入力  
　　[…] ⬇️  
　　　保存ディレクトリ選択(省略) ⇒  ｢場所｣ ⬇️  
　　｢✅ソリューションとプロジェクトを同じディレクトリに配置する｣ ⬇️  
　　[作成] ⬇️  
　｢追加情報｣  
　　｢フレームワーク (F)｣  
　　　｢.NET 10.0 (長期的なサポート)｣ ⬇️  
　　[作成] ⬇️  
## UIモジュール作成  
　｢ソリューションエクスプローラー｣  
　　｢📄MainWindow.xaml｣ W⬇️  
　　｢MainWindow.xaml 📌 ✖｣ / ｢XAML｣  
　　　編集 (⚠️Link先はGUI実装済み)  
　　　　[MainWindow.xaml](https://github.com/AHazeyama/public/blob/main/exrm_wpf/MainWindow.xaml)
## イベント処理モジュール作成  
　｢ソリューションエクスプローラー｣  
　　｢📄MainWindow.xaml｣  
　　　｢C# MainWindow.xaml.cs｣ W⬇️  
　　｢MainWindow.xaml.cs 📌 ✖｣  
　　　編集 (⚠️Link先は下記実装済み)  
　　　　☆ 削除 ＋ バックアップ ＋ Undoロジック モジュール  
　　　　[MainWindow.xaml.cs](https://github.com/AHazeyama/public/blob/main/exrm_wpf/MainWindow.xaml.cs)  

## ロジックモジュール作成  
　｢ソリューションエクスプローラー｣  
　　｢exrm｣ 右⬇️ ⇒ ｢追加｣ ⬇️ ⇒ ｢新しい項目…｣ ⬇️  
　　　｢新しい項目の追加｣  
　　　　｢exrm/｣に"ExrmCore.cs"を入力  
　　　　　[追加] ⬇️  
　　　｢ExrmCore 📌 ✖｣  
　　　　編集 (⚠️Link先はイベント処理モジュール実装済み)  
　　　　　[ExrmCore.cs](https://github.com/AHazeyama/public/blob/main/exrm_wpf/ExrmCore.cs)
## クラス指定明確化  
　｢ソリューションエクスプローラー｣  
　　｢📄App.xaml｣  
　　　｢C# App.xaml.cs｣ W⬇️  
　　｢App.xaml.cs 📌 ✖｣  
　　　　編集  
　　　　　旧：public partial class App : Application  
　　　　　新：public partial class App : System.Windows.Application  
## プロジェクトファイル変更(WinFormsの有効化、単体起動exe作成コマンド)  
　｢ソリューションエクスプローラー｣  
　　｢exrm｣ 右⬇️ ⇒ ｢プロジェクト ファイルの編集｣ ⬇️  
　　　｢exrm 📌 ✖｣  
　　　　編集 (⚠️Link先はWinForm有効化 & 単体起動exe生成 実装済み)  
　　　　　[exrm_wpf.csproj](https://github.com/AHazeyama/public/blob/main/exrm_wpf/exrm_wpf.csproj)  
## テスト環境構築  
　｢ソリューションエクスプローラー｣  
　　｢exrm｣ 右⬇️ ⇒ ｢追加｣ ⬇️ ⇒ ｢新しい項目…｣ ⬇️  
　　　｢新しい項目の追加｣  
　　　　｢exrm/｣に"mktest.ps1"を入力  
　　　　[追加] ⬇️  
　｢mktest 📌 ✖｣  
　　![](assets/shell_P.png)
```PowerShell
　　 #! /usr/bin/pwsh  
　　 # Resuires -Version 7.4  
　　 # Test環境構築スクリプト。実行はGit登録後に行います。  
　　 mkdir test1st  
　　 cd test1st  
　　 New-Item test_11.txt  
　　 New-Item test_12.txt  
　　 New-Item work_11.txt  
　　 New-Item work_12.txt  
　　 mkdir test2nd  
　　 cd test2nd  
　　 New-Item test_21.txt  
　　 New-Item test_22.csv  
　　 New-Item work_21.txt  
　　 New-Item work_22.csv  
　　 cd ..  
　　 mkdir test3rd  
　　 cd test3rd  
　　 New-Item test_31.txt  
　　 New-Item test_32.csv  
　　 New-Item work_31.txt  
　　 New-Item work_32.csv  
　　 cd ..  
　　 mkdir work4th  
　　 cd work4th  
　　 New-Item work_41.txt  
　　 New-Item work_42.txt  
　　 cd ../..  
　　 Write-Host "`r`n ---- Test Environment ----" -Foreground Cyan  
　　 tree /f test1st  
```
## バージョン管理登録(Git)  
　｢Gitリポジトリの作成｣  
　　左ペインの｢ローカル｣ ⬇️  # 今回はローカルのみ  
　　　｢□ README.mdの追加｣にチェック  
　　[作成とプッシュ] ⬇️  
### Git README.md 編集  
　｢ソリューションエクスプローラー｣  
　　アイコン列から"すべてのファイルを表示" ⬇️  
　　　｢📄README.md｣ 右⬇️ ⇒ ｢プロジェクトに含める｣ ⬇️  
　　　｢📄README.md｣ W⬇️  
　　　｢README.md 📌 ✖｣  
　　　　![](assets/logo_Markdown.png) 編集  
　　　　GitHub [README.md](https://github.com/AHazeyama/public/blob/main/exrm_wpf/README.md)  
　　　｢📄プレビューを開く｣ ⬇️  
## ターミナル表示  
　　｢表示｣ ⇒ ｢ターミナル｣ ⬇️  
### Test環境構築  
　｢Developer PowerShell 7 📌 ✖｣  
　　![](assets/shell_P.png)  
```PowerShell
　　　　　　./mktest.ps1 <⏎>  
```
## 動作確認  
### アプリ起動  
　　｢VisualStudio｣  
　　　　・上部のアイコンから[▶ 実行] ⬇️  
### 試行 ( 🗀test1st で実施 )
1. ｢**Select**｣ をクリックし、**Exec directory** を選択
2. **not removed words** に**削除除外対象**に含まれる文字列を指定  
3. ｢**Scan**｣ をクリックし、**Prossesing nessage** に表示される削除対象を確認  
複数指定する場合は "**,**" で区切って下さい
4. **☑ Recursive processing** で、下位階層に対する処理の可否を選択 
5. ｢**Delete**｣ をクリックして実行
6. 必要に応じて ｢**Undo**｣ で元に戻す
<br>

## 単体アプリ作成  
  
### Visual Studio  

🔷 アイコン準備  
　　§ .ico ファイルを用意（256x256含むもの推奨）  
　　§ プロジェクトに追加  
　　　⇒ ソリューションエクスプローラー  
　　　⇒ 右クリック「追加」 ⇒ 「既存の項目」  
🔷 アプリにアイコンを設定  
　　WPF / WinForms 共通  
　　　i. プロジェクト右クリック  
　　　ii. 「プロパティ」  
　　　iii. 「アプリケーション」  
　　　iv. 「アイコンとマニフェスト」  
　　　v.  アイコン選択  
🔷 csproj 直接設定（確実）  
　　.csproj に追加：  
　　｢exrm_wpf｣ 右⬇️  
　　　｢プロジェクトファイルの編集｣ ⬇️  
　　![](assets/logo_XML.png)
```xml
　　<PropertyGroup>  
　　　　<PublishSingleFile>true</PublishSingleFile>  
　　　　<SelfContained>true</SelfContained>  
　　　　<RuntimeIdentifier>win-x64</RuntimeIdentifier>  
　　　　<ApplicationIcon>app.ico</ApplicationIcon>  
　　</PropertyGroup>  
```
🔷 単一exe化（Single File Publish）  
　　「公開」「現在公開している場所」「ターゲット」  
　　　「🗀 フォルダー」️ ⬇️ ⇒ [次へ(N)] ️⬇️  
　　「公開」「どのローカルターゲットに発行しますか」「特定のターゲット」  
　　　「🗀 フォルダー」️ ⬇️ ⇒ [次へ(N)]️ ⬇️  
　　「公開」「ローカルまたはネットワークフォルダーへのパスを指定してください」「場所」  
　　　「フォルダーの場所」👈指定 ⇒ [参照'(R)…] ⬇️ ⇒ [完了(F)] ⬇️  
　　「実行プロファイル作成の進行状況」[完了]  
　　　[閉じる] ⬇️  
　　[発行]️ ⬇️：👈exeが作成される (言葉が解りにくい<font size="5">😾</font>)  
🔷 公開結果 ⇒ <font size="5">🪰</font>デバッグ (勝手にやって<font size="5">😎</font>)  
　📦 出力先  
　　　🗀 : exrm_wpf\bin\Release\net10.0-windows\win-x64\publish  
　　単体起動exeは"publish"に出力される。  
> [!CAUTION]
> ⚠️ 🗀 win-x64 以下のexeは **.dll** が必要( **️単体ではない** )。  
  
### Visual Studio使わない方法  
プロジェクトフォルダ（.csproj がある場所）で  
　　![](assets/shell_P.png)  
```PowerShell
　　dotnet publish -c Release -r win-x64 --self-contained true -p:PublishSingleFile=true -p:IncludeNativeLibrariesForSelfExtract=true <⏎>  
```
　📦 出力先  
　　　bin\Release\net10.0-windows\win-x64\publish\  

## Git 更新 (README.md、exrm.exe)  
　｢VisualStudio｣  
　　右下の｢🖋️アイコン｣ ⬇️  
　｢Git 変更｣  
　　変更 / 追加したファイルをフォーカスし｢＋｣ ⬇️  
　　　｢メッセージを入力してください <必須>｣ にコメント入力  
　　[すべてをコミット] ⬇️  