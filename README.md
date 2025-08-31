# Background Image Processor

画像に背景を追加するPythonスクリプトです。入力画像を指定されたサイズの背景画像の中央に配置し、新しい画像として保存します。

## 🚀 機能

- 指定されたサイズ（5000x3750ピクセル）の背景画像を生成
- 入力画像を背景の中央に配置
- アスペクト比を保持したまま画像をリサイズ
- 複数の画像ファイルを一括処理
- PNG、JPEG、JPG形式に対応

## 📋 必要な環境

- Python 3.6以上
- Pillow (PIL) ライブラリ

## 🔧 インストール

1. リポジトリをクローン
```bash
git clone https://github.com/TanakaMikihisa/get_Background_image.git
cd get_Background_image
```

2. 必要なライブラリをインストール
```bash
pip install -r requirements.txt
```

## 📁 フォルダ構成

```
get_Background_image/
├── background_image.py      # メインスクリプト
├── input_images/           # 処理したい画像を配置
├── output_images/          # 処理後の画像が保存される
├── requirements.txt        # 依存関係
└── README.md              # このファイル
```

## 🎯 使用方法

1. `input_images/` フォルダに処理したい画像ファイル（PNG、JPEG、JPG）を配置
2. スクリプトを実行
```bash
python background_image.py
```
3. 処理された画像が `output_images/` フォルダに保存されます

## ⚙️ 設定

スクリプト内で以下の設定を変更できます：

- `BASE_IMAGE_WIDTH`: 背景画像の幅（デフォルト: 5000px）
- `BASE_IMAGE_HEIGHT`: 背景画像の高さ（デフォルト: 3750px）
- `BASE_IMAGE_COLOR`: 背景色（デフォルト: RGB(89, 156, 170)）
- `TARGET_HEIGHT`: 中央に配置する画像の高さ（デフォルト: 2500px）

## 📸 使用例

入力画像を背景画像の中央に配置し、アスペクト比を保持したままリサイズして保存します。

## 🤝 貢献

プルリクエストやイシューの報告を歓迎します。

## 📄 ライセンス

このプロジェクトはMITライセンスの下で公開されています。