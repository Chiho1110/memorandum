# Anaconda Prompt上で、仮想環境を作る

## 共通部分
1. Anaconda Promptを開く。
2. `conda info -e` などで、現状の仮想環境を確認しておく。
3. `conda create -n 環境名 python=バージョン`で仮想環境を作成する。pythonのバージョンは指定しなくてもよい。
4. `conda activate 環境名`で仮想環境を起動できる。
5. 閉じる際には、`deactivate`で可能。
6. 削除する際には、`conda remove -n 環境名 --all`で実行。

## Jupyterで仮想環境を利用する。
1. `conda install conda-forge::ipykernel`でipykernelをインストール。どうしてもうまくいかなければ、pip installで。
2. `ipython kernel install --user --name=仮想環境名`を実行。
3. Jupyter Notebook上で、新規ファイル作成時などに選択できることを確認。
4. 削除する際は、`jupyter kernelspec uninstall 仮想環境名`を実行。
