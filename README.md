# Self-paced Multi-view Co-training for person re-id experiment

Thanks to Yanlu for implementing [spaco in matlab](https://github.com/syferya/SPaCo)

## Run
```shell
bash spaco.sh
```
alternatively, you can run with 
```shell
python examples/spaco.py --arch1 resnet50 --arch2 densenet121 --iter-step 5 --dataset market1501std --logs-dir logs/
```

Please cite spaco in your publications if it helps your research:  
@inproceedings{ma2017self,  
  title={Self-Paced Co-training},   
  author={Ma, Fan and Meng, Deyu and Xie, Qi and Li, Zina and Dong, Xuanyi},  
  booktitle={International Conference on Machine Learning},  
  pages={2275--2284},  
  year={2017}  
}

# Open-ReID
Open-ReID is a lightweight library of person re-identification for research
purpose. It aims to provide a uniform interface for different datasets, a full
set of models and evaluation metrics, as well as examples to reproduce (near)
state-of-the-art results.

## Installation

Install [PyTorch](http://pytorch.org/) (version >= 0.2.0). Although we support
both python2 and python3, we recommend python3 for better performance.

```shell
git clone https://github.com/Cysu/open-reid.git
cd open-reid
python setup.py install
```

## Examples

```shell
python examples/softmax_loss.py -d viper -b 64 -j 2 -a resnet50 --logs-dir logs/softmax-loss/viper-resnet50
```

This is just a quick example. VIPeR dataset may not be large enough to train a deep neural network.

Check about more [examples](https://cysu.github.io/open-reid/examples/training_id.html)
and [benchmarks](https://cysu.github.io/open-reid/examples/benchmarks.html).
