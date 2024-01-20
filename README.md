# JS Trace ID Formatter

This app converts a list of trace IDs separated by new lines, into a list of double-quoted, comma-separated trace IDs.

From this:

```
b413dddbac91b251782bb7cdeac6803f
5ad56251a19cd4ad0a60fc99e45e437c
d7e3feb59d52154d406167422611708f
ed2b4f48e2a20300c55862c72f86574b
```

to this:
```
"b413dddbac91b251782bb7cdeac6803f", "5ad56251a19cd4ad0a60fc99e45e437c", "d7e3feb59d52154d406167422611708f", "ed2b4f48e2a20300c55862c72f86574b"
```


The original list of trace IDs is retrieved from copying cells in a spreadsheet, which adds a new line between each cell. When submitting multiple trace IDs to be searched in Sumo Logic, each trace ID needs to be surrounded in double-quotes, and separated by commas. 
