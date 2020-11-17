



## Efficient Warm Restart Projected Gradient Descent (EWR-PGD)

We propose a new white box adversarial attack method named EWR-PGD which exceeds the state-of-the-art attacks performance. It is more efficient than the state-of-the-art [ODI-PGD](https://github.com/ermongroup/ODS) method.

**Code will be available soon.**

* * *
### Comparison of  EWR-PGD and ODI-PGD 
**When reducing the models to the same accuracy, the number of restarts required by the EWR-PGD significantly less than that of the ODI-PGD. EWR-PGD is up to roughly 5 times faster than ODI-PGD.**



![image](./imgs/result1.bmp)

![image](./imgs/result2.png)

Figure 1. On 10 state-of-the-art defense models, comparison of the number of restarts required (the lower the better) when the EWR-PGD and ODI-PGD method reduce the models to the same accuracy.

The models are available online:

* [TRADES-Small Cnn, TRADES-WRN](https://github.com/yaodongyu/TRADES)
* [Mardy-WRN](https://github.com/MadryLab/cifar10_challenge)
* [MART-ResNet18, MART-WRN](https://github.com/YisenWang/MART)
* [FBTF-ResNet18](https://github.com/anonymous-sushi-armadillo/fast\_is\_better\_than\_free\_CIFAR10)
* [pytorch ResNeXt101-DenoiseAll, ResNet152-Denoise, ResNet152-Baseline(https://github.com/TransEmbedBA/TREMBA)

* * *

### Results on 3 White-box leaderboards

**EWR-PGD ranks first on the TRADES white-box MNIST and CIFAR-10 leaderboards, reducing the accuracy of their MNIST model to 92.52% and the accuracy of their CIFAR-10 model to 52.95%. EWR-PGD also ranks first on MardyLab’s White-box CIFAR-10 leaderboard, reducing the accuracy of their CIFAR-10 model to 43.96%.**

Table 1. Accuracy(the lower the better) under EWR-PGD and SOTA attacks and corresponding complexity.

| dataset |model  | EWR-PGD   |EWR-PGD complexity | SOTA | SOTA complexity
| --- | --- | --- | --- | --- | --- |
| MNIST  | [TRADES-SMN](https://github.com/yaodongyu/TRADES ) | **92.52%** | **(20+300)×800** | 92.58% | ------------- |
| CIFAR-10 | [TRADES-WRN](https://github.com/yaodongyu/TRADES) | **52.96%** |**(5+100)×30**  | 53.01% |  (10+150)×20 |
| CIFAR-10 | [Mardy-WRN](https://github.com/MadryLab/cifar10_challenge) | **43.96%** | **(5+100)×30**  | 43.99% | (10+150)×20 |

* * *
### Results on CIKM2020 Analyticup: Alibaba-Tsinghua Adversarial Challenge on Object Detection

**EWR-PGD ranks first among 1701 teams in [CIKM2020 Analyticup: Alibaba-Tsinghua Adversarial Challenge on Object Detection](https://tianchi.aliyun.com/competition/entrance/531806/rankingList). Surpassing the runner-up approach by∼14% in terms of scores.**

* * *

### contact
Please contact **liuye_ly94@163.com** if you have any question.Enjoy!