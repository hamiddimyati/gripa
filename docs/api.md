# API Reference

There is only one module, `gripa.Gripa`, that can be used for detecting anomalies in time series.

> *class* gripa.**Gripa**(*window_size=11, algorithm="hpf", threshold=3*)

### Parameters
* `window_size`: *int or float, default=11*
* `algorithm`: *{"hpf", "ssa"}, default="hpf"*
* `threshold`: *float, default=3*

### Attributes
* `anomaly_score`: score for labelling anomaly

### Methods
* `fit(X)`: train the Gripa model, which can generate attribute `anomaly_score`
* `fit_predict(X)`: train and generate anomaly labels (`True` or `False`)
