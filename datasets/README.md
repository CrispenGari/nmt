### Dataset

Our dataset will contains `5` `<lang>-en.csv` files between the following south african languages:

1. `af-en` - Afrikaans to English
2. `xh-en` - Xhosa to English
3. `zu-en` - Zulu to English
4. `ts-en` - Tswana to English
5. `st-en` - Sotho to English

The following languages were filtered out on bidirectional paring between the `src(source)` and `trg(target)` where the source language was english and the target being any language among those selected:

```
ve - Venda
tn - Tswana
ss - Swati
nr - Ndebele (nd)
en - English
```

So each language contains a `name` and a `code`. In python a language type looks as follows:

```py
class Language:
  def __init__(self, code: str, name: str):
    self.name = name
    self.code = code

  def __repr__(self) -> str:
    return f"Language: <{self.name}>"

  def __str__(self) -> str:
      return f"Language: <{self.name}>"

```

The language codes where scraped on [wikipedia](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) though they were hard-coded in the notebook that creates translation dataset.
