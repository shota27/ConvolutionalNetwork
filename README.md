# プロジェクト名

## 自作部分
- **CNNモデルの拡張**: 元々の1層CNNモデルを3層のCNNと6層のバッチ正規化のモデルに拡張しました。

## 配布部分
- **CNN1層のモデル**　
- **手書き文字データ** 各文字200枚ずつ計3000枚が配布されました
- **モジュール**　　基本的な活性化関数が含まれています  

## アーキテクチャ
以下のようにモデルのアーキテクチャを設計しました：
Conv(32) -> BatchNorm -> ReLU -> MaxPooling
-> Conv(32,64) -> BatchNorm -> ReLU -> MaxPooling
-> Conv(32,64) -> BatchNorm -> ReLU -> MaxPooling
-> Affine(64,100) -> BatchNorm -> ReLU
-> Affine(100,100) -> BatchNorm -> ReLU
-> Affine(100,100) -> BatchNorm -> ReLU
-> Affine(100,15)




