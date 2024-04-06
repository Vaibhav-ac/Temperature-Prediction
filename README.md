# Temperature Prediction

This notebook implements a many-to-one Recurrent Neural Network (RNN) model for time series analysis to predict the mean temperature by analyzing previous days' data. The implementation of the neural network model was done using [Keras](https://keras.io/).

Instead of RNNs, Long Short-Term Memory networks (LSTMs) can also be used. Here, the window size for previous data was taken as 7 days (one week) to predict the mean temperature for the 8th day. As 7 days is not a very long context, RNNs can work just fine.

Some blogs and videos that helped me build a proper understanding and improve this notebook are referenced below:

- [Jason Brownlee's Blog](https://machinelearningmastery.com/understanding-simple-recurrent-neural-networks-in-keras/) about RNN in Keras
- [Greg Hogg's Video](https://youtu.be/kGdbPnMCdOg?si=2OgtqRvoZGXrtxhf) about Multivariate Time Series Forecasting
- [Colah's Blog](https://colah.github.io/posts/2015-08-Understanding-LSTMs/) about LSTMs
- [Philippe Remy's Blog](https://philipperemy.github.io/keras-stateful-lstm/) about Stateful LSTM in Keras

Furthermore, the dataset used in the notebook is taken from [Kaggle](https://www.kaggle.com/datasets/sumanthvrao/daily-climate-time-series-data).

## Requirements
- TensorFlow version 2.10.1
- Keras version 2.10.0
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

(Note: TensorFlow versions above 2.10 are not supported on GPU on Windows Native, which is why these specific versions were used.)
