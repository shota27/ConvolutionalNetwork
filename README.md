##自作部分
・1層のCNNモデルをCNN3層、バッチ正規化6層に拡張

##アーキテクチャ
Conv(32)->BatchNorm->ReLU->MaxPooling->
Conv(32,64)->BatchNorm->ReLU->MaxPooling->
Conv(32,64)->BatchNorm->ReLU->MaxPooling->
Affine(64,100)->BatchNorm->ReLU->
Affine(100,100)->BatchNorm->ReLU->
Affine(100,100)->BatchNorm->ReLU->
Affine(100,15)

##配布部分
・一層のCNN
・layers.py
