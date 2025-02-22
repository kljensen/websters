# Webster's Revised Unabridged Dictionary (1913 + 1828) 📚💾

I started using this dictionary after read
James Somers' enjoyable article
[You’re probably using the wrong dictionary](https://jsomers.net/blog/dictionary).

I found need for formats other than stardict and so
converted the dictionary to a tab separated format (TSV)
using [pyglossary](https://github.com/ilius/pyglossary).

I hope it is useful for others.

# Accessing the data

Download the zip from this archive and unzip as you wish to
get the tsv. You can query using a variety of tools. E.g. this
is me getting the definition for beautiful using duckdb.

```
D select * from "websters-1913-1828.tsv" where word = 'Beautiful';
┌───────────┬────────────────────────────────────────────────────────────────────────────────────┐
│   word    │                                     definition                                     │
├───────────┼────────────────────────────────────────────────────────────────────────────────────┤
│ Beautiful │ Beautiful \\Beau"ti*ful\\, a.\n   Having the qualities which constitute beauty;... │
└───────────┴────────────────────────────────────────────────────────────────────────────────────┘
```

## License

That dictionary is pre-1928 and so in the public domain in the
United States. 
