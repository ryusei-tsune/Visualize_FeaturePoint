# Visualize_FeaturePoint

## 概要
このリポジトリは，別のプログラムによって検出した特徴点を可視化するものです．具体的には，検出した特徴点座標が `x,y,z` の形式で保存されたテキストファイル(`Assets/Data/points.txt`)を `Assets/Scrits/DataVisualizer.cs` に与えることで，Unity のScene上に特徴点が表示されます．

### 使用方法
1. まず Unity で `Visualize-FP-Scene` を開き，Hierarchy の `+` から `XR/AR Default Point Cloud` を作成します．
2. 作成したオブジェクトのコンポーネントの `AR Point Cloud` と `AR Point Cloud Particle Visualizer` のチェックを外します．
3. 作成したオブジェクトに `Assets/Scrits/DataVisualizer.cs` を追加します．
4. スクリプトの Data の箇所に表示したい特徴点データのファイルを追加します．
5. 最後に実行し，特徴点が可視化されます．

### 補足
特徴点データの座標によっては `main camera` の座標，角度を調整する必要があります．もし何も表示されない場合は調整してみてください．