# renm_PySide6_Vim
## OverView
目的 : PySide6を使用したアプリケーション開発  
内容 : ファイル/ディレクトリ名一括変換ツール[renm_ps6]  
|Item|Content|
|:--|:--|
|OS|![](./assets/logo_Windows11.png) / ![](./assets/logo_Ubuntu.png)|
|言語|![](./assets/logo_Python.png)|
|Framework|![](./assets/logo_PySide6.png)|
|Editor|![](./assets/logo_Vim.png)|

※ 記号例
```
⬇️:マウスクリック、"･･･":テキスト、a/b:選択(a or b)、｢･･･｣:ウィンドウ/メニュー/フォーム、
[･･･]:ボタン、<･･･>:Key、⇒:次動作、#･･･:コメント  
```
<br>

# ファイル/フォルダーの排他的削除ツール [exrm]作成手順
## 開発環境構築
### 仮想環境生成
　　![](assets/shell_P.png) Commands
```PowerShell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass <⏎>  # コマンド抑止バイパス
py -m venv renm_env <⏎>  # 仮想環境構築
.\renm_env\Scripts\Activate.ps1 <⏎>  # 仮想環境起動
py -m pip install -U pip <⏎>  # Pkg管理Toolアップデート
py -m pip install PySide6 pyinstaller pyinstaller-versionfile <⏎>  # Toolインストール
pip list <⏎>  # 適用ツール確認
# Development process
deactivate <⏎>  # 仮想環境停止 (開発終了時に実行)
```
　　![](assets/shell_B.png) Commands
```bash
py -m venv renm_env <⏎>  # 仮想環境構築
source ./renm_env/bin/activate <⏎>  # 仮想環境起動
py -m pip install -u pip <⏎>  # Pkg管理Toolアップデート
py -m pip install PySide6 pyinstaller pyinstaller-versionfile <⏎>  # Toolインストール
pip list <⏎>  # 適用ツール確認
# Development process
deactivate <⏎>  # 仮想環境停止 (開発終了時に実行)
```
> [!NOTE]  
> 実行状況は末尾 [Apendix] に記載

## 開発
### renm_ps6.py コーディング
　![](./assets/logo_Python.png) Source code  
　GitHub [renm_ps6.py](https://github.com/AHazeyama/public/blob/main/renm_ps6/renm_ps6.py)
## 動作確認
　![](./assets/shell_BP.png)
```Powershell
Python3 renm_ps6.py <⏎>
```
### バージョン指定
　renm_ps6.versionを編集  
　GitHub [renm_ps6.version](https://github.com/AHazeyama/public/blob/main/renm_ps6/renm_ps6.version)
### icon 作成
　renm_ps6.icoを作成
　解像度：16x16, 32x32, 64x64, 128x128, 256x256 [pixel] を内包する事  
　GitHub [renm_ps6.ico](https://github.com/AHazeyama/public/blob/main/renm_ps6/renm_ps6.ico)  
　使用ツール [GreenFish Icon Editor Pro ](https://greenfishsoftware.org/)  

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

# Apendix
### Command Line & Messages
![](./assets/shell_P.png)  
```Powershell
PS C:\bin\renm_ps6> Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
PS C:\bin\renm_ps6> py -m venv renm_env
PS C:\bin\renm_ps6> .\renm_env\Scripts\Activate.ps1
(renm_env) PS C:\bin\renm_ps6> py -m pip install -U pip
Requirement already satisfied: pip in c:\bin\renm_ps6\renm_env\lib\site-packages (25.3)
Collecting pip
  Using cached pip-26.1.2-py3-none-any.whl.metadata (4.6 kB)
Using cached pip-26.1.2-py3-none-any.whl (1.8 MB)
Installing collected packages: pip
  Attempting uninstall: pip
    Found existing installation: pip 25.3
    Uninstalling pip-25.3:
      Successfully uninstalled pip-25.3
Successfully installed pip-26.1.2
(renm_env) PS C:\bin\renm_ps6> py -m pip install Pyside6 pyinstaller pyinstaller-versionfile
Collecting Pyside6
  Using cached pyside6-6.11.1-cp310-abi3-win_amd64.whl.metadata (5.5 kB)
Collecting pyinstaller
  Using cached pyinstaller-6.21.0-py3-none-win_amd64.whl.metadata (8.5 kB)
Collecting pyinstaller-versionfile
  Using cached pyinstaller_versionfile-3.1.0-py3-none-any.whl.metadata (11 kB)
Collecting shiboken6==6.11.1 (from Pyside6)
  Using cached shiboken6-6.11.1-cp310-abi3-win_amd64.whl.metadata (2.5 kB)
Collecting PySide6_Essentials==6.11.1 (from Pyside6)
  Using cached pyside6_essentials-6.11.1-cp310-abi3-win_amd64.whl.metadata (3.8 kB)
Collecting PySide6_Addons==6.11.1 (from Pyside6)
  Using cached pyside6_addons-6.11.1-cp310-abi3-win_amd64.whl.metadata (4.2 kB)
Collecting altgraph (from pyinstaller)
  Using cached altgraph-0.17.5-py2.py3-none-any.whl.metadata (7.5 kB)
Collecting packaging>=22.0 (from pyinstaller)
  Using cached packaging-26.2-py3-none-any.whl.metadata (3.5 kB)
Collecting pefile>=2022.5.30 (from pyinstaller)
  Using cached pefile-2024.8.26-py3-none-any.whl.metadata (1.4 kB)
Collecting pyinstaller-hooks-contrib>=2026.6 (from pyinstaller)
  Using cached pyinstaller_hooks_contrib-2026.6-py3-none-any.whl.metadata (16 kB)
Collecting pywin32-ctypes>=0.2.1 (from pyinstaller)
  Using cached pywin32_ctypes-0.2.3-py3-none-any.whl.metadata (3.9 kB)
Collecting setuptools>=42.0.0 (from pyinstaller)
  Using cached setuptools-83.0.0-py3-none-any.whl.metadata (6.6 kB)
Collecting Jinja2 (from pyinstaller-versionfile)
  Using cached jinja2-3.1.6-py3-none-any.whl.metadata (2.9 kB)
Collecting PyYAML (from pyinstaller-versionfile)
  Using cached pyyaml-6.0.3-cp314-cp314-win_amd64.whl.metadata (2.4 kB)
Collecting MarkupSafe>=2.0 (from Jinja2->pyinstaller-versionfile)
  Using cached markupsafe-3.0.3-cp314-cp314-win_amd64.whl.metadata (2.8 kB)
Using cached pyside6-6.11.1-cp310-abi3-win_amd64.whl (578 kB)
Using cached pyside6_addons-6.11.1-cp310-abi3-win_amd64.whl (168.8 MB)
Using cached pyside6_essentials-6.11.1-cp310-abi3-win_amd64.whl (77.5 MB)
Using cached shiboken6-6.11.1-cp310-abi3-win_amd64.whl (1.2 MB)
Using cached pyinstaller-6.21.0-py3-none-win_amd64.whl (1.4 MB)
Using cached pyinstaller_versionfile-3.1.0-py3-none-any.whl (13 kB)
Using cached packaging-26.2-py3-none-any.whl (100 kB)
Using cached pefile-2024.8.26-py3-none-any.whl (74 kB)
Using cached pyinstaller_hooks_contrib-2026.6-py3-none-any.whl (457 kB)
Using cached pywin32_ctypes-0.2.3-py3-none-any.whl (30 kB)
Using cached setuptools-83.0.0-py3-none-any.whl (1.0 MB)
Using cached altgraph-0.17.5-py2.py3-none-any.whl (21 kB)
Using cached jinja2-3.1.6-py3-none-any.whl (134 kB)
Using cached markupsafe-3.0.3-cp314-cp314-win_amd64.whl (15 kB)
Using cached pyyaml-6.0.3-cp314-cp314-win_amd64.whl (156 kB)
Installing collected packages: altgraph, shiboken6, setuptools, PyYAML, pywin32-ctypes, pefile, packaging, MarkupSafe, PySide6_Essentials, pyinstaller-hooks-contrib, Jinja2, PySide6_Addons, pyinstaller-versionfile, pyinstaller, Pyside6
Successfully installed Jinja2-3.1.6 MarkupSafe-3.0.3 PySide6_Addons-6.11.1 PySide6_Essentials-6.11.1 PyYAML-6.0.3 Pyside6-6.11.1 altgraph-0.17.5 packaging-26.2 pefile-2024.8.26 pyinstaller-6.21.0 pyinstaller-hooks-contrib-2026.6 pyinstaller-versionfile-3.1.0 pywin32-ctypes-0.2.3 setuptools-83.0.0 shiboken6-6.11.1
(renm_env) PS C:\bin\renm_ps6> pip list
Package                   Version
------------------------- ---------
altgraph                  0.17.5
Jinja2                    3.1.6
MarkupSafe                3.0.3
packaging                 26.2
pefile                    2024.8.26
pip                       26.1.2
pyinstaller               6.21.0
pyinstaller-hooks-contrib 2026.6
pyinstaller_versionfile   3.1.0
PySide6                   6.11.1
PySide6_Addons            6.11.1
PySide6_Essentials        6.11.1
pywin32-ctypes            0.2.3
PyYAML                    6.0.3
setuptools                83.0.0
shiboken6                 6.11.1
(renm_env) PS C:\bin\renm_ps6>
```
![](./assets/shell_B.png)  
```bash
Guest@Ubuntu:~/bin/renm_ps6$ py -m venv renm_env
Guest@Ubuntu:~/bin/renm_ps6$ source ./renm_env/bin/activate
(renm_env) Guest@Ubuntu:~/bin/renm_ps6$ py -m pip install -U pip
Requirement already satisfied: pip in ./renm_env/lib/python3.12/site-packages (24.0)
Collecting pip
  Using cached pip-26.1.2-py3-none-any.whl.metadata (4.6 kB)
Using cached pip-26.1.2-py3-none-any.whl (1.8 MB)
Installing collected packages: pip
  Attempting uninstall: pip
    Found existing installation: pip 24.0
    Uninstalling pip-24.0:
      Successfully uninstalled pip-24.0
Successfully installed pip-26.1.2
(renm_env) Guest@Ubuntu:~/bin/renm_ps6$ py -m pip install PySide6 pyinstaller pyinstaller-versionfile
Collecting PySide6
  Using cached pyside6-6.11.1-cp310-abi3-manylinux_2_34_x86_64.whl.metadata (5.3 kB)
Collecting pyinstaller
  Using cached pyinstaller-6.21.0-py3-none-manylinux2014_x86_64.whl.metadata (8.5 kB)
Collecting pyinstaller-versionfile
  Using cached pyinstaller_versionfile-3.1.0-py3-none-any.whl.metadata (11 kB)
Collecting shiboken6==6.11.1 (from PySide6)
  Using cached shiboken6-6.11.1-cp310-abi3-manylinux_2_34_x86_64.whl.metadata (2.4 kB)
Collecting PySide6_Essentials==6.11.1 (from PySide6)
  Using cached pyside6_essentials-6.11.1-cp310-abi3-manylinux_2_34_x86_64.whl.metadata (3.6 kB)
Collecting PySide6_Addons==6.11.1 (from PySide6)
  Using cached pyside6_addons-6.11.1-cp310-abi3-manylinux_2_34_x86_64.whl.metadata (4.0 kB)
Collecting altgraph (from pyinstaller)
  Using cached altgraph-0.17.5-py2.py3-none-any.whl.metadata (7.5 kB)
Collecting packaging>=22.0 (from pyinstaller)
  Using cached packaging-26.2-py3-none-any.whl.metadata (3.5 kB)
Collecting pyinstaller-hooks-contrib>=2026.6 (from pyinstaller)
  Using cached pyinstaller_hooks_contrib-2026.6-py3-none-any.whl.metadata (16 kB)
Collecting setuptools>=42.0.0 (from pyinstaller)
  Using cached setuptools-83.0.0-py3-none-any.whl.metadata (6.6 kB)
Collecting Jinja2 (from pyinstaller-versionfile)
  Using cached jinja2-3.1.6-py3-none-any.whl.metadata (2.9 kB)
Collecting PyYAML (from pyinstaller-versionfile)
  Using cached pyyaml-6.0.3-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl.metadata (2.4 kB)
Collecting MarkupSafe>=2.0 (from Jinja2->pyinstaller-versionfile)
  Using cached markupsafe-3.0.3-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl.metadata (2.7 kB)
Using cached pyside6-6.11.1-cp310-abi3-manylinux_2_34_x86_64.whl (572 kB)
Using cached pyside6_addons-6.11.1-cp310-abi3-manylinux_2_34_x86_64.whl (175.1 MB)
Using cached pyside6_essentials-6.11.1-cp310-abi3-manylinux_2_34_x86_64.whl (79.9 MB)
Using cached shiboken6-6.11.1-cp310-abi3-manylinux_2_34_x86_64.whl (272 kB)
Using cached pyinstaller-6.21.0-py3-none-manylinux2014_x86_64.whl (754 kB)
Using cached pyinstaller_versionfile-3.1.0-py3-none-any.whl (13 kB)
Using cached packaging-26.2-py3-none-any.whl (100 kB)
Using cached pyinstaller_hooks_contrib-2026.6-py3-none-any.whl (457 kB)
Using cached setuptools-83.0.0-py3-none-any.whl (1.0 MB)
Using cached altgraph-0.17.5-py2.py3-none-any.whl (21 kB)
Using cached jinja2-3.1.6-py3-none-any.whl (134 kB)
Using cached markupsafe-3.0.3-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl (22 kB)
Using cached pyyaml-6.0.3-cp312-cp312-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl (807 kB)
Installing collected packages: altgraph, shiboken6, setuptools, PyYAML, packaging, MarkupSafe, PySide6_Essentials, pyinstaller-hooks-contrib, Jinja2, PySide6_Addons, pyinstaller-versionfile, pyinstaller, PySide6
Successfully installed Jinja2-3.1.6 MarkupSafe-3.0.3 PySide6-6.11.1 PySide6_Addons-6.11.1 PySide6_Essentials-6.11.1 PyYAML-6.0.3 altgraph-0.17.5 packaging-26.2 pyinstaller-6.21.0 pyinstaller-hooks-contrib-2026.6 pyinstaller-versionfile-3.1.0 setuptools-83.0.0 shiboken6-6.11.1
(renm_env) Guest@Ubuntu:~/bin/renm_ps6$ pip list
Package                   Version
------------------------- -------
altgraph                  0.17.5
Jinja2                    3.1.6
MarkupSafe                3.0.3
packaging                 26.2
pip                       26.1.2
pyinstaller               6.21.0
pyinstaller-hooks-contrib 2026.6
pyinstaller_versionfile   3.1.0
PySide6                   6.11.1
PySide6_Addons            6.11.1
PySide6_Essentials        6.11.1
PyYAML                    6.0.3
setuptools                83.0.0
shiboken6                 6.11.1
(renm_env) Guest@Ubuntu:~/bin/renm_ps6$
```
