How to print all table content
===

def print_full(x):
    pd.set_option('display.max_rows', len(x))
    print(x)
    pd.reset_option('display.max_rows')
    
with pd.option_context('display.max_rows', 999, 'display.max_columns', 3):
    print df
    
---
ref: http://stackoverflow.com/questions/19124601/is-there-a-way-to-pretty-print-the-entire-pandas-series-dataframe
