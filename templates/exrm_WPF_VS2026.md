<p akugb=:keft>  
	<img src="./assets/Title_exrm_dark.png#gh-dark-mode-only" alt="banner dark">  
	<img src="./assets/Title_exrm_light.png#gh-light-mode-only" alt="banner light">  
</p>  

<!--
<img src="./assets/Title_exrm_light.png">  
-->

# OverView  
目的 : VisualStudioを使用したアプリケーション開発  
内容 : 排他的ファイル/ディレクトリ削除ツール [exrm_wpf]  

|Item|Content|
|:--|:--|
|OS|<img src="./assets/env/M_OS_Win11.png" height="13">|  
|IDE|<img src="./assets/env/M_IDE_VisualStudio2026.png" height="18">|  
|Language|<img src="./assets/env/M_LANG_Csharp.png" height="14">　**/**　<img src="./assets/env/M_LANG_XML.png" height="16">　**/**　<img src="./assets/env/M_LANG_Markdown.png" height="16">  
|Framework|<img src="./assets/env/M_FW_dotnet10.png" height="14"> <img src="./assets/env/M_FW_WPF.png" height="12">|
|SHELL|<img src="./assets/env/M_SHELL_PowerrShell.png" height="13">
> [!caution]
> Trademarks: Company names, product names, and logos used in documents related to this project are trademarks or registered trademarks of their respective owners. They are cited solely for the purpose of describing the technologies used.
 

> [!NOTE]  
> ※ 凡例  
> 　<img src="./assets/env/M_monitor.png" height="14"> デスクトップ、️<img src="./assets/env/M_click.png" height="14">：マウスクリック、 <img src="./assets/env/M_button.png" height="14">：ボタン、<img src="./assets/env/M_key.png" height="14">：Press the Key、<img src="./assets/env/M_return.png" height="12">：Enter key press、  
> 　<img src="./assets/env/M_text.png" height="14">：テキスト、**a** / **b**：選択(**a** or **b**)、<img src="./assets/env/M_menu.png" height="11">：ウィンドウ/メニュー/フォーム、⇒：次動作、<img src="./assets/env/M_comment.png" height="12">：コメント、  
> <img src="./assets/env/M_win.png" height="14">：ウィンドウ / ペイン / ダイアログ 、<img src="./assets/env/M_term.png" height="14">：ターミナル、 <img src="./assets/env/M_write.png" height="14"> : 編集 / コーディング / 描画  
> <img src="./assets/env/M_copy.png" height="14">：クリックでText表示 (表示されたTextの右上にある <img src="./assets/env/M_git-copy.png" height="14"> <img src="./assets/env/M_click.png" height="14"> でコピー)  
> 縮小表示されている画像は <img src="./assets/env/M_click.png" height="14"> で拡大されます (マウスカーソルが <img src="./assets/env/M_info.png" height="14"> になる画像が縮小表示画像です)。  
>
> <img src="./assets/env/M_infoG.png" height="14"> ブラウザを **Darkモード** にして頂けると、見やすくなります。  

# ファイル/フォルダーの排他的削除ツール [exrm]作成手順

※｢.NET 10.0SDK｣をインストール (手順省略)  
　　[<img src="./assets/env/M_link.png" height="14"> Installer ](https://dotnet.microsoft.com/ja-jp/download/dotnet/10.0)  
※｢VisualStudioInstaller｣で、ワークロード｢.NETデスクトップ開発｣をインストール (手順省略)  
　　[<img src="./assets/env/M_link.png" height="14"> Source code / GitHub](https://github.com/AHazeyama/public/tree/main/exrm_wpf)

## VisualStudio起動
　<img src="./assets/env/M_monitor.png" height="14"> タスクバーの
<img src="./assets/env/M_menu-L.png" height="12">
<img src="./assets/env/M_OS_Win11icon.png" height="14"> 
<img src="./assets/env/M_menu-R.png" height="12">
<img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">
　<img src="./assets/env/M_menu-L.png" height="14">
<img src="./assets/env/M_IDE_VisualStudioInsiders.png" height="18">｣ <img src="./assets/env/M_click.png" height="14">  
　<img src="./assets/prtsc/M_VS_new-prj.png">
 <img src="./assets/env/M_click.png" height="14">  
　　<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> 新しいプロジェクトの作成 <img src="./assets/env/M_menu-R.png" height="12">  
　　　<img src="./assets/env/M_menu-L.png" height="12" align="top">
<img src="./assets/prtsc/M_VS_MENU-search.png" height="24">
<img src="./assets/env/M_menu-R.png" height="12">  で <img src="./assets/env/M_text-LR.png" height="12">WPF<img src="./assets/env/M_text-LR.png" height="12"> を検索  
　　　　<img src="./assets/env/M_menu-L.png" height="12" align="top">
<img src="./assets/prtsc/M_VS_MENU_wpf-app-menu.png" height="32">
<img src="./assets/env/M_menu-R.png" height="12">
<img src="./assets/env/M_click.png" height="14">
<img src="./assets/env/M_next.png" height="14">
<img src="./assets/prtsc/M_VS_BTN_next.png" height="14"> 
<img src="./assets/env/M_click.png" height="14">  
　　<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> 新しいプロジェクトを構成します <img src="./assets/env/M_menu-R.png" height="12">  
　　　<img src="./assets/env/M_menu-L.png" height="12" align="top"> 
<img src="./assets/prtsc/M_VS_new-prj-name.png" height="32">
<img src="./assets/env/M_menu-R.png" height="12"> に 
<img src="./assets/env/M_text-LR.png" height="12">exrm_wpf<img src="./assets/env/M_text-LR.png" height="12"> を入力 
<img src="./assets/env/M_next.png" height="14">  
　　　<img src="./assets/env/M_menu-L.png" height="12" align="top"> 
<img src="./assets/prtsc/M_VS_new-prj-name.png" height="32">
<img src="./assets/env/M_menu-R.png" height="12"> に 
<img src="./assets/env/M_text-LR.png" height="12">保存先<img src="./assets/env/M_text-LR.png" height="12"> を入力、または  
　　　<img src="./assets/env/M_button-L.png" height="12"> …
<img src="./assets/env/M_button-R.png" height="12">
<img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">　保存先を選択  
　　　<img src="./assets/env/M_menu-L.png" height="12">
<img src="./assets/env/M_check.png" height="12">
<img src="./assets/env/M_menu-R.png" height="12">
ソリューションとプロジェクトを同じディレクトリに配置する
<img src="./assets/env/M_click.png" height="14">
<img src="./assets/env/M_next.png" height="14">
<img src="./assets/prtsc/M_VS_BTN_next.png" height="14"> 
<img src="./assets/env/M_click.png" height="14">  
　<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> 追加情報 <img src="./assets/env/M_menu-R.png" height="12">  
　　　<img src="./assets/env/M_menu-L.png" height="12" align="top">
<img src="./assets/prtsc/M_VS_new-framework.png" height="32">
<img src="./assets/env/M_menu-R.png" height="12"> は 
<img src="./assets/env/M_text-LR.png" height="12"> `.NET 10.0(長期的なサポート)` <img src="./assets/env/M_text-LR.png" height="12"> を選択
<img src="./assets/env/M_next.png" height="14">
<img src="./assets/prtsc/M_VS_BTN_create.png" height="14">
<img src="./assets/env/M_click.png" height="14">  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　<img src="./assets/prtsc/M_VS_creating.png" width="256">  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　[<img src="./assets/prtsc/M_VS_WIN_visualstudio01.png" width="320">](./assets/prtsc/M_VS_PANE_all.png)  

## UIモジュール作成  
<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> ソリューションエクスプローラー <img src="./assets/env/M_menu-R.png" height="12">  
　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/env/M_file.png" height="14"> Mainwindow.xaml <img src="./assets/env/M_menu-R.png" height="12"> W <img src="./assets/env/M_click.png" height="14">  
　　<img src="./assets/prtsc/M_VS_PANE_solution-explorer01.png" >  
　　　　　　　　　　<img src="./assets/env/M_allow-D.png" height="14" align="top">  
　　[<img src="./assets/prtsc/M_VS_PANE_mainwindow-xaml.png" width="240">](./assets/prtsc/M_VS_PANE_mainwindow-xaml.png)
　<img src="./assets/env/M_allow-R.png" height="14" align="top">
　[<img src="./assets/prtsc/M_VS_PANE_mainwindow-xaml-after.png" width="240">](./assets/prtsc/M_VS_PANE_mainwindow-xaml-after.png)  
　　編集 (<img src="./assets/env/M_caution.png" height="14"> Link先はGUI実装済み)  
　　　[<img src="./assets/env/M_link.png" height="14"> MainWindow.xaml](https://github.com/AHazeyama/exrm_wpf/blob/main/MainWindow.xaml)  

## イベント処理モジュール作成  
<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> ソリューションエクスプローラー <img src="./assets/env/M_menu-R.png" height="12">  
　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/env/M_file.png" height="14"> C# Mainwindow.xaml.cs <img src="./assets/env/M_menu-R.png" height="12"> 
 <img src="./assets/env/M_click.png" height="14">  
　　<img src="./assets/prtsc/M_VS_PANE_solution-explorer02.png" >  
　　　　　　　　　<img src="./assets/env/M_allow-D.png" height="14" align="top">  
　　[<img src="./assets/prtsc/M_VS_PANE_mainwindow-xaml-cs.png" width="240">](./assets/prtsc/M_VS_PANE_mainwindow-xaml-cs.png)　
<img src="./assets/env/M_allow-R.png" height="14" align="top">　
[<img src="./assets/prtsc/M_VS_PANE_mainwindow-xaml-cs-after.png" width="240">](./assets/prtsc/M_VS_PANE_mainwindow-xaml-cs-after.png)  
　　<img src="./assets/env/M_LANG_Csharp.png" height="14"> <img src="./assets/env/M_write.png" height="14"> : **削除** ＋ **バックアップ** ＋ **Undo** の各ロジックモジュール付加  
　　　[ <img src="./assets/env/M_link.png" height="14"> MainWindow.xaml.cs](https://github.com/AHazeyama/exrm_wpf/blob/main/MainWindow.xaml.cs)　　　　　　<img src="./assets/env/M_comment-F.png" height="12"> <img src="./assets/env/M_caution.png" height="14"> Link先は <img src="./assets/env/M_write.png" height="14"> 済み  

## ロジックモジュール作成  
　<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> ソリューションエクスプローラー <img src="./assets/env/M_menu-R.png" height="12">   
　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_exrm-wpf.png"> <img src="./assets/env/M_menu-R.png" height="12"> 右 <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14"> 
　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_addition.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_next.png" height="14">
　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_new-item.png" height="12"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  
　　[<img src="./assets/prtsc/M_VS_PANE_solution-explorer03 .png" width="320">](./assets/prtsc/M_VS_PANE_solution-explorer03%20.png)  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　<img src="./assets/prtsc/M_DLG_add-new-item.png" width="256" align="top"> <img src="./assets/env/M_text-LR.png" height="12"> ExrmCore.cs <img src="./assets/env/M_text-LR.png" height="12"> 指定 <img src="./assets/env/M_next.png" height="14" align="top">
<img src="./assets/prtsc/M_VS_BTN_addition.png" height="14"> <img src="./assets/env/M_click.png" height="14">  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　[<img src="./assets/prtsc/M_VS_PANE_add-exrmcore-cs.png" width="320">](./assets/prtsc/M_VS_PANE_add-exrmcore-cs.png)  
　　<img src="./assets/env/M_LANG_Csharp.png" height="14"> <img src="./assets/env/M_write.png" height="14"> : ロジックモジュール付加  
　　　[<img src="./assets/env/M_link.png" height="14"> ExrmCore.cs](https://github.com/AHazeyama/exrm_wpf/blob/main/ExrmCore.cs)　　　　　　　　　　　<img src="./assets/env/M_comment-F.png" height="12"> <img src="./assets/env/M_caution.png" height="14"> Link先は <img src="./assets/env/M_write.png" height="14"> 済み  

## クラス指定明確化  
　<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> ソリューションエクスプローラー <img src="./assets/env/M_menu-R.png" height="12">  
　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_app-xaml-cs.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> W <img src="./assets/env/M_click.png" height="14">  
　　<img src="./assets/prtsc/M_VS_PANE_solution-explorer04.png">  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　[<img src="./assets/prtsc/M_VS_PANE_app-xaml-cs.png" height="128">](./assets/prtsc/M_VS_PANE_app-xaml-cs.png)　
<img src="./assets/env/M_allow-R.png" height="14" align="top">　
[<img src="./assets/prtsc/M_VS_PANE_app-xaml-cs-after.png" height="128">](./assets/prtsc/M_VS_PANE_app-xaml-cs-after.png)  

<details>  
<summary>  
<img src="./assets/env/M_copy.png" height="14">  
<img src="./assets/env/M_LANG_Csharp.png" height="14"> <img src="./assets/env/M_write.png" height="14"> : クラス名追記  

　　　旧：<img src="./assets/prtsc/M_VS_TEXT_application.png">  
　　　新：<img src="./assets/prtsc/M_VS_TEXT_application-after.png">  
</summary>  
  
```  
public partial class App : System.Windows.Application
```  
</details>  

## プロジェクトファイル変更 (WinForms有効化 & 単一EXE配布設定)  
　<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> ソリューションエクスプローラー <img src="./assets/env/M_menu-R.png" height="12">  
　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_exrm-wpf.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> 右 <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_editing-project-files.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  
　　<img src="./assets/prtsc/M_VS_PANE_solution-explorer05.png">   
　　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　[<img src="./assets/prtsc/M_VS_PANE_exrm-wpf-csproj.png" width="320">](./assets/prtsc/M_VS_PANE_exrm-wpf-csproj.png)  
　　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　[<img src="./assets/prtsc/M_VS_PANE_exrm-wpf-csproj-1st.png" width="320">](./assets/prtsc/M_VS_PANE_exrm-wpf-csproj-1st.png)  

<details>  
<summary>
<img src="./assets/env/M_copy.png" height="14">  
<img src="./assets/env/M_LANG_XML.png" height="14"> <img src="./assets/env/M_write.png" height="14"> : WinForms有効化、単体起動(.exe)作成コマンド追加  
</summary>  
  
```  
    <!-- ここから配布用設定 -->
    <RuntimeIdentifier>win-x64</RuntimeIdentifier>  
    <SelfContained>true</SelfContained>  
    <PublishSingleFile>true</PublishSingleFile>  
    <IncludeNativeLibrariesForSelfExtract>true<IncludeNativeLibrariesForSelfExtract>  
    <EnableCompressionInSingleFile>true</EnableCompressionInSingleFile>  
```  
</details>  

## テスト環境構築  
　<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> ソリューションエクスプローラー <img src="./assets/env/M_menu-R.png" height="12">   
　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_exrm-wpf.png"> <img src="./assets/env/M_menu-R.png" height="12"> 右 <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">
　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_addition.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_next.png" height="14">
　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_new-item.png" height="12"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  
　　[<img src="./assets/prtsc/M_VS_PANE_solution-explorer03 .png" width="320">](./assets/prtsc/M_VS_PANE_solution-explorer03%20.png)  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　 <img src="./assets/prtsc/M_DLG_add-new-item.png" width="256" align="top"> <img src="./assets/env/M_text-LR.png" height="12"> mktest.ps1 <img src="./assets/env/M_text-LR.png" height="12"> 指定 <img src="./assets/env/M_next.png" height="14" align="top">
<img src="./assets/prtsc/M_VS_BTN_addition.png" height="14"> <img src="./assets/env/M_click.png" height="14">  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　[<img src="./assets/prtsc/M_VS_PANE_mktest-ps1.png" height="128">](./assets/prtsc/M_VS_PANE_exrm-wpf-after.png)
<details>  
<summary>
<img src="./assets/env/M_copy.png" height="14">  
<img src="./assets/env/M_SHELL_PowerrShell.png" height="12"> <img src="./assets/env/M_write.png" height="14"> Source code　　　<img src="./assets/env/M_comment-F.png" height="12"> <img src="./assets/env/M_copy.png" height="14"> <img src="./assets/env/M_click.png" height="14"> <img src="./assets/prtsc/M_COM_001.png" height="14">
</summary>  
  
```  
#!/usr/bin/pwsh
#Requires -Version 7.0
mkdir test1st
cd test1st
New-Item test_11.txt
New-Item test_12.txt
New-Item work_11.txt
New-Item work_12.txt
New-Item dummy_11.txt
New-Item dummy_12.txt
mkdir test2nd
cd test2nd
New-Item test_21.txt
New-Item test_22.csv
New-Item work_21.txt
New-Item work_22.csv
New-Item dummy_11.txt
New-Item dummy_12.txt
cd ..
mkdir test3rd
cd test3rd
New-Item test_31.txt
New-Item test_32.csv
New-Item work_31.txt
New-Item work_32.csv
New-Item dummy_11.txt
New-Item dummy_12.txt
cd ..
mkdir work4th
cd work4th
New-Item work_41.txt
New-Item work_42.txt
cd ../..
# & c_write "Cyan" "`r`n --- Test Environment ----"
Write-Host "`r`n --- Test Environment ---" -Foreground Cyan
tree /f test1st
```  
</details>  

## バージョン管理登録(Git)  
### Gitリポジトリの作成  
　<img src="./assets/env/M_win.png" height="14" align="top">
<img src="./assets/prtsc/M_VS_MENU_icon.png" align="top"> 右下の 
<img src="./assets/env/M_menu-L.png" height="12" align="top"> 
<img src="./assets/prtsc/M_VS_MENU_source-control.png" height="14" align="top"> 
<img src="./assets/env/M_menu-R.png" height="12" align="top"> 
<img src="./assets/env/M_click.png" height="14" align="top">　
 <img src="./assets/env/M_allow-R.png" height="14" align="top">　
<img src="./assets/env/M_menu-L.png" height="12" align="top"> 
<img src="./assets/prtsc/M_VS_MENU_git.png" height="14" align="top"> 
<img src="./assets/env/M_menu-R.png" height="12" align="top"> 
<img src="./assets/env/M_click.png" height="14" align="top">  
　　<img src="./assets/prtsc/M_VS_WIN_add-source-control.png" width="320">  
　　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　<img src="./assets/env/M_menu-L.png" height="12" align="top"> <img src="./assets/prtsc/M_VS_MENU_git-local.png" height="14" align="top"> <img src="./assets/env/M_menu-R.png" height="12" align="top"> <img src="./assets/env/M_click.png" height="14" align="top"> <img src="./assets/env/M_next.png" height="14" align="top">　
<img src="./assets/env/M_menu-L.png" height="12" align="top"> <img src="./assets/prtsc/M_VS_CHK_git-readme-on.png" height="14" align="top"> <img src="./assets/env/M_menu-R.png" height="12" align="top"> <img src="./assets/env/M_click.png" height="14" align="top">　
<img src="./assets/env/M_menu-L.png" height="12" align="top"> <img src="./assets/prtsc/M_VS_MENU_git-create.png" height="14" align="top"> <img src="./assets/env/M_menu-R.png" height="12" align="top"> <img src="./assets/env/M_click.png" height="14" align="top">  
　　<img src="./assets/prtsc/M_VS_WIN_git-creating-ripository.png" width="256">  

> [!NOTE]
> Gitをローカルに作成します (GitHubへの登録は別途)  

　　<img src="./assets/prtsc/M_VS_PANE_solution-explorer07.png">  
　　Gitリポジトリ作成で付加されるファイル  
　　　<img src="./assets/prtsc/M_VS_FILE_gitattributes.png"> : Gitでのファイル/フォルダの属性(改行コード、差分表示等の設定)  
　　　<img src="./assets/prtsc/M_VS_FILE_gitignore.png"> 　: GitHubへのPushルール  
　　　<img src="./assets/prtsc/M_VS_FILE_readme-md.png"> : GitHubで表示されるREADME <img src="./assets/env/M_LANG_Markdown.png" height="14">  

### Git README.md 編集  
　　<img src="./assets/env/M_LANG_Markdown.png" height="16" align="top"> <img src="./assets/env/M_write.png" height="14" align="top">　:　<img src="./assets/env/M_link.png" height="14" align="top"> [<img src="./assets/prtsc/M_GIT_VIEW_readme.png" width="240" align="top">](https://github.com/AHazeyama/exrm_wpf)  
　　　Source code [<img src="./assets/env/M_link.png" height="14"> README.md](https://github.com/AHazeyama/exrm_wpf/edit/main/README.md)  
 
## Debug用DIR作成
　<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> ソリューションエクスプローラー <img src="./assets/env/M_menu-R.png" height="12">   
　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_display.png"> <img src="./assets/env/M_menu-R.png" height="12"> 右 <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">　
<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_terminal.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  
　　<img src="./assets/prtsc/M_VS_PANE_power-shell01.png" width="320">  
<details>  
<summary>
<img src="./assets/env/M_copy.png" height="14">  
<img src="./assets/prtsc/M_VS_CMD_mktest-ps1.png">
&nbsp;<img src="./assets/env/M_return.png" height="12">  
</summary>  
  
```  
.\mktest.ps1  
```  
</details>  

　　[<img src="./assets/prtsc/M_VS_PANE_power-shell-mktest.png" width="320">](./assets/prtsc/M_VS_PANE_power-shell-mktest.png)  

## 動作確認  
### 　アプリ起動  
　<img src="./assets/env/M_win.png" height="14" align="top">
<img src="./assets/prtsc/M_VS_MENU_icon.png" align="top"> 
<img src="./assets/env/M_menu-L.png" height="12"> メニューバー 
<img src="./assets/env/M_menu-R.png" height="12"> の
<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_exrmwpf-run.png" hight="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  

　　[<img src="./assets/prtsc/M_VS_PANE_menu-exrmwpf.png" width="420">](./assets/prtsc/M_VS_PANE_menu-exrmwpf.png)

　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　[<img src="./assets/prtsc/M_VS_WIN_exrm-run.png" width="240" align="top">](./assets/prtsc/M_VS_WIN_exrm-run.png")
　<img src="./assets/env/M_allow-R.png" height="14" align="top">　[<img src="./assets/prtsc/M_VS_WIN_exrm-exe.png" height="240">](./assets/prtsc/M_VS_WIN_exrm-exe.png)  

### 　試行 ( <img src="./assets/env/M_folder.png" height="14"> test1st で実施 )
1. <img src="./assets/prtsc/M_EXRM_select.png" height="14"> <img src="./assets/env/M_click.png" height="14">、処理対象DIRを選択  
2. <img src="./assets/prtsc/M_EXRM_not-removed-words.png" height="14"> に**削除除外対象**に含まれる文字列を指定  
複数指定する場合は "**,**" で区切って下さい
3. <img src="./assets/prtsc/M_EXRM_scan.png" height="14"> を <img src="./assets/env/M_click.png" height="14"> 、<img src="./assets/env/M_win.png" height="14"> **Prossesing nessage** に表示される削除対象を確認  
4. <img src="./assets/prtsc/M_EXRM_recursive-processing.png" height="14"> <img src="./assets/env/M_check.png" height="14"> で、下位階層に対する処理の可否を選択 
5. <img src="./assets/prtsc/M_EXRM_delete.png" height="14"> <img src="./assets/env/M_click.png" height="14"> で実行
6. 必要に応じて <img src="./assets/prtsc/M_EXRM_undo.png" height="14"> <img src="./assets/env/M_click.png" height="14"> で元に戻せます。
<br>

## 単体アプリ作成  
### <img src="./assets/env/M_visualstudio-icon.png" height="14"> バージョン指定
　<img src="./assets/env/M_win.png" height="14" align="top">
<img src="./assets/env/M_menu-L.png" height="12"> ソリューションエクスプローラー <img src="./assets/env/M_menu-R.png" height="12">  
　　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_exrm-wpf.png" hight="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">
　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_editing-project-files.png" hight="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  
　　<img src="./assets/prtsc/M_VS_PANE_solution-explorer08.png" width="320">  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　[<img src="./assets/prtsc/M_VS_PANE_exrm-wpf-csproj-1st.png" width="320">](./assets/prtsc//M_VS_PANE_exrm-wpf-csproj-1st.png)  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　[<img src="./assets/prtsc/M_VS_PANE_exrm-wpf-csproj-2nd.png" width="320">](./assets/prtsc/M_VS_PANE_exrm-wpf-csproj-2nd.png)  
<details>  
<summary>
　<img src="./assets/env/M_copy.png" height="14">  
<img src="./assets/env/M_LANG_XML.png" height="14"> <img src="./assets/env/M_write.png" height="14"> : Version情報追記  
</summary>  
  
```  
    <!-- バージョン情報 -->
    <Version>2.0.0+2</Version>
    <AssemblyVersion>2.0.0.0</AssemblyVersion>
    <FileVersion>2.0.0.2</FileVersion>
    <InformationalVersion>2.0.0+2</InformationalVersion> 
```  
</details>  

### 　<img src="./assets/env/M_monitor.png" height="14"> icon 作成
　　<img src="./assets/env/M_file.png" height="14"> **exrm.ico** を作成  
　　解像度：256, 128, 96, 64, 48, 32, 16 [Pixel]の画像をを内包する".ico"ファイルを作成します。  
　　方法はお任せ。VisualStudioでも作成出来ます(方法は省略)。  
　　　GitHub [<img src="./assets/env/M_link.png" height="14"> exrm_wpf.ico](https://github.com/AHazeyama/public/blob/main/exrm_wpf/exrm_wpf.ico)  
　　　.ico作成ツール [<img src="./assets/env/M_link.png" height="14"> GreenFish Icon Editor Pro ](https://greenfishsoftware.org/)　　　<img src="./assets/env/M_comment-F.png" height="12"> <img src="./assets/prtsc/M_COM_reference.png" height="12"> 

### <img src="./assets/env/M_visualstudio-icon.png" height="14"> iconをプロジェクトへ追加
#### 　　<img src="./assets/env/M_file.png" height="14"> .icon追加
　<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> ソリューションエクスプローラー <img src="./assets/env/M_menu-R.png" height="12">   
　　　<img src="./assets/env/M_menu-L.png" height="12"> ペイン内の空白部分 <img src="./assets/env/M_menu-R.png" height="12"> 右 <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">　
<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_addition.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">　
<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_existing-items.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  
　　　[<img src="./assets/prtsc/M_VS_PANE_solution-explorer09.png" width="480">](./assets/prtsc/M_VS_PANE_solution-explorer09.png)  
　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　　<img src="./assets/env/M_file-exproler.png" align="top"> : <img src="./assets/env/M_menu-L.png" height="12" align="top"> **.ico** <img src="./assets/env/M_menu-R.png" height="12" align="top"> 選択  
　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　　[<img src="./assets/prtsc/M_VS_WIN_icon-editor.png" width="320">](./assets/prtsc/M_VS_WIN_icon-editor.png)  

> [!NOTE]
> &emsp;必要なら <img src="./assets/env/M_write.png" height="14">  


#### 　<img src="./assets/env/M_visualstudio-icon.png" height="14"> アプリにアイコンを設定
　　<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12"> ソリューションエクスプローラー <img src="./assets/env/M_menu-R.png" height="12">   
　　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_exrm-wpf.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> 右 <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">　
<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_property.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">　<img src="./assets/env/M_file.png" height="14"> **.ico** 選択  
　　　[<img src="./assets/prtsc/M_VS_PANE_solution-explorer10.png" width="180">](./assets/prtsc/M_VS_PANE_solution-explorer10.png)
　<img src="./assets/env/M_allow-R.png" height="14" align="top">　
[<img src="./assets/prtsc/M_VS_PANE_exrm-wpf-property.png" width="180" align="top">](./assets/prtsc/M_VS_PANE_exrm-wpf-property.png)　
<img src="./assets/env/M_allow-R.png" height="14" align="top">　
<img src="./assets/env/M_file-exproler.png" align="top">  
　　　<img src="./assets/env/M_menu-L.png" height="12" align="top"> <img src="./assets/prtsc/M_VS_DDOWN_resource.png" width="240"> <img src="./assets/env/M_menu-R.png" height="12">
<img src="./assets/env/M_click.png" height="14" align="top">  

#### 　<img src="./assets/env/M_visualstudio-icon.png" height="14"> アイコン設定  
　　<img src="./assets/env/M_win.png" height="14" align="top">
<img src="./assets/env/M_menu-L.png" height="12"> ソリューションエクスプローラー <img src="./assets/env/M_menu-R.png" height="12">  
　　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_exrm-wpf.png" hight="14"> <img src="./assets/env/M_menu-R.png" height="12"> 右<img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">
　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_editing-project-files.png" hight="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  
　　　<img src="./assets/prtsc/M_VS_PANE_solution-explorer08.png" width="320">  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　　[<img src="./assets/prtsc/M_VS_PANE_exrm-wpf-csproj-2nd.png" width="320">](./assets/prtsc/M_VS_PANE_exrm-wpf-csproj-2nd.png)  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　　[<img src="./assets/prtsc/M_VS_PANE_exrm-wpf-csproj-3rd.png" width="320">](./assets/prtsc/M_VS_PANE_exrm-wpf-csproj-3rd.png)  
<details>  
<summary>
　　<img src="./assets/env/M_copy.png" height="14">  
<img src="./assets/env/M_LANG_XML.png" height="14"> <img src="./assets/env/M_write.png" height="14"> : Version情報追記  
</summary>  
  
```  
    <!-- icon setting -->
    <ApplicationIcon>exrm.ico</ApplicationIcon>

  </PropertyGroup>      # このTAGは既存、これ以上とこれ以下のコマンドを追記

  <!-- icon setteing -->
  <ItemGroup>
    <None Remove="exrm.ico" />
  </ItemGroup>
```  
</details>  
<br>

### 　<img src="./assets/env/M_visualstudio-icon.png" height="14"> 単一exe化（Single File Publish）  
　　<img src="./assets/env/M_win.png" height="14" align="top">
<img src="./assets/env/M_menu-L.png" height="12"> ソリューションエクスプローラー <img src="./assets/env/M_menu-R.png" height="12">  
　　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_exrm-wpf.png" hight="14"> <img src="./assets/env/M_menu-R.png" height="12"> 右 <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">　
<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_issue.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  
　　 　[<img src="./assets/prtsc/M_VS_PANE_solution-explorer11.png" width="320">](./assets/prtsc/M_VS_PANE_exrm-wpf-csproj-2nd.png)  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_target.png" hight="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">　
<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_folder.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">　
<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_BTN_next2.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  
　　　[<img src="./assets/prtsc/M_VS_DLG_public01.png" width="320">](./assets/prtsc/M_VS_DLG_public01.png)  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_specific-target.png" hight="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">　
<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_folder.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">　
<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_BTN_next2.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  
　　　[<img src="./assets/prtsc/M_VS_DLG_public02.png" width="320">](./assets/prtsc/M_VS_DLG_public02.png)  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_place.png" hight="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">　
<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_reference.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14"> <img src="./assets/env/M_next.png" height="14">　
**出力** <img src="./assets/env/M_folder.png" height="14"> **選択** <img src="./assets/env/M_next.png" height="14">　
<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MENU_completion.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  
　　　[<img src="./assets/prtsc/M_VS_DLG_public03.png" width="320">](./assets/prtsc/M_VS_DLG_public03.png)　
<img src="./assets/env/M_allow-T.png" height="28" align="top">　
<img src="./assets/env/M_file-exproler.png" align="top">  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_BTN_issue.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  
　　　[<img src="./assets/prtsc/M_VS_PANE_exrm-wpf-issue1.png" width="320">](./assets/prtsc/M_VS_PANE_exrm-wpf-issue1.png)  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　　[<img src="./assets/prtsc/M_VS_PANE_exrm-wpf-issue2.png" width="320">](./assets/prtsc/M_VS_PANE_exrm-wpf-issue2.png)  
　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　　[<img src="./assets/prtsc/M_VS_PANE_exrm-wpf-issue3.png" width="320">](./assets/prtsc/M_VS_PANE_exrm-wpf-issue3.png)  

　　出力先 <img src="./assets/env/M_folder.png" height="14">  
　　　**exrm_wpf\bin\Release\net10.0-windows\win-x64\publish**  
　　　<img src="./assets/prtsc/M_COM_exe-output-folder.png" height="14">
> [!CAUTION]
> ⚠️ 🗁 win-x64 以下のexeは **.dll** が必要( **️単体ではない** )。  

### 　Visual Studio使わない方法  
　　プロジェクトフォルダ（.csproj がある場所）で  

　　<img src="./assets/env/M_term.png" height="14"> <img src="./assets/env/M_SHELL_PowerrShell.png" height="12">
<details>  
<summary>
<img src="./assets/env/M_copy.png" height="14"> <img src="./assets/env/M_write.png" height="14"> COMMAND  
</summary>  

```  
dotnet publish -c Release -r win-x64 --self-contained true ` 
-p:PublishSingleFile=true -p:IncludeNativeLibrariesForSelfExtract=true
```  
</details>  

　[<img src="./assets/prtsc/M_VS_PANE_pwsh-exe-issue.png" width="560">](./assets/prtsc/M_VS_PANE_pwsh-exe-issue.png)  

## Git 更新 (README.md、exrm.exe)  
　<img src="./assets/env/M_win.png" height="14" align="top">
<img src="./assets/prtsc/M_VS_MENU_icon.png" align="top"> 右下の 
<img src="./assets/env/M_menu-L.png" height="12" align="top"> 
<img src="./assets/prtsc/M_VS_MENU_change-source.png" height="14" align="top"> 
<img src="./assets/env/M_menu-R.png" height="12" align="top"> 
<img src="./assets/env/M_click.png" height="14" align="top">  
　　<img src="./assets/prtsc/M_VS_WIN_change-source.png" width="320">  
　　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　<img src="./assets/env/M_win.png" height="14"> <img src="./assets/env/M_menu-L.png" height="12" align="top"> <img src="./assets/prtsc/M_VS_BTN_git-all-add.png" height="14" align="top"> <img src="./assets/env/M_menu-R.png" height="12" align="top"> <img src="./assets/env/M_click.png" height="14" align="top">  
> [!TIP]
> <img src="./assets/env/M_file.png" height="14"> 個別にaddする場合は各<img src="./assets/env/M_file.png" height="14"> 右側の <img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_BTN_git-Individual-add.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  

　　<img src="./assets/prtsc/M_VS_PANE_git-status.png" width="320">  
　　　　　　　　<img src="./assets/env/M_allow-D.png" height="14">  
　　<img src="./assets/env/M_menu-L.png" height="12"> <img src="./assets/prtsc/M_VS_MSG_commit-message.png" height="14"> <img src="./assets/env/M_menu-R.png" height="12"> へコミットメッセージを入力 <img src="./assets/env/M_next.png" height="14"> <img src="./assets/env/M_button-L.png" height="12"> <img src="./assets/prtsc/M_VS_BTN_git-all-commit.png" height="14"> <img src="./assets/env/M_button-R.png" height="12"> <img src="./assets/env/M_click.png" height="14">  

> [!TIP]
> <img src="./assets/prtsc/M_VS_BTN_copilot.png" height="18"> <img src="./assets/env/M_click.png" height="14"> : CopilotによるCommitメッセージ自動生成可能

　　<img src="./assets/prtsc/M_VS_PANE_git-commit.png" width="320">  

### 以上で開発は終了です。
### 　検証項目 (Example: normal system 、 <img src="./assets/env/M_folder.png" height="14"> test1st で実施 )
1. <img src="./assets/prtsc/M_EXRM_select.png" height="14"> <img src="./assets/env/M_click.png" height="14">、処理対象DIRを選択  
2. <img src="./assets/prtsc/M_EXRM_not-removed-words.png" height="14"> に**削除除外対象**に含まれる文字列を指定  
複数指定する場合は "**,**" で区切って下さい
3. <img src="./assets/prtsc/M_EXRM_scan.png" height="14"> を <img src="./assets/env/M_click.png" height="14"> 、<img src="./assets/env/M_win.png" height="14"> **Prossesing nessage** に表示される削除対象を確認  
4. <img src="./assets/prtsc/M_EXRM_recursive-processing.png" height="14"> <img src="./assets/env/M_check.png" height="14"> で、下位階層に対する処理の可否を選択 
5. <img src="./assets/prtsc/M_EXRM_delete.png" height="14"> <img src="./assets/env/M_click.png" height="14"> で実行
6. 必要に応じて <img src="./assets/prtsc/M_EXRM_undo.png" height="14"> <img src="./assets/env/M_click.png" height="14"> で元に戻せます。

　　<img src="./assets/env/M_caution.png" height="14"> 検証のバリエーションに関しては別途記載予定
<!-- 後日、SoftwareDevelopmentGuide整備後に記載  
#### 項目設定方法  
　[🔗SoftwareDevelopmentGuideへのリンク]  
-->  
