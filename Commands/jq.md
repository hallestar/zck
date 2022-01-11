# jq

## snippets

- 取国家/地区码并以csv输出

```bash
curl 'https://raw.githubusercontent.com/lukes/ISO-3166-Countries-with-Regional-Codes/master/all/all.json' | jq -r '.[] | [.name, ."country-code", ."alpha-3"] | @csv'

...
"Virgin Islands (U.S.)","850","VIR"
"Wallis and Futuna","876","WLF"
"Western Sahara","732","ESH"
"Yemen","887","YEM"
"Zambia","894","ZMB"
"Zimbabwe","716","ZWE"
```

- 列出所有keys

```bash
curl 'https://raw.githubusercontent.com/lukes/ISO-3166-Countries-with-Regional-Codes/master/all/all.json' | jq ".[0] | keys"
[
  "alpha-2",
  "alpha-3",
  "country-code",
  "intermediate-region",
  "intermediate-region-code",
  "iso_3166-2",
  "name",
  "region",
  "region-code",
  "sub-region",
  "sub-region-code"
]
```

- 取某个值

```bash
curl 'https://raw.githubusercontent.com/lukes/ISO-3166-Countries-with-Regional-Codes/master/all/all.json' | jq '.[0] | ."alpha-2"'
"AF"
```
