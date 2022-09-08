<h1 align="center">Future weather forecasting</h1>
<div align="center">

![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg) ![macOS](https://svgshare.com/i/ZjP.svg) ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg) [![Only 32 Kb](https://badge-size.herokuapp.com/Naereen/StrapDown.js/master/strapdown.min.js)](https://github.com/mohsin-riad/bijoy-to-unicode-automation/blob/main/Source/main.ipynb)

</div>

<h2 align="center">Future Weather prediction using Prophet</h2>
<hr>
<h2 align="center">Installation</h2>

> Open terminal

```
    git clone https://github.com/mohsin-riad/future-weather-forecasting.git
    cd future-weather-forecasting
```

<h2 align="center">Dataset Intro</h2>

The series of data points plotted against time is known as time series. It is a de-facto analysis technique used in market evaluation and in weather forecast. It is an exciting topic to study as it somehow tends to predict the future, which we are always interested in.

There are two types of Machine Learning(ML) models that are used for time series analysis:

-Temporal Dependence Model

-General Additive Model (GAM)

<h2 align="center">Prophet (additive model)</h2>

Prophet is a powerful time series analysis package released by Core Data Science Team at Meta. It is simple and easy to go package for performing time series analytics and forecasting at scale.

<img width=“964” src=a../asset/1.png>

Prophet uses a decomposable time series model with three main model components: trend, seasonality, and holidays. They are combined in the following equation:

```y(t) = g(t) + s(t) + h(t) + e(t)```

Here, `g(t)` is a trend function which models the non-periodic changes. It can be either a linear function or a logistic function.
`s(t)` represents a periodic changes i.e weekly, monthly, yearly. An yearly seasonal component is modeled using Fourier series and weekly seasonal component using dummy variables.
`h(t)` is a function that represents the effect of holidays which occur on irregular schedules.`(n≥1 days)`
The term e(t) represents error changes that are not accommodated by the model.
The research paper for prophet can be found here.

> **Installation**

```pip install fbprophet```
or
```python -m pip install prophet```

<h2 align="center">Important Links</h2>

- [Prophet doc](https://facebook.github.io/prophet/docs/quick_start.html#python-api)
- [Prophet Source](https://github.com/facebook/prophet)
- [Blog](https://research.facebook.com/blog/2017/02/prophet-forecasting-at-scale/)