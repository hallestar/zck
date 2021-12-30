# bash

## jq

### snippets

```bash
curl 'https://raw.githubusercontent.com/lukes/ISO-3166-Countries-with-Regional-Codes/master/all/all.json' | jq -r '.[] | [.name, ."country-code", ."alpha-3"] | @csv'
```
