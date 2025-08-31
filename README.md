# 🖼️ Background Image Processor

画像に美しい背景を追加するPythonスクリプトです。入力画像を指定されたサイズの背景画像の中央に配置し、プロフェッショナルな画像を作成します。

## ✨ 主な特徴

- 🎨 **カスタマイズ可能な背景**: サイズ、色、配置を自由に設定
- 📐 **アスペクト比保持**: 元画像の比率を維持しながらリサイズ
- 🚀 **一括処理**: 複数の画像を同時に処理
- 💾 **多形式対応**: PNG、JPEG、JPG形式をサポート
- ⚡ **高速処理**: 効率的な画像処理アルゴリズム

## 🛠️ 必要な環境

- **Python**: 3.6以上
- **ライブラリ**: Pillow (PIL)

## 📦 インストール

### 1. リポジトリのクローン
```bash
git clone https://github.com/TanakaMikihisa/get_Background_image.git
cd get_Background_image
```

### 2. 依存関係のインストール
```bash
pip install -r requirements.txt
```

## 📁 プロジェクト構造

```
get_Background_image/
├── 📄 background_image.py    # メインスクリプト
├── 🖼️ examples/             # サンプル画像
├── 📥 input_images/         # 入力画像フォルダ
├── 📤 output_images/        # 出力画像フォルダ
├── 📋 requirements.txt      # 依存関係
└── 📖 README.md            # このファイル
```

## 🎯 使用方法

### 基本的な使い方

1. **画像の準備**
   - `input_images/` フォルダに処理したい画像を配置
   - 対応形式: PNG、JPEG、JPG

2. **スクリプトの実行**
   ```bash
   python background_image.py
   ```

3. **結果の確認**
   - 処理された画像が `output_images/` フォルダに保存されます

### 設定のカスタマイズ

スクリプト内で以下の設定を変更できます：

| 設定項目 | 説明 | デフォルト値 |
|---------|------|-------------|
| `BASE_IMAGE_WIDTH` | 背景画像の幅 | 5000px |
| `BASE_IMAGE_HEIGHT` | 背景画像の高さ | 3750px |
| `BASE_IMAGE_COLOR` | 背景色（RGB） | (89, 156, 170) |
| `TARGET_HEIGHT` | 中央画像の高さ | 2500px |

## 📸 サンプル画像

examplesフォルダには以下のサンプル画像が含まれています：

- 🎡 **梅田観覧車.png** - 大阪の梅田スカイビルの観覧車
![梅田観覧車](examples/梅田観覧車.png)

- 🏘️ **沖縄街並み.png** - 沖縄の伝統的な街並み
![沖縄街並み](examples/沖縄街並み.png)

- 🔴 **null2赤.png** - 赤色のサンプル画像
![null2赤](examples/null2赤.png)

- 📚 **君の名は.png** - アニメ「君の名は。」の画像
![君の名は](examples/君の名は.png)
## 🔧 カスタマイズ例

### 背景色の変更
```python
BASE_IMAGE_COLOR = (255, 0, 0)  # 赤色
BASE_IMAGE_COLOR = (0, 255, 0)  # 緑色
BASE_IMAGE_COLOR = (0, 0, 255)  # 青色
```

### サイズの変更
```python
BASE_IMAGE_WIDTH = 4000   # 幅を4000pxに
BASE_IMAGE_HEIGHT = 3000  # 高さを3000pxに
```

## 🚀 高度な使用方法

### バッチ処理
複数の画像を一度に処理する場合：
1. `input_images/` フォルダに複数の画像を配置
2. スクリプトを実行
3. すべての画像が自動的に処理されます

### 出力形式の指定
現在は元画像の形式が保持されますが、必要に応じて変換も可能です。

## 🤝 貢献

このプロジェクトへの貢献を歓迎します！

- 🐛 **バグ報告**: 問題を見つけた場合はIssueを作成
- 💡 **機能提案**: 新しい機能のアイデアがあれば共有
- 🔧 **プルリクエスト**: 改善案があればPRを送信

## 📄 ライセンス

このプロジェクトは [MIT License](LICENSE) の下で公開されています。

## 📞 サポート

質問や問題がある場合は、GitHubのIssueページでお気軽にお声かけください。

---

⭐ このプロジェクトが役立ったら、スターを付けてください！