# Применение нейросетей для прогнозирования временных рядов

На примере фреймворка [`pytorch`](https://pytorch.org)

## Установка необходимых пакетов

- `pip install torch`
- `conda install -c conda-forge torch`

## Элементы нейросети:

### Функции активации

Основные функции активации:

- линейная (тождественная)
- сигмоида (логистическое распределение)
- гиперболический тангенс `tanh`
- ReLU (rectified linear unit)

Полный список [`здесь`](https://docs.pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity) и 
[`здесь`](https://docs.pytorch.org/docs/stable/nn.html#non-linear-activations-other)

### Ячейки и слои

#### Линейный слой

Задаётся классом [`Linear`](https://docs.pytorch.org/docs/stable/generated/torch.nn.Linear.html#torch.nn.Linear) в PyTorch + слой активации

$$
\begin{aligned}
	y&=b+w_1x_1+\cdots+w_nx_n=Wx+b & y&\in\mathbb{R}^{units}
\end{aligned}
$$

#### Рекуррентный слой

Описание можно найти [здесь](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)

Основные слои:

 - [`RNN`](https://docs.pytorch.org/docs/stable/generated/torch.nn.RNN.html#torch.nn.RNN) в PyTorch
 - [`LSTM`](https://docs.pytorch.org/docs/stable/generated/torch.nn.LSTM.html#torch.nn.LSTM) в PyTorch
 - [`GRU`](https://docs.pytorch.org/docs/stable/generated/torch.nn.GRU.html#torch.nn.GRU) в PyTorch