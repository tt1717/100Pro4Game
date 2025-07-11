# このリポジトリはサンプルコードのみです (後日更新予定)

# Unity ML-Agents サンプルプロジェクト

このリポジトリは「Unityではじめる機械学習・強化学習 Unity ML-Agents 実践ゲームプログラミング v2.2対応版」のサンプルコードを含んでいます。

## 動作環境

### 必須環境
- Unity Hub
- Unity Editor（ML-Agents 2.2に対応したバージョン）
- Python 3.7以上
- Git

### 推奨環境
- OS: Windows 10/11, macOS 10.15以上
- RAM: 8GB以上
- GPU: NVIDIA GPU（CUDA対応）

## セットアップ手順

1. **Unity環境のセットアップ**
   ```bash
   # Unity Hubのインストール
   # https://unity.com/download からダウンロード
   ```

2. **ML-Agentsのインストール**
   ```bash
   # Unity Package ManagerからML-Agents 2.2をインストール
   # Window > Package Manager > + > Add package from git URL
   # com.unity.ml-agents を入力
   ```

3. **Python環境のセットアップ**
   ```bash
   # ML-Agents Pythonパッケージのインストール
   pip install mlagents==0.28.0
   ```

4. **プロジェクトのインポート**
   - Unity Hubで新規プロジェクトを作成
   - 各章の.unitypackageファイルをインポート
   - Assets > Import Package > Custom Package から選択

## プロジェクト構成

- `2/`: 第2章のサンプル
  - `2_1/`: RollerBallサンプル
  - `2_5/`: その他のサンプル
- `4/`: 第4章のサンプル
- `6/`: 第6章のサンプル
- `7/`: 第7章のサンプル

## 実行方法

1. **学習の実行**
   ```bash
   # プロジェクトのルートディレクトリで実行
   mlagents-learn config/rollerball_config.yaml --run-id=rollerball
   ```

2. **推論の実行**
   - Unity Editorで該当シーンを開く
   - Play ボタンを押して実行

## トラブルシューティング

### よくある問題

1. **ML-Agentsのバージョン不一致**
   - Unity側とPython側のML-Agentsバージョンが一致していることを確認
   - 必要に応じて`pip install mlagents==0.28.0`を実行

2. **Python環境の問題**
   - 仮想環境の使用を推奨
   - 必要なパッケージがすべてインストールされていることを確認

3. **GPUの利用**
   - NVIDIA GPUを使用する場合は、CUDAとcuDNNが正しくインストールされていることを確認

## 注意事項

- このサンプルコードは学習用途に限定されています
- 商用利用は禁止されています
- 一部のサンプルでは追加のアセットが必要な場合があります
- 書籍の該当章を参照することで、より詳細な情報を得ることができます

## ライセンス

- 本書のサンプルプログラム（特定のものを除く）の著作権は著者に帰属します
- 一部のサンプルは以下のライセンスで提供されています：
  - Unity Companion License
  - オープンソース
  - MITライセンス

## 参考リンク

- [Unity ML-Agents 公式ドキュメント](https://github.com/Unity-Technologies/ml-agents)
- [Unity 公式サイト](https://unity.com/)
- [Python 公式サイト](https://www.python.org/) 
