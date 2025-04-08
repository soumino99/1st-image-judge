# 1st-image-judge

PyTorchを用いた画像分類プロジェクトです。学生チームによる短期間の実装・検証を目的としています。

## 概要

- **検出対象**: 肺炎（Pneumonia） vs 正常（Normal）
- **目的**:
  - 機械学習・深層学習の基礎理解
  - 小規模チームによる実装・分析・可視化の経験
  - インターン応募やポートフォリオとして提示できる成果物の作成
- **将来的な応用**:
  - 医療画像分類や他タスクへの応用
  - Webアプリ化

## 技術スタック

- **言語**: Python 3.10+
- **フレームワーク**: PyTorch（torch, torchvision）
- **開発環境**: VS Code + Jupyter Notebook（ローカル実行環境）
- **可視化／前処理**: matplotlib, seaborn, OpenCV
- **バージョン管理**: Git / GitHub
- **コミュニケーション**: Slack

## プロジェクト構成

- **data/**: 学習・検証・テスト画像（Git管理対象外）
- **notebooks/**: 分析・学習用Notebook（3部構成）
- **src/**: モデル構築・学習・データ処理スクリプト
- **models/**: 学習済みモデル（`.pt`）
- **assets/**: 可視化用画像（混同行列・Grad-CAMなど）
- **Docs/**: ドキュメント全般
- **MyDocs/**: 個人的なメモ

## Notebookファイル

1. **01_data_check.ipynb**: データ可視化・構成確認
2. **02_model_train.ipynb**: 転移学習ベースのCNNモデル学習
3. **03_eval_visualize.ipynb**: 評価指標・混同行列・誤分類表示・Grad-CAM

## 学習モデル

- **モデル**: 転移学習ベース（例: ResNet18）
- **出力層**: 2クラス分類向けに変更（肺炎 or 正常）
- **損失関数**: CrossEntropyLoss
- **最適化**: Adam
- **評価**: Accuracy・混同行列・Grad-CAM可視化

## 今後の展望

- 精度改善（データ拡張・ハイパーパラメータ調整）
- Grad-CAM等の可視化強化
