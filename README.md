# Dukascopy data feed extractor

dsdfe is **not** affiliated, endorsed, or vetted by Dukascopy Europe IBS AS. It's
an open-source tool that is intended for **personal** research and educational purposes only.
For more information regarding the terms of use refer to the legal section of the [dukascopy website](https://www.dukascopy.com/).


## Install
requires python >= 3.9
```
pip install dsdfe
```

## Extract

```python
import dsdfe

symbol = 'eurusd'
range = dsdfe.generate_datetime_range("2021-01-01", "2021-01-05")

dsdfe.extract(symbol, range)
```

## Transform

```python
import dsdfe

bi5 = 'out/EURUSD_20210101_20210104.bi5'
csv = 'out/EURUSD_20210101_20210104.csv'

df = dsdfe.transform(bi5, csv)
```
