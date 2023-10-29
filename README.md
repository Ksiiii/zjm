# zjm
深度神经网络在机器学习中应用时面临两类主要问题：优化问题和泛化问题。

优化问题：深度神经网络的优化具有挑战性。

神经网络的损失函数通常是非凸函数，因此找到全局最优解往往困难。
深度神经网络的参数通常非常多，而训练数据也很大，因此使用计算代价较高的二阶优化方法不太可行，而一阶优化方法的训练效率通常较低。
深度神经网络存在梯度消失或梯度爆炸问题，导致基于梯度的优化方法经常失效。
泛化问题：由于深度神经网络的复杂度较高且具有强大的拟合能力，很容易在训练集上产生过拟合现象。因此，在训练深度神经网络时需要采用一定的正则化方法来提高网络的泛化能力。

目前，研究人员通过大量实践总结了一些经验方法，以在神经网络的表示能力、复杂度、学习效率和泛化能力之间取得良好的平衡，从而得到良好的网络模型。本系列文章将从网络优化和网络正则化两个方面来介绍如下方法：

在网络优化方面，常用的方法包括优化算法的选择、参数初始化方法、数据预处理方法、逐层归一化方法和超参数优化方法。
在网络正则化方面，一些提高网络泛化能力的方法包括ℓ1和ℓ2正则化、权重衰减、提前停止、丢弃法、数据增强和标签平滑等。


本文主要实现Adagrad算法、RMSProp算法、Adam算法，和简单的参数初始化、批量规范化和层归一化。

本人运行代码的环境是Python 3.7.16和torch版本如下：<img width="325" alt="image" src="https://github.com/Ksiiii/zjm/assets/139730257/f7972ca5-f5f3-4cc1-a8e1-cda8945f5a75">
其他版本只要相对应torch和cuda应该可以运行
