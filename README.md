# particlenet-toptagging
研究用。ParticleNetのチュートリアルとして、top vs QCD classificationを行う。

## Links
- [ArXiv:1902.08570 ParticleNet: Jet Tagging via Particle Clouds](https://arxiv.org/abs/1902.08570)
- [Top Quark Tagging Reference Dataset](https://zenodo.org/record/2603256#.Y80FFMnP1D8)
- [kerasで同様のことを行っている例。基本的にはこれを参考にする](https://github.com/hqucms/ParticleNet)


## Setup
- uproot_methodsがnumpy<=1.23じゃないと動かないので注意
- とりあえず、`pip freeze`したものを`requirements.txt`に書いてあるので、それを使う

```
pip install -r requirements.txt
mkdir models processed
```

## Usage
- `1_check_dataset.ipynb`でデータセットの確認（別に動かす必要はない）
- `2_preprocessing.ipynb`でデータの前処理（`/processed/`以下にデータセットが作成されます）
- `3_train.ipynb`で学習（`/models/`以下にモデルと学習履歴が保存されます）