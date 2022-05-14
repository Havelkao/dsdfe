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
