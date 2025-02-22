<h1 align="center">
  Webster's Revised Unabridged Dictionary
  <br>(1913 + 1828)
</h1>

I started using this dictionary after read
James Somers' enjoyable article
[You’re probably using the wrong dictionary](https://jsomers.net/blog/dictionary).
I found need for formats other than stardict and so
converted the dictionary to a tab separated format (TSV)
using [pyglossary](https://github.com/ilius/pyglossary).
I hope it is useful for others.

## Accessing the data

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

The definitions are in plaintext like this, for "Desireous":

```
Desirous \De*sir"ous\, a. [F. d['e]sireux, OF. desiros, fr.
   desir. See {Desire}, n.]
   Feeling desire; eagerly wishing; solicitous; eager to obtain;
   covetous.

         Jesus knew that they were desirous to ask him. --John
                                                  xvi. 19.

         Be not desirous of his dainties.         --Prov. xxiii.
                                                  3.
```

## License

That dictionary is pre-1928 and so in the public domain in the
United States. 
