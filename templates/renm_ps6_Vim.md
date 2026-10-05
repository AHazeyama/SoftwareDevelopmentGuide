<p akugb=:keft>  
	<img src="./assets/Title_renm_dark.png#gh-dark-mode-only" alt="banner dark">  
	<img src="./assets/Title_renm_light.png#gh-light-mode-only" alt="banner light">  
</p>  

# OverView
目的 : PySide6を使用したアプリケーション開発  
内容 : ファイル/ディレクトリ名一括変換ツール[renm_ps6]  
|Item|Content|
|:--|:--|
|OS|<img src="./assets/env/M_OS_Win11.png" height="13">　**/**　<img src="./assets/env/M_OS_Ubuntu.png" height="13">|  
|Shell|<img src="./assets/env/M_SHELL_PowerrShell.png" height="14">  
|Language|<img src="./assets/env/M_LANG_Python.png" height="20">|  
|Framework|<img src="./assets/env/M_FW_PySide6.png" height="32">|  
|Editor|<img src="./assets/env/M_EDT_Vim-icon.png" height="24">　**/**　<img src="./assets/env/M_EDT_VSCode-banner.png" height="24">


> [!caution]
> Trademarks: Company names, product names, and logos used in documents related to this project are trademarks or registered trademarks of their respective owners. They are cited solely for the purpose of describing the technologies used.

> [!NOTE]  
> 凡例  
> [<img src="./assets/env/M_legend.png" width="540">](./assets/env/M_legend.png)  
>
> 縮小画像 (マウスカーソルが <img src="./assets/env/M_info.png" height="14"> に変化する画像) は <img src="./assets/env/M_click.png" height="14"> で拡大表示します。  
>
> Source code / コマンド は <img src="./assets/env/M_copy.png" height="14"> <img src="./assets/env/M_click.png" height="14"> でText表示します (表示されたTextの右上にある <img src="./assets/env/M_git-copy.png" height="14"> <img src="./assets/env/M_click.png" height="14"> でコピー)。  
>
> <img src="./assets/env/M_infoG.png" height="14"> ブラウザを **Darkモード** にして頂けると、見やすくなります。  

# ファイル/フォルダーの一括リネームツール [renm]作成手順

## Python 開発環境共通設定  
　　Pythonを使用した開発に関する共通設定を記載しています。  
　　[<img src="./assets/env/M_link.png" height="14"> **Common settings for the development environment**](https://github.com/AHazeyama/Tkinter_tools/blob/main/CommonSettings.md)

## 開発
### renm_ps6.py コーディング
　[<img src="./assets/env/M_LANG_Python.png" height="18"><br>　　<img src="./assets/env/M_link.png" height="14"> Source code [renm_ps6.py]](https://github.com/AHazeyama/public/blob/main/renm_ps6/renm_ps6.py)  
#### 動作確認
　<img src="./assets/env/M_SHELL_PowerrShell.png" height="12">　/　<img src="./assets/env/M_SHELL_BASH.png" height="12">
<details>  
<summary>  
　<img src="./assets/env/M_copy.png" height="14">  
　<img src="./assets/cmd/M_CMD_pyhton3-renm_ps6.png">  

</summary>   

```PWSH
Python3 renm_ps6.py  
```

</details>  

　　[<img src="./assets/renm_ps6.png" height="256">](./assets/renm_ps6.png)  



### バージョン指定
　renm_ps6.versionを編集  
　GitHub [renm_ps6.version](https://github.com/AHazeyama/renm_ps6/blob/main/renm_ps6.version)

### icon 作成
　renm_ps6.icoを作成  
　解像度：256x256, 128x128, 96x96, 64x64, 48x48, 32x32, 16x16 [pixel] を内包する事  
　　(128,64Pixelは他のサイズで代用可能なため、`.exe`容量を削減する場合は省略可)。  
　GitHub [renm_ps6.ico](https://github.com/AHazeyama/renm_ps6/blob/main/renm_ps6.ico)　
　<img src="./assets/prtsc/renm_ps6.ico" height="64" align="top">

　使用ツール　:　<img src="./assets/env/M_link.png" height="14" align="top"> [<img src="./assets/env/M_TOOL_greenfish.png" height="20" align="top">](https://greenfishsoftware.org/)　　　<img src="./assets/env/M_COM_refernce.png">  

## テスト環境構築  
　<img src="./assets/env/M_SHELL_PowerrShell.png" height="12">  
　<img src="./assets/env/M_file.png" height="14">
 [mktest.ps1](https://github.com/AHazeyama/renm_ps6/blob/main/mktest.ps1)  

### 試行  
1. ｢**Select**｣ をクリックし、**Exec directory** を選択
2. **not removed words** に**削除除外対象**に含まれる文字列を指定  
3. ｢**Scan**｣ をクリックし、**Prossesing nessage** に表示される削除対象を確認  
複数指定する場合は "**,**" で区切って下さい
4. **☑ Recursive processing** で、下位階層に対する処理の可否を選択 
5. ｢**Delete**｣ をクリックして実行
6. 必要に応じて ｢**Undo**｣ で元に戻す
<br>

## 単体アプリ作成  
　<img src="./assets/env/M_SHELL_PowerrShell.png" height="12">  
<details>  
<summary>  
　<img src="./assets/env/M_copy.png" height="14">  
　<img src="./assets/cmd/M_CMD_pyinstaller-pysice6-renm.png">  

</summary>   

```PWSH
pyinstaller `
  --noconsole --onefile `
  --icon=renm_ps6.ico `
  --add-data "renm_ps6.ico;." `
  --version-file=renm_ps6.version `
  --collect-all PySide6 `
  renm_ps6.py
```

</details>  

　[<img src="./assets/prtsc/M_MSG_pyinstaller-pyside6-renm.png" width="540">](./assets/prtsc/M_MSG_pyinstaller-pyside6-renm.png)  

　出力先  
　　<img src="./assets/env/M_folder.png" height="14"> :　.\ dist \
