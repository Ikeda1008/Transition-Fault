# Transition-Fault Simulation

このプロジェクトは、卒業研究”AIアクセラレータ演算器の遅延故障シミュレーション”を行うためのコード。

## 研究の目的
- AIアクセラレータにおける演算器の遅延故障（Delay Fault）の影響を評価する。
- 故障検出や診断アルゴリズムの検証。
  
## コードの説明
- 8値論理シミュレーションを実装。以下の3つのビット配列。
-vals_bp[0] = Final（V2サイクルでの最終状態）
-vals_bp[1] = Initial（V1サイクルでの初期状態）
-vals_bp[2] = Activity（V1からV2へ遷移したかどうかのフラグ
- inject_cb（コールバック）を使って Activity ビットと Initial/Final ビットの論理積を取ることで、Rise/Fallを特定した。
## 開発環境
- Python 3
- KyuPy

