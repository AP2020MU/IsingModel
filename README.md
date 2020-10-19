# IsingModelSimulation
2次元Ising模型のMarkov連鎖MonteCarloシミュレーションを，Python3を用いて行うことを目的とする．
概要はIsingSimulation.pdfに記載した通りである．

###IsingModel.pyを実行する際の注意点###

・ソースコードをそのまま実行すると，おそらくIMPORTERRORが発生する．これは"japanize_matplotlib"がインストールされていないことによると思われる．

-->もし，実行環境において既にmatplotlibのグラフの中に日本語フォントを表示することができるなら，"import japanize_matplotlib"をコメントアウトするだけで実行可能になるはずである．

-->それ以外の場合，

    1. "$ pip install japanize_matplotlib"を実行して環境に"japanize_matplotlib"をインストールする
    
    2. 他の方法でmatplotlibのグラフの中に日本語フォントを表示できるようにする
    
    3. IsingModel.pyのクラスメソッドのうち"visualize_*()"の中のtitleやlabelから日本語を消し，アルファベットのみにする
    
のいずれかを行う必要がある．
    
   
