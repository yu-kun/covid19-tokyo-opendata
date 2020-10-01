# covid19-tokyo-opendata

## 概要 / Overview

東京都オープンデータカタログサイトの[東京都 新型コロナウイルス陽性患者発表詳細](https://catalog.data.metro.tokyo.lg.jp/dataset/t000010d0000000068)のcsvファイルを元にPython jupyterを用いて陽性患者数を年代別の積み上げグラフを出力するコード。

Source code to a distribution of patients by age group created with Python Jupyter on the basis of Tokyo Open Data Catalogue Site csv file.

## 実行に必要なソフトウェア環境 / Required software environment

当方の実行環境は以下のとおりです。Docker、VS code環境があれば他環境でも動く見込み。

My software enviroment is as follows. The same operation can be executed with Docker, VS code environment.


- macOS Catalina 10.15.5
- Docker version 19.03.8
- Visual Studio Code 1.46.0 (Extension: Remote Development, Docker, Python)

## Python Jupyter起動方法 / Python Jupyter start up guidelines 

~~~
git clone https://github.com/yu-kun/covid19-tokyo-opendata.git
~~~

VS Codeから上記で作成されたcovid19-tokyo-opendataフォルダを開きF1でプロンプトを起動の上、下記コマンドを実行する。

Open covid19-tokyo-opendata folder in VS Code, press F1, input the command below, Enter.

~~~
>Remote-Containers: Open Folder in Container
~~~

初回はDocker imageのビルドと拡張機能の導入、コンテナの起動で数分かかる。コンテナ環境起動後にpatient.pyファイルを開き、"# %%"行の上部にあるRun Cellボタンをクリック(Shift+Enter)するとJupyter Serverが起動しコードが実行される。

A few minutes will take to run the container for Docker image building and installing extentions. Open patient.py file after launching the container. By pressing Run Cell abowe "# %%" line you will launch Jupyter Server to run a code.


## 実行例 / Example

![日別陽性患者数](https://github.com/yu-kun/covid19-tokyo-opendata/blob/master/data/daily_patient_number_20201001.png)
![年代別陽性患者数](https://github.com/yu-kun/covid19-tokyo-opendata/blob/master/data/distribution_of_patients_by_age_group_20201001.png)

## 参考サイト / Reference

- [新型コロナウイルス感染症対策サイト](https://stopcovid19.metro.tokyo.lg.jp/) / [Tokyo COVID-19 Information](https://stopcovid19.metro.tokyo.lg.jp/en)
