# PatchMLP 

This is an offical implementation of PatchMLP.




### Training

1. Install requirements. ```pip install -r requirements.txt```

2. Download data. You can download all the datasets from [Autoformer](https://drive.google.com/drive/folders/1ZOYpTUa82_jCcxIdTmyr0LXQfvaM9vIy). Create a seperate folder ```./dataset``` and put all the csv files in the directory.

3. Training. All the scripts are in the directory ```./scripts/PatchMLP``` and ```./scripts/PatchMLPPE```. The default model is PatchMLP/42 and PatchMLPPE/42. For example, if you want to get the multivariate forecasting results for electricity dataset with PathMLP Positional Encoding, just run the following command, and you can open ```./result.txt``` to see the results once the training is done:
```
sh ./scripts/PatchMLPPE/electricity.sh
```

You can adjust the hyperparameters based on your needs (e.g. different patch length, different look-back windows and prediction lengths.). We also provide codes for the baseline models.


```

## Acknowledgement

We appreciate the following github repo very much for the valuable code base and datasets:

https://github.com/yuqinie98/PatchTST

https://github.com/cure-lab/LTSF-Linear

https://github.com/zhouhaoyi/Informer2020

https://github.com/thuml/Autoformer

https://github.com/MAZiqing/FEDformer

https://github.com/alipay/Pyraformer

https://github.com/ts-kim/RevIN

https://github.com/timeseriesAI/tsai

## Contact

If you have any questions, please contact us: jgm667@mocs.utc.edu 

## Citation

If you find this repo useful in your research, please consider citing our paper as follows:

```
@article{GDo-2023-PatchMLP,
  title={},
  author={},
  journal={arXiv preprint arXiv:2211.14730},
  year={2023}
}
```

