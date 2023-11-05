# 時系列データ分析(TSA：Time Series Analysis)
## 0. はじめに
　静岡大学 情報学部 情報科学科 峰野研究室では, 毎年後期で峰野研究室に配属が決まった学部3年生を対象に, 情報科学演習と称して時系列データの分析方法について学ぶ時間を設けている.   
　そのための環境設定用ファイル(setup.txt)と学習用フォルダ(study)を用意した. 
 学習用フォルダ(study)内は, 以下のような構成になっている.  
- データ前処理用ファイル(data.ipynb)
- 学習モデル作成用ファイル(model.ipynb)
- dataフォルダ > 加工前のデータ(trainval_data.xlsx)
- imageフォルダ > ipynb埋め込み用画像(image1,2,3,4.jpg)
## 1. 環境構築について
　環境構築用ファイル(setup.txt)に記載されている内容を以下に示す.  
### 1.1 実行環境
- Windows11上のAnaconda  
- プロセッサ：AMD Ryzen 7 5825U  
- メモリ：16GB  
### 1.2 環境構築
- Anaconda公式サイト(URL：https://www.anaconda.com/products/distribution)から適用OS版の「Anaconda Distribution」をダウンロードする  
- ウィザードに従って, Anacondaをインストール  
- スタート画面から「Anaconda Prompt(Anaconda3)」を起動    
- 仮想環境の構築  
a. 使用する仮想環境を作成する  
```$ conda create -n "任意の環境名" python=3.9```  
b. 作成した仮想環境をアクティベートする  
```$ conda activate "任意の環境名"```   
c. 基本的なライブラリをインストール  
```$ conda install ipykernel ipywidgets pandas openpyxl numpy matplotlib seaborn scikit-learn tqdm```  
- tensorflowをインストールする  
```$ pip install tensorflow==2.12```  
```$ pip install --force-reinstall charset-normalizer==3.1.0 --user```  
- VSCodeで「predict」フォルダを開き, studyフォルダ内の, data.ipynbとmodel.ipynbを順に実行し, エラーが出ずに実行が完了すれば, 環境構築は完了   
## 2. データ前処理
## 3. モデル構築
