〇実行環境
・ Windows11上のAnaconda
・ プロセッサ：AMD Ryzen 7 5825U
・ メモリ：16GB

〇環境構築

Windows環境, Linux環境, Mac環境などに関わらず, Anacondaを利用することを推奨する
※Anaconda ・・・ Pythonの実行環境であり, データサイエンスに必要とされる各種ツールやライブラリを提供するプラットフォーム

1. Anaconda公式サイト(URL：https://www.anaconda.com/products/distribution)から適用OS版の「Anaconda Distribution」をダウンロードする

2. ウィザードに従って, Anacondaをインストール

3. スタート画面から「Anaconda Prompt(Anaconda3)」を起動
　※起動すると, コマンドの左端に(base)と表示されるはず

4. 仮想環境の構築
4-1. 使用する仮想環境を作成する
「$ conda create -n "任意の環境名" python=3.9」

4-2. 作成した仮想環境をアクティベートする
「$ conda activate "任意の環境名"」
※実行後, コマンドの左端が(base)から(任意の環境名)になるはず

4-3. 基本的なライブラリをインストール
「$ conda install ipykernel ipywidgets pandas openpyxl numpy matplotlib seaborn scikit-learn tqdm」

※ conda install で下記のopenssl関係等のエラーが出た場合
エラー内容:CondaSSLError: OpenSSL appears to be unavailable on this machine. OpenSSL is required to download and install packages.
→ https://slproweb.com/products/Win32OpenSSL.htmlのページの「Win64 OpenSSL v1.1.1v」をダウンロードして再度実行し直すと解決することがある
　 ・ダウンロードEXEファイルURL:https://slproweb.com/download/Win64OpenSSL-1_1_1v.exe

5. tensorflowをインストールする
「$ pip install tensorflow==2.12」
「$ pip install --force-reinstall charset-normalizer==3.1.0 --user」

6. VSCodeで「predict」フォルダを開き, studyフォルダ内の, data.ipynbとmodel.ipynbを順に実行し, エラーが出ずに実行が完了すれば, 環境構築は完了

※ 各自作業を進めていくうえで, 必要なライブラリがあれば, 追加や削除, バージョンのダウングレードを行うこと

-------------------
作成日：2023/09/16
作成者：原田 海斗
-------------------